# OrchardSkills.OrchardCore.WindowsOnRaspberryPi

Orchard Core IoT Windows 10 Development Environment on a Raspberry Pi 4

With your favorite browser, head over to: 

Download a clean windows 10 on arm image from https://uup.rg-adguard.net/

![WoR-001](https://user-images.githubusercontent.com/59172485/103178291-b2cec680-483e-11eb-86ee-b27e15f1eead.png)

For Select type select Windows (Insider Version)

For Select version select Windows 10 Insider Preview 21277.1000(rs_prerelease)[arm64]

For Select language select en-us: English (United States)

For Select edition select Windows 10 Professional

For Select type download select Download ISO compiler in OneClick! (run download CMD-file) 

Click on the download link on the right creatingISO_21277.1000_en-us_arm64_professional.cmd

![WoR-002](https://user-images.githubusercontent.com/59172485/103178293-bc582e80-483e-11eb-8aa8-3914612f8a5e.png)

Click on Keep

![WoR-003](https://user-images.githubusercontent.com/59172485/103180011-ee718c80-484e-11eb-9249-8ab811202a26.png)

File is downloaded in the Download folder.

![WoR-004](https://user-images.githubusercontent.com/59172485/103180012-ee718c80-484e-11eb-8b0d-d01eec71621c.png)

Create a new folder

![WoR-005](https://user-images.githubusercontent.com/59172485/103180014-ef0a2300-484e-11eb-8500-65a0c30bde8b.png)

Name the folder WOR-ISO

![WoR-006](https://user-images.githubusercontent.com/59172485/103180015-ef0a2300-484e-11eb-873c-8f55754ac4bb.png)

Move the file creatingISO_21277.1000_en-us_arm64_professional.cmd tp the WOR-ISO folder

![WoR-007](https://user-images.githubusercontent.com/59172485/103180016-ef0a2300-484e-11eb-94be-045a72813d12.png)

Click on the creatingISO_21277.1000_en-us_arm64_professional.cmd file to select it and the right click and select Run as administrator.

![WoR-008](https://user-images.githubusercontent.com/59172485/103180017-efa2b980-484e-11eb-8913-8c7ae7b2ff11.png)

Click on More info link

![WoR-009](https://user-images.githubusercontent.com/59172485/103180018-efa2b980-484e-11eb-803a-43121eefa988.png)

Click on Run anyway

![WoR-010](https://user-images.githubusercontent.com/59172485/103180019-efa2b980-484e-11eb-9342-883803019847.png)

This will start the process of creating an ISO file.


![WoR-011](https://user-images.githubusercontent.com/59172485/103180020-efa2b980-484e-11eb-97a4-7e976e78801b.png)

The process will complete. Press any key to exit.

![WoR-012](https://user-images.githubusercontent.com/59172485/103180021-f03b5000-484e-11eb-8d46-ed5f21385d2e.png)

The ISO file is generated.

Download NTlite From https://www.ntlite.com/download/

![WoR-013](https://user-images.githubusercontent.com/59172485/103230514-e834ec00-48f2-11eb-8ba8-7342249a725c.png)

![WoR-014](https://user-images.githubusercontent.com/59172485/103230516-e8cd8280-48f2-11eb-808d-bb977b0293a0.png)

![WoR-015](https://user-images.githubusercontent.com/59172485/103230517-e9661900-48f2-11eb-9ab0-0644a2069a76.png)

![WoR-016](https://user-images.githubusercontent.com/59172485/103230519-e9661900-48f2-11eb-827a-0224158c9be0.png)

![WoR-017](https://user-images.githubusercontent.com/59172485/103230520-e9661900-48f2-11eb-8c99-22e9ba591a61.png)

![WoR-018](https://user-images.githubusercontent.com/59172485/103230521-e9feaf80-48f2-11eb-865a-821571239955.png)

Download 7-Zip From https://www.7-zip.org/download.html

Extract Install.wim from the sources folder inside your windows 10 on arm iso
Windows10.iso > Sources > Install.wim

Open NTlite Then Load Install.wim
In NTLite You should see a Presets Tab on the top left , Click on import then load 0.3.0.xml
On your Right you should see 0.3.0 , Double click it
Then on your Left click on Regestry
Drag the registry files there

Click on Apply

After its done Right click your Install.wim file and open it with 7-Zip
after that you can Modify the image directly

[Modify]
C:\Windows\Cursors (Delete this folder then copy the new one)
C:\Program Files (Arm) (Add Edge here)
C:\Windows\Web (Replace it)

[Delete]
C:\Windows\System32\Recovery
C:\Windows\System32\BingMaps.dll
C:\Windows\SysWoW64\OneDriveSetup.exe
C:\Windows\SysWoW64\BingMaps.dll
C:\Windows\SysArm32\BingMaps.dll
C:\Windows\WinSxS\arm64.x86_microsoft-windows-onedrive-setup_31bf3856ad364e35_10.0.20262.1_none_524224da765836ec (Delete this whole folder)
C:\Users\Default\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\OneDrive.lnk
C:\Program Files (x86)\Internet Explorer
C:\Program Files (Arm)\Internet Explorer
C:\Program Files (Arm)\Windows Defender
C:\Program Files (Arm)\Windows Mail
C:\Program Files\Internet Explorer
