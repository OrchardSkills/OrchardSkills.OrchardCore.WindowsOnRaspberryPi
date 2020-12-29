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

Click on the Download 64-bit link from the stable versions

![WoR-014](https://user-images.githubusercontent.com/59172485/103230516-e8cd8280-48f2-11eb-808d-bb977b0293a0.png)

Make sure I accept the agreement is selected and press the Next button

![WoR-015](https://user-images.githubusercontent.com/59172485/103230517-e9661900-48f2-11eb-9ab0-0644a2069a76.png)

Click on the Next button

![WoR-016](https://user-images.githubusercontent.com/59172485/103230519-e9661900-48f2-11eb-827a-0224158c9be0.png)

Click on the Next Button

![WoR-017](https://user-images.githubusercontent.com/59172485/103230520-e9661900-48f2-11eb-8c99-22e9ba591a61.png)

Click on the Finish button

![WoR-018](https://user-images.githubusercontent.com/59172485/103230521-e9feaf80-48f2-11eb-865a-821571239955.png)

Select the Free (limited, non-commercial) Option and press the OK button.

Download 7-Zip From https://www.7-zip.org/download.html and install it.

![WoR-019](https://user-images.githubusercontent.com/59172485/103251312-ac6f4600-4935-11eb-97f6-fd4b779e6cd3.png)

Right click on the ISO file and select 7 Zip and then Open archive. This will open up the 7 Zip Application and list the files in the archive.

![WoR-020](https://user-images.githubusercontent.com/59172485/103251314-ad07dc80-4935-11eb-886a-2b45e625f425.png)

Create a new folder

![WoR-021](https://user-images.githubusercontent.com/59172485/103251315-ad07dc80-4935-11eb-96a8-919cb501cc66.png)

Name it WIN10-WIM

![WoR-022](https://user-images.githubusercontent.com/59172485/103251316-ada07300-4935-11eb-880c-f180a69836d5.png)

Select the Install.wim from the sources folder inside your windows 10 on arm iso file Windows10.iso > Sources > Install.wim and extract it in the new folder that was just created. Just drag and drop the file to the folder.

![WoR-023](https://user-images.githubusercontent.com/59172485/103251317-ada07300-4935-11eb-9693-91836ca0c5a5.png)

install.wim now extracted in the new folder

![WoR-024](https://user-images.githubusercontent.com/59172485/103251318-ada07300-4935-11eb-8018-ac96677ee609.png)

Launch the NTLite application and select Add Image file (WIM, ESD, SWM)

![WoR-025](https://user-images.githubusercontent.com/59172485/103251320-ae390980-4935-11eb-8585-1ada808a0c06.png)

Select the install.wim file that was extracted from the archive

![WoR-026](https://user-images.githubusercontent.com/59172485/103251321-ae390980-4935-11eb-88b2-03109c79e5ed.png)

Select OK to continue.

![WoR-027](https://user-images.githubusercontent.com/59172485/103251322-ae390980-4935-11eb-9580-c1d2a23cb8f6.png)

Select Load to load the file for editing

![WoR-028](https://user-images.githubusercontent.com/59172485/103251324-aed1a000-4935-11eb-930d-668f5de6bb9b.png)

Once the file is loaded a green led image will be displayed.

![WoR-029](https://user-images.githubusercontent.com/59172485/103251326-aed1a000-4935-11eb-85b2-e7c7551a9fa8.png)

![WoR-030](https://user-images.githubusercontent.com/59172485/103251328-aed1a000-4935-11eb-9272-132759506824.png)

![WoR-031](https://user-images.githubusercontent.com/59172485/103251329-aed1a000-4935-11eb-9d2a-e620569d69e4.png)

![WoR-032](https://user-images.githubusercontent.com/59172485/103251330-af6a3680-4935-11eb-98a0-d9ceecd6d4c4.png)

![WoR-033](https://user-images.githubusercontent.com/59172485/103251331-af6a3680-4935-11eb-956a-1203e11a9b3e.png)

![WoR-034](https://user-images.githubusercontent.com/59172485/103251332-af6a3680-4935-11eb-8e0f-cdce8233ebab.png)

![WoR-035](https://user-images.githubusercontent.com/59172485/103251333-b002cd00-4935-11eb-9da0-b0610543dfa6.png)

![WoR-036](https://user-images.githubusercontent.com/59172485/103251334-b002cd00-4935-11eb-99f8-cbccc3016346.png)

![WoR-037](https://user-images.githubusercontent.com/59172485/103251335-b002cd00-4935-11eb-9a67-27f47ccc89b2.png)

![WoR-038](https://user-images.githubusercontent.com/59172485/103251336-b002cd00-4935-11eb-9a48-63907ec899c9.png)

![WoR-039](https://user-images.githubusercontent.com/59172485/103251337-b09b6380-4935-11eb-9872-2a4a28386d8a.png)

![WoR-040](https://user-images.githubusercontent.com/59172485/103251339-b09b6380-4935-11eb-9d8f-005fcc49b4b8.png)

![WoR-041](https://user-images.githubusercontent.com/59172485/103251340-b09b6380-4935-11eb-8510-418a7de420af.png)

![WoR-042](https://user-images.githubusercontent.com/59172485/103251341-b133fa00-4935-11eb-9afb-c1ba4b3f2f0a.png)

![WoR-043](https://user-images.githubusercontent.com/59172485/103251343-b133fa00-4935-11eb-9d01-9690a8502d1e.png)

![WoR-044](https://user-images.githubusercontent.com/59172485/103251345-b133fa00-4935-11eb-9262-844078219d7b.png)

![WoR-045](https://user-images.githubusercontent.com/59172485/103251346-b1cc9080-4935-11eb-8dfb-c1fb979a17e3.png)

![WoR-046](https://user-images.githubusercontent.com/59172485/103251347-b1cc9080-4935-11eb-9708-032df247c53f.png)

![WoR-047](https://user-images.githubusercontent.com/59172485/103251348-b1cc9080-4935-11eb-9974-b00840af5fa1.png)

![WoR-048](https://user-images.githubusercontent.com/59172485/103251349-b2652700-4935-11eb-8038-4becf0a3a0b9.png)

![WoR-049](https://user-images.githubusercontent.com/59172485/103251350-b2652700-4935-11eb-9702-4009cbd0d4df.png)

![WoR-050](https://user-images.githubusercontent.com/59172485/103251351-b2652700-4935-11eb-9f44-c781774c17f0.png)

![WoR-051](https://user-images.githubusercontent.com/59172485/103251352-b2fdbd80-4935-11eb-8694-c91bb6bd9e3a.png)

![WoR-052](https://user-images.githubusercontent.com/59172485/103251353-b2fdbd80-4935-11eb-94a3-0a20db412437.png)

![WoR-053](https://user-images.githubusercontent.com/59172485/103251354-b2fdbd80-4935-11eb-9ad4-782ff39fb930.png)

![WoR-054](https://user-images.githubusercontent.com/59172485/103251356-b3965400-4935-11eb-9473-cd4e0394a421.png)

![WoR-055](https://user-images.githubusercontent.com/59172485/103251358-b3965400-4935-11eb-9a95-8073cf813aec.png)

![WoR-056](https://user-images.githubusercontent.com/59172485/103251360-b3965400-4935-11eb-811d-bb599adace85.png)

![WoR-057](https://user-images.githubusercontent.com/59172485/103251363-b42eea80-4935-11eb-88be-ee96984ac173.png)

![WoR-058](https://user-images.githubusercontent.com/59172485/103251364-b42eea80-4935-11eb-9b26-4cc96fe8bbbc.png)

![WoR-059](https://user-images.githubusercontent.com/59172485/103251365-b4c78100-4935-11eb-9de7-698b2184a9a9.png)

![WoR-060](https://user-images.githubusercontent.com/59172485/103251366-b4c78100-4935-11eb-9bf7-b168eff1a562.png)

![WoR-061](https://user-images.githubusercontent.com/59172485/103251367-b4c78100-4935-11eb-8cdf-00fe5f9bacb4.png)

![WoR-062](https://user-images.githubusercontent.com/59172485/103251368-b5601780-4935-11eb-827c-4aacb78eaeb2.png)

![WoR-063](https://user-images.githubusercontent.com/59172485/103251369-b5601780-4935-11eb-82fe-eea60989dcf3.png)

![WoR-064](https://user-images.githubusercontent.com/59172485/103251370-b5f8ae00-4935-11eb-8aed-d5f4571c5477.png)

![WoR-065](https://user-images.githubusercontent.com/59172485/103251372-b5f8ae00-4935-11eb-9468-712d05d7142b.png)

![WoR-066](https://user-images.githubusercontent.com/59172485/103251374-b6914480-4935-11eb-9ab1-0d9ea8707998.png)

![WoR-067](https://user-images.githubusercontent.com/59172485/103251375-b6914480-4935-11eb-9120-e776611a4e56.png)

![WoR-068](https://user-images.githubusercontent.com/59172485/103251376-b6914480-4935-11eb-896f-9319db796a28.png)

![WoR-069](https://user-images.githubusercontent.com/59172485/103251378-b729db00-4935-11eb-92d7-a097b6604ebb.png)

![WoR-070](https://user-images.githubusercontent.com/59172485/103251382-b729db00-4935-11eb-8962-86f131d8cfeb.png)

![WoR-071](https://user-images.githubusercontent.com/59172485/103251383-b7c27180-4935-11eb-9bf4-e4427b215445.png)

![WoR-072](https://user-images.githubusercontent.com/59172485/103251384-b7c27180-4935-11eb-89e6-dc7853fd901a.png)

![WoR-073](https://user-images.githubusercontent.com/59172485/103251385-b7c27180-4935-11eb-8c3a-bace92eb3d15.png)

![WoR-074](https://user-images.githubusercontent.com/59172485/103251386-b7c27180-4935-11eb-9b6d-252b1abef461.png)

![WoR-075](https://user-images.githubusercontent.com/59172485/103251387-b85b0800-4935-11eb-8a89-36aeef3cfadd.png)

![WoR-076](https://user-images.githubusercontent.com/59172485/103251388-b85b0800-4935-11eb-8f6c-104ee21c1019.png)

![WoR-077](https://user-images.githubusercontent.com/59172485/103251390-b85b0800-4935-11eb-84f5-3e4ed52519ed.png)

![WoR-078](https://user-images.githubusercontent.com/59172485/103251391-b85b0800-4935-11eb-8798-2be0aa8deffc.png)

![WoR-079](https://user-images.githubusercontent.com/59172485/103251392-b8f39e80-4935-11eb-85a3-7679a21a9518.png)

![WoR-080](https://user-images.githubusercontent.com/59172485/103251393-b8f39e80-4935-11eb-8caa-23a22f5b470e.png)

![WoR-081](https://user-images.githubusercontent.com/59172485/103251394-b8f39e80-4935-11eb-8146-f3b69efb65c7.png)

![WoR-082](https://user-images.githubusercontent.com/59172485/103251395-b98c3500-4935-11eb-8588-1c1597a84180.png)

![WoR-083](https://user-images.githubusercontent.com/59172485/103251397-b98c3500-4935-11eb-8cf6-49aaf279c28f.png)



Open NTlite Then Load Install.wim
In NTLite You should see a Presets Tab on the top left , Click on import then load 0.3.0.xml
On your Right you should see 0.3.0 , Double click it
Then on your Left click on Registry
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
