# Jarkom-Modul-4-IT08-2024

| Nama          | NRP          |
| ------------- | ------------ |
| Irfan Qobus Salim | 5027221058 |
| Aisha Ayya Ratiandari | 5027231056 |

## Pembagian Rute Subnet

| Nama Subnet           | Rute                                                         | Jumlah IP | Netmask |
|-----------------------|--------------------------------------------------------------|-----------|---------|
| A1                    | Hololive - Holo-EN                                           | 2         | /30     |
| A2                    | Holo-EN - Holo-Myth                                          | 2         | /30     |
| A3                    | Holo-Myth - Switch2 - Kiara_Calli--(193_HOST) - Gura_Ame_Ina--(309_HOST) | 503       | /23     |
| A4                    | Holo Myth - HoloPromise - Project-Hope - HoloCouncil         | 3         | /29     |
| A5                    | Project-Hope - Irys--(2_HOST)                                | 3         | /29     |
| A6                    | Holo-Council - Switch4 - Kronii_Mumei--(39_HOST) - Bae-Fauna--(22_HOST) | 62 | /26 |
| A7                    | Holo-EN - HoloAdvent                                         | 2         | /30     |
| A8                    | HoloAdvent - Switch5 - FuwaMoco--(5_HOST) - Shiori_Nerissa--(12_HOST) - Biboo--(10_HOST) | 28 | /27 |
| A9                    | Hololive - Holo-JP                                           | 2         | /30     |
| A10                   | Holo-JP - Switch1 - GEN:0 - DEV_IS                           | 3         | /29     |
| A11                   | DEV_IS - Re:GLOSS = Ririka_Raden--(3_HOST) - Ao--(3_HOST) - Hajime_Kanade--(7_HOST) | 14 | /28 |
| A12                   | GEN:0 - Switch3 - MiComet--(1501_HOST) - Sora_Robo_AZKi--(542_HOST) - GEN:1 | 2045 | /21 |
| A13                   | GEN:1 - GAMERS                                               | 2         | /30     |
| A14                   | GEN:1 - Member - FBK_Matsuri--(321_HOST) - Aki_Hachama--(148_HOST) | 470 | /23 |
| A15                   | GAMERS - Fubuki - Korone--(51_HOST) - Okayu--(32_HOST) - Mio--(36_HOST) | 120 | /25 |
| A16                   | Hololive - Holo-ID                                           | 2         | /30     |
| A17                   | Holo-ID - AREA15                                             | 2         | /30     |
| A18                   | AREA15 - Switch6 - Risu--(319_HOST) - Moona--(201_HOST) - lofi--(140_HOST) | 661 | /22 |
| A19                   | Holo-ID - holoro                                             | 2         | /30     |
| A20                   | holoro - Switch7 - Ollie--(20_HOST) - Anya--(3_HOST) - Reina--(10_HOST) | 34 | /26 |
| A21                   | Holo-ID - holoh3ro                                           | 2         | /30     |
| A22                   | holoh3ro - Switch8 - Zeta--(81_HOST) - Kaela--(71_HOST) - Kobo--(146_HOST) | 299 | /23 |
| **Total**             |                                                              | **4263**  | **/19** |

