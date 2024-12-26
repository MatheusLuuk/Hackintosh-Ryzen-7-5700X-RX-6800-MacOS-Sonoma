# Hackintosh: Ryzen 7 5700X + RX 6800 (MacOS Sonoma)

Para fins de backup de arquivos do meu primeiro hackintosh 100%!!!

# Prints
![image](https://github.com/user-attachments/assets/bca25755-0efb-4585-b997-1e9555bfa4ff)
![image](https://github.com/user-attachments/assets/164934fc-f9d5-4df6-a535-5adada3c104f)


**MacOS version:** Sonoma 14.7.2 \
**OpenCore version:** 1.0.3

# Especificações
| Componente  | Modelo |
| ------------- | ------------- |
| Placa Mãe  | ASUS TUF Gaming X570-PLUS  |
| CPU  | AMD Ryzen 7 5700x  |
| GPU | ASUS TUF Radeon RX 6800 16GB GDDR6 |
| RAM | 32GB Asgard Feryr 3200MHz C18 (2x16GB)
| WAN | - |
| LAN CHIPSET	| Realtek® L8200A Gigabit LAN |
| AUDIO CHIPSET	| Realtek® ALC S1200A |
| Amazenamento MacOS | SSD SATA Ceamere 512Gb |
| Amazenamento Windows | 1TB NVME Asgard PCIe3.0 X4 3300/3000Mbps (r/w) |
| CPU Cooler | Water Cooler SuperFrame ISENGARD 360mm SF-W360 |
| Fonte | XPG Core Reactor 850W, 80 Plus Gold Modular |
| Gabinete | Lian Li O11 Dynimic |
| Refrigeração | Kit de Fans 3x3 Aigo 12 PRO |

# O que está funcionando
* Todos os MacOS desde Big Sur até Sequoia
* Áudio: painel frontal, painel traseiro incluindo Optic Digital Out + receptores e alto-falantes
* Todas as portas USB
* Monitoramento de temperatura para tudo, incluindo GPU
* Tudo, desde iCloud e telefones, pads e gadgets da Apple
* Sleep/wake up

# O que não está funcionando
* Microfone e entrada de linha no painel traseiro (problema conhecido da AMD)
* Wifi, Bluetooth, Airdrop, Airplay, Sidecar (Ainda não instalei a placa Wi-Fi/Bluetooth)

# ACPI Usadas
* SSDT-EC.aml
* SSDT-GPRW.aml
* SSDT-HPET.aml
* SSDT-PLUG.aml
* SSDT-SBUS.aml
* SSDT-USBW.aml
* SSDT-USBX.aml

# Kexts Usadas
* AMDRyzenCPUPowerManagement.kext
* AppleALC.kext
* AppleMCEReporterDisabler.kext
* FeatureUnlock.kext
* Lilu.kext
* NVMeFix.kext
* RealtekRTL8111.kext
* RestrictEvents.kext
* SMCAMDProcessor.kext
* SMCRadeonSensor.kext
* USBMap.kext
* USBWakeFixup.kext
* VirtualSMC.kext
* WhateverGreen.kext

# Configurações de BIOS
**Desabilitado**
* Fast Boot
* Secure Boot
* Serial/COM Port
* Compatibility Support Module (CSM) \

**Habilitado**
* Above 4G decoding
* Resizable BAR definida como "Auto", O config.plist já tem uma configuração para manter esta opção habilitada para garantir o melhor desempenho gráfico no Windows
* EHCI/XHCI Hand-off
* OS type: Other Types, com o Windows 8.1/10 UEFI Mode habilitado ele dá erro de segurança e não dá boot
* SATA Mode: AHCI

# Resultado do Geekbench
GPU \
![image](https://github.com/user-attachments/assets/2e1c91a1-5bef-46fd-adb0-480b94e707b4)

CPU \
![image](https://github.com/user-attachments/assets/53aa92bc-d3bc-4abb-9f6d-f5cd2caa04aa)

# Créditos
* Agradecimento para o [Gabriel Luchina](https://github.com/CCSilvs/EFI-ASUS-TUF-GAMING-X570-PLUS-BR?tab=readme-ov-file#specs:~:text=Special%20thnx%20to-,Gabriel%20Luchina,-His%20knowledge%20and)
* Seu conhecimento e repositório [BASE-EFI-AMD-RYZEN-THREADRIPPER](https://github.com/CCSilvs/EFI-ASUS-TUF-GAMING-X570-PLUS-BR?tab=readme-ov-file#specs:~:text=BASE%2DEFI%2DAMD%2DRYZEN%2DTHREADRIPPER)
* Hackintosh Profissional - ed. 2024/2025 Por Gabriel Luchina
* [Opencore Team](https://github.com/CCSilvs/EFI-ASUS-TUF-GAMING-X570-PLUS-BR?tab=readme-ov-file#specs:~:text=AMD%2DRYZEN%2DTHREADRIPPER-,Opencore%20Team,-About)
