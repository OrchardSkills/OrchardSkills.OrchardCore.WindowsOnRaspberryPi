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

Click on the download link on the right creatingISO_21277.1000_en-us_arm64_professional.cms

![WoR-002](https://user-images.githubusercontent.com/59172485/103178293-bc582e80-483e-11eb-8aa8-3914612f8a5e.png)

Click on Keep


Download NTlite From https://www.ntlite.com/download/
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
