# Security Onion Beats and Sysmon deployment files

This repo will help speed up the process for deploying sysmon v13 (with Olaf Hartong config.xml) and winlogbeats 7.17.1 (with winlogbeat.yml). 

https://github.com/olafhartong/sysmon-modular

https://www.elastic.co/downloads/past-releases/winlogbeat-7-16-2

Download both folders and extract all contents.

The folder "seconion" can be placed in "C:\Windows\Temp" and executed with the following light-weight-agent-deployment.ps1 file.

The folder "seconion(With_bat_file)" can also be placed in "C:\Windows\Temp" and executed with start-scripts-sysmon-seconionbeat.ps1 file which will kick off the batch script "seconionbeat-deploy-script.bat" #Note: Ensure to rename folder "seconion(With_bat_file)" to "seconion" before running ps1 file.

The powershell script will install both sysmon and seconionbeat (aka "winlogbeats").

Note: You can name the beat agent and yml file whatever you like. Make sure to edit scripts with proper file location and naming convnetion so that binaries install properly.

![Screenshot 2022-01-04 055843](https://user-images.githubusercontent.com/70167373/148050106-f2a45824-6b8a-44b8-b64d-c6955783c1ff.png)

# light-weight-agent-deployment.ps1

![Screenshot 2022-01-04 060924](https://user-images.githubusercontent.com/70167373/148050464-6c5038e9-f888-4761-86ed-4f4084d4612a.png)


# seconionbeat.yml

Before installing, ensure you change the IP of the SIEM you will be sending windows event logs to in the yml file below.

![Screenshot 2022-01-04 061335](https://user-images.githubusercontent.com/70167373/148050978-3e0afad5-3db8-4c72-a5f9-89690108ac6b.png)