## CPT / VLSM
### Topologi
![test](https://github.com/user-attachments/assets/b5292789-9da2-4973-afc7-b1f8b5bdded5)

### Pembagian IP - VLSM
| Subnet | Network ID     | Netmask         | Broadcast      | Range IP                        |
| ------ | -------------- | --------------- | -------------- | ------------------------------- |
| A12    | 192.237.0.0    | 255.255.248.0   | 192.237.7.255  | 192.237.0.1 - 192.237.7.254     |
| A18    | 192.237.8.0    | 255.255.252.0   | 192.237.11.255 | 192.237.8.1 - 192.237.11.254    |
| A3     | 192.237.12.0   | 255.255.254.0   | 192.237.13.255 | 192.237.12.1 - 192.237.13.254   |
| A14    | 192.237.14.0   | 255.255.254.0   | 192.237.15.255 | 192.237.14.1 - 192.237.15.254   |
| A22    | 192.237.16.0   | 255.255.254.0   | 192.237.17.255 | 192.237.16.1 - 192.237.17.254   |
| A15    | 192.237.18.0   | 255.255.255.128 | 192.237.18.127 | 192.237.18.1 - 192.237.18.126   |
| A6     | 192.237.18.128 | 255.255.255.192 | 192.237.18.191 | 192.237.18.129 - 192.237.18.190 |
| A20    | 192.237.18.192 | 255.255.255.192 | 192.237.18.255 | 192.237.18.193 - 192.237.18.254 |
| A8     | 192.237.19.0   | 255.255.255.224 | 192.237.19.31  | 192.237.19.1 - 192.237.19.30    |
| A11    | 192.237.19.32  | 255.255.255.240 | 192.237.19.47  | 192.237.19.33 - 192.237.19.46   |
| A4     | 192.237.19.48  | 255.255.255.248 | 192.237.19.55  | 192.237.19.49 - 192.237.19.54   |
| A5     | 192.237.19.56  | 255.255.255.248 | 192.237.19.63  | 192.237.19.57 - 192.237.19.62   |
| A10    | 192.237.19.64  | 255.255.255.248 | 192.237.19.71  | 192.237.19.65 - 192.237.19.70   |
| A1     | 192.237.19.72  | 255.255.255.252 | 192.237.19.75  | 192.237.19.73 - 192.237.19.74   |
| A2     | 192.237.19.76  | 255.255.255.252 | 192.237.19.79  | 192.237.19.77 - 192.237.19.78   |
| A7     | 192.237.19.80  | 255.255.255.252 | 192.237.19.83  | 192.237.19.81 - 192.237.19.82   |
| A9     | 192.237.19.84  | 255.255.255.252 | 192.237.19.87  | 192.237.19.85 - 192.237.19.86   |
| A13    | 192.237.19.88  | 255.255.255.252 | 192.237.19.91  | 192.237.19.89 - 192.237.19.90   |
| A16    | 192.237.19.92  | 255.255.255.252 | 192.237.19.95  | 192.237.19.93 - 192.237.19.94   |
| A17    | 192.237.19.96  | 255.255.255.252 | 192.237.19.99  | 192.237.19.97 - 192.237.19.98   |
| A19    | 192.237.19.100 | 255.255.255.252 | 192.237.19.103 | 192.237.19.101 - 192.237.19.102 |
| A21    | 192.237.19.104 | 255.255.255.252 | 192.237.19.107 | 192.237.19.105 - 192.237.19.106 |

## GNS3 / CIDR
## TOPOLOGI
![Screenshot 2024-11-13 012515](https://github.com/user-attachments/assets/1994f60a-8f4c-4b6b-8949-5fde5c979a6c)

### Penggabungan
Pembagian 1
![gabung1](https://github.com/user-attachments/assets/17b0b1a3-01ba-45aa-87ab-49585d57c164)

Pembagian 2
![gabung2](https://github.com/user-attachments/assets/13851991-1201-49fd-938f-6add06cc09df)

Pembagian 3
![gabung3](https://github.com/user-attachments/assets/c0cda4e1-675f-4f40-a898-1df180a2f2c4)

Pembagian 4
![gabung4](https://github.com/user-attachments/assets/b670a59d-0cab-487e-a502-0f64423f99d9)

Pembagian 5
![gabung5](https://github.com/user-attachments/assets/84fd6591-350f-4ab3-a840-2d7ff740921a)

Pembagian 6
![gabung6](https://github.com/user-attachments/assets/674147fa-2a46-4526-a9c9-d6163e770dd6)

Pembagian 7
![gabung7](https://github.com/user-attachments/assets/954b693b-d721-4d99-8fbe-ce364bf5ed1a)

Pembagian 8
![gabung9](https://github.com/user-attachments/assets/6ba73f97-40b7-485b-8422-6d92907eecd7)

Pembagian 9
![gabung8](https://github.com/user-attachments/assets/ae97eaa2-f6f8-40ad-9a00-0fb9f54d84d2)

Pembagian 10
![gabung10](https://github.com/user-attachments/assets/32278479-76cc-41c5-9911-35368295b7ee)






