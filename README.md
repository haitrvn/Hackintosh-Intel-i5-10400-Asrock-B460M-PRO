
# Ngôn ngữ: [English][[Vietnames]](README_VN.md)
# Hackintosh-Intel-i5-10400-Asrock-B460M-PRO(OpenCore 0.9.0 - macOS Ventura 13.2.1)

# Info PC

- Main: Asrock B460M Pro **[Link](https://www.anphatpc.com.vn/mainboard-asrock-b460m-pro4.html)**
- CPU: Intel® Core™ i5-10400 **[Link](https://www.anphatpc.com.vn/cpu-intel-core-i5-10400-12m-cache-2.90-ghz-up-to-4.30-ghz-6c12t-socket-1200-comet-lake-s_id32925.html)**
- Ram: 16GB (2x6GB) **[Link](https://www.anphatpc.com.vn/ram-kingston-hyperx-fury-8gb-1x8gb-ddr4-bus-2666mhz-black.html)**
- SSD: Samsung 970 EVO plus 512 **[Link](https://memoryzone.com.vn/ssd-samsung-970-evo-plus-pcie-nvme-v-nand-m-2-2280-500gb-mz-v7s500bw)**
- Wifi card: Broadcom BCM94352Z **[Link](https://shopee.vn/Card-WiFi-DW1560-(BCM94352Z)-cho-laptop-c%C3%B3-ch%C3%A2n-m2-ngff-i.74031021.7255189037)**

    ![About this Mac](Images/Screen_SystemInformation.png)

# Guide Hackintosh + OpenCore
- **[Opencore](https://dortania.github.io/OpenCore-Desktop-Guide)**.
- **[Wifi](https://elitemacx86.com/threads/how-to-enable-intel-wifi-on-macos-clover-opencore.604/)**.
- **[Bluletooth](https://elitemacx86.com/threads/how-to-enable-broadcom-bluetooth-on-macos.607/)**.
- **[Slow boot time](https://github.com/dortania/bugtracker/issues/192)**.

# Works
- Continuity:
    - Handoff
    - iMessage
    - Air Drop
- DisplayPort Output (4k resolution / 75hz)
- Sleep
- Wake
- Audio (select internal speakers)
- Ethernet
- Bluetooth
- WiFi
- All USB ports (Full 3.0 + 2.0 + type C)
- Dual Boot (Windows + MacOS) (NOTE: Install MacOS in second partition - after EFI partition)
- About 40s to boot up(counting from boot entry)

# May Not Works
- HDMI Port - not yet patch

# Note
The file config.plist. Please change MLB, SystemSerialNumber, SystemUUID into your code

```
		<dict>
			<key>AdviseFeatures</key>
			<false/>
			<key>MLB</key>
			<string>XXXXXXXXXXXXXXXXX</string>
			<key>MaxBIOSVersion</key>
			<false/>
			<key>ProcessorType</key>
			<integer>0</integer>
			<key>ROM</key>
			<data>ESIzRFVm</data>
			<key>SpoofVendor</key>
			<true/>
			<key>SystemMemoryStatus</key>
			<string>Auto</string>
			<key>SystemProductName</key>
			<string>iMac20,1</string>
			<key>SystemSerialNumber</key>
			<string>XXXXXXXXXXXX</string>
			<key>SystemUUID</key>
			<string>XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX</string>
		</dict>
```

