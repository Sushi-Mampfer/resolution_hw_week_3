# The perfect alarm
A semi configurable alarm, you can set times from 1-15 hours. It's perfect, because it'll definitely make you wake up early.

<img width="1744" height="1076" alt="image" src="https://github.com/user-attachments/assets/578303ca-c0a7-4d8d-b41f-c51e439108e3" />

It works by using a 4060 that triggers a 4020 on it's final output, since the 4020 is triggered on the falling edge it continues perfectly. And the last 4 outputs of the 4020 are 1/2/4/8 hour(s) (although an hour is a bit less than 58 minutes, because I couldn't use exact values). The buzzers signal is grounded by 4 different switches which are grounded by the 1/2/4/8 hour(s) pins. This allows you to put in any number from 1 to 15 hours. The reset switch grounds the buzzers input and powers the RESET pin on the 4060 and 4020.

---
## Schematic

<img width="1280" height="525" alt="image" src="https://github.com/user-attachments/assets/016db169-4801-4b29-86d9-871a360ae4da" />


## PCB

<img width="972" height="648" alt="image" src="https://github.com/user-attachments/assets/7ac92632-513e-46bc-9f24-da7acdbad363" />
