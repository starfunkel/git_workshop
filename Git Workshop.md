# <center>Git Pizza Freitag</center>

## <center>Ein Vortrag vom Versionieren</center>

</br><div style="margin-left: auto;
            margin-right: auto;
            width: 35%">

![Happy with Git](assets/git-commit-organized.jpg)</div></br>

#### <center>Von Christian Rathnau</center></br>

<div style="margin-left: 350px;
            width: 35%
            ">

![integrate](assets/integrate.png)</div></br></br></br></br></br></br></br>

***
</br></br>
## <center> 1. Was ist ein Version Control System ?</center></br></br></br>

<div style="margin-left: auto;
            margin-right: auto;
            width: 75%">

 - Unterstützt bei der <b>Organisation von Projektdateien</b> jedweder Art</div></br>
 
 <div style="margin-left: auto;
            margin-right: auto;
            width: 75%">

![Symbolbild](assets/Symbolbild.png)</div></br>

<div style="margin-left: auto;
            margin-right: auto;
            width: 75%">

- Ermöglicht <b>Änderungsrückverfolgung</b> von Projektdateien</div></br></br>

<div style="margin-left: auto;
            margin-right: auto;
            width: 75%">

![Git Desktop](assets\git_desktop_changes.png)</div></br>

<div style="margin-left: auto;
            margin-right: auto;
            width: 75%">

- Ermöglicht den <b>Urheber</b> einer jeden Änderung zu identifizieren</div></br>

<div style="margin-left: auto;
            margin-right: auto;
            width: 75%">

![Git Desktop](assets\git_desktop_author.png)</div></br></br></br></br>

***
</br></br></br></br></br></br></br></br>

## <center>Boah wat?  Code? ... Konfig Dateien? ...</br> Pah! Ich benutze GUI !!1!1</center></br></br></br></br></br>

## <center><b>Hold your beer!!</b></center></br></br>

<div style="margin-left: auto;
            margin-right: auto;
            width: 75%">

![drunk_baby](assets\drunk_baby.png)</div></br></br></br></br></br></br></br></br></br>





### <center>GUIs ändern sich</center></br>

 
<div style="margin-left: auto;
            margin-right: auto;
            width: 75%">

![wget_win_old](assets\old_wgetgui-screenshot.png)</div>



<div style="margin-left: auto;
            margin-right: auto;
            width: 75%">

![wget_win_new](assets\new_wget_gui.jpg)
</div></br></br>

<div style="margin-left: auto;
            margin-right: auto;
            width: 75%">

 - GUIs bilden i.d.R. nicht alle Features ab</div></br></br>

<div style="margin-left: auto;
            margin-right: auto;
            width: 75%">

 ![wget_win_new](assets\wget-cli.png)</div></br></br>








</br></br></br></br></br></br></br></br></br></br></br></br>

***
## <center>Real Life Beispiele</center>

</br></br></br>

### <center>Konfigdateien im Windows Umfeld (Fokus Administration)</center>

</br></br>

<div style="margin-left: auto;
            margin-right: auto;
            width: 70%">

|Switch Konfigs|Router Konfigs|Schedlued Task|Generic xmls|CMD, PoSh, Python Scripts|csv Dateien, Text Dateien|[*]
|-|-|-|-|-|-|-|
</br>
<center>[*]: Prinzipiel lassen sich alle Dateitypen mit Git versionieren. Bei Konfigdateien liegt der Vorteil auf der Hand. Man kann die Änderungen lesen.
</div>

</br></br></br></br></br></br></br></br></br>

#### <center>Dabei sind mit Git versionierte Dateien nicht bloße Historienketten von in der Vergangenheit gespeichertem Code.</center>

</br></br></br>

#### <center>Ein weiterer zentraler Ansatz ist die die Möglichkeit der Kollaboration im Team, oder völlig fremden Menschen über  einer Organisationsgrenzen.</center>

</br></br></br></br></br></br></br></br></br></br></br></br>

***
## <center>Ein typerischer Workflow</center>

Anfang

<div style="margin-left: auto;
            margin-right: auto;
            width: 70%">

![Alt text](https://wac-cdn.atlassian.com/dam/jcr:223f5106-2191-4450-8916-e5c80d7d907a/02.svg?cdnVersion=800)
</div>

lunch time

```bash
git status
git add <some-file>
git commit -m 'some usefull message'
git push
```

<div style="margin-left: auto;
            margin-right: auto;
            width: 70%">

![Alt text](https://wac-cdn.atlassian.com/dam/jcr:e2c88c1b-fb28-46a3-93be-c1c45f86bd1c/03%20(1).svg?cdnVersion=800)
</div>

git push -u origin marys-feature

<div style="margin-left: auto;
            margin-right: auto;
            width: 70%">

![Alt text](https://wac-cdn.atlassian.com/dam/jcr:d0c471b4-61c8-4005-86bc-904d894e391b/04.svg?cdnVersion=800)
</div>

merging
<div style="margin-left: auto;
            margin-right: auto;
            width: 70%">

![Alt text](https://wac-cdn.atlassian.com/dam/jcr:09308632-38a3-4637-bba2-af2110629d56/07.svg?cdnVersion=800)

general Working

<div style="margin-left: auto;
            margin-right: auto;
            width: 70%">

![Alt text](https://wac-cdn.atlassian.com/dam/jcr:a13c18d6-94f3-4fc4-84fb-2b8f1b2fd339/01%20How%20it%20works.svg?cdnVersion=800)
</div>

branches

<div style="margin-left: auto;
            margin-right: auto;
            width: 70%">

![Alt text](https://wac-cdn.atlassian.com/dam/jcr:34c86360-8dea-4be4-92f7-6597d4d5bfae/02%20Feature%20branches.svg?cdnVersion=800)
</div>

release

<div style="margin-left: auto;
            margin-right: auto;
            width: 70%">

![Alt text](https://wac-cdn.atlassian.com/dam/jcr:8f00f1a4-ef2d-498a-a2c6-8020bb97902f/03%20Release%20branches.svg?cdnVersion=800)
</div>







<div style="margin-left: 600px;
            width: 35%
            ">

![integrate](/Pizza%20Freitag/assets/integrate.png)
</div>

****