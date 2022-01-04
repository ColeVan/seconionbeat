# Security Onion Beats and Sysmon deployment files

These zip files will help speed up the process for deploying sysmon v13 (with Olaf Hartong config.xml) and winlogbeats 7.16.2 (with winlogbeat.yml). 

https://github.com/olafhartong/sysmon-modular

https://www.elastic.co/downloads/past-releases/winlogbeat-7-16-2

Download both folders and extract all to see the contents.

The folder "seconion" can be placed in "C:\Windows\Temp" and executed with the following light-weight-agent-deployment.ps1 file.

The powershell script will install both sysmon and seconionbeat (aka "winlogbeats").

Note: You can name the beat agent and yml file whatever you like. Make edit scripts with proper file location so that agents binaries install properly.

![Screenshot 2022-01-04 055843](https://user-images.githubusercontent.com/70167373/148050106-f2a45824-6b8a-44b8-b64d-c6955783c1ff.png)

![Screenshot 2022-01-04 060924](https://user-images.githubusercontent.com/70167373/148050464-6c5038e9-f888-4761-86ed-4f4084d4612a.png)
