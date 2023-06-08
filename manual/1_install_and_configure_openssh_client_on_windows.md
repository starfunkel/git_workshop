# Install OpenSSH Client on Windows

```powershell
# Add Windows Capeability
Add-WindowsCapability -Online -Name OpenSSH.Client~~~~0.0.1.0
# Start the sshd service
Start-Service sshd


# OPTIONAL but recommended:
Set-Service -Name sshd -StartupType 'Automatic'

# Confirm the Firewall rule is configured. It should be created automatically by setup. Run the following to verify
if (!(Get-NetFirewallRule -Name "OpenSSH-Server-In-TCP" -ErrorAction SilentlyContinue | Select-Object Name, Enabled)) {
    Write-Output "Firewall Rule 'OpenSSH-Server-In-TCP' does not exist, creating it..."
    New-NetFirewallRule -Name 'OpenSSH-Server-In-TCP' -DisplayName 'OpenSSH Server (sshd)' -Enabled True -Direction Inbound -Protocol TCP -Action Allow -LocalPort 22
} else {
    Write-Output "Firewall rule 'OpenSSH-Server-In-TCP' has been created and exists."
}
```

## Navigate to %USERPROFILE%/.ssh (if .ssh does not exist create it now)

```powershell
PS ~\.ssh> ssh-keygen.exe
Generating public/private rsa key pair.
Enter file in which to save the key (%USERPROFILE%/.ssh/id_rsa): $KEY.rsa
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in $KEY.rsa.
Your public key has been saved in $KEY.rsa.pub.
The key fingerprint is:
SHA256:xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
integrate-it\rathnau@II-LAP-60
The keys randomart image is:
+---[RSA 3072]----+
|...o .oo..++. o  |
|... = oo.=o..+ . |
|.. o + .o B.. o .|
|. + . ..+= + o . |
| . +   +S=* +    |
|        *.++ o   |
|       . +. .    |
|         .       |
|        .E       |
+----[SHA256]-----+

```

## Setup ssh to communicate with Github
<br>

```powershell
# Edit 
%USERPROFILE%\.ssh\config
```

- Add 

```powershell
Host *
    AddKeysToAgent yes
    IdentitiesOnly yes

# and

Host github.com
    HostName github.com
    User your_user_name
    IdentityFile ~/.ssh/KEY.rsa

```

- Run ssh-add to connect your fresh identity file with the SSH daemon / service

```powershell
ssh-add ~/.ssh/your_file_name
```

