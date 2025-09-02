🚰 Filling Water Tank using Siemens S7-1500 PLC & TP700 HMI

📌 Project Overview  
This project demonstrates a **Filling Water Tank ** implemented using a Siemens **S7-1500 PLC (CPU 1515-2 PN)** and a **TP700 Comfort HMI panel**.  

The system simulates an automated filling operation where a tank is filled until a **High Level (HL)** sensor is reached and stopped until the **Low Level (LL)** sensor is triggered. The project showcases **Auto/Manual operation** and **real-time monitoring** on the HMI.  

---

🛠 Hardware Used  
- **PLC**: Siemens S7-1500 CPU 1515-2 PN  
- **HMI**: Siemens TP700 Comfort Panel  
- **Software**: TIA Portal (Step 7 + WinCC Comfort/Advanced)  

---

🔄 Tank Filling Logic  

The system follows a simple **two-point control sequence**:  

| Condition                 | Action                          |
|---------------------------|---------------------------------|
| Tank level < LL           | ✅ Open Fill Valve (start filling) |
| Tank level ≥ HL           | ❌ Close Fill Valve (stop filling) |
| Stop button pressed       | ❌ All outputs OFF (safe state)   |
| Manual mode               | Operator can open/close valves from HMI |

- **Auto Mode**: Tank fills automatically between LL and HL  

---

📊 Features  
- Automatic filling between LL and HL  
- Manual override mode from HMI  
- Start / Stop  pushbutton controls  
- Level trend visualization on HMI  
- Simulation support (PLCSIM + WinCC Runtime Advanced)  

---

🖥 HMI Design  
- **Overview Screen**: Tank graphic with live level and valve states  
- **Auto/Manual Screen**: Set LL, HL, and hysteresis values  
- **Manual Control Screen**: Direct jog buttons for valves/pump  
- **Trends**: Real-time plot of tank level %  

---

📂 Project Files  
- **PLC Program**: Written in LADL in TIA Portal  
- **HMI Screens**: Designed in WinCC Comfort  

---



🚀 How to Run  

  # Clone the repository
    git clone https://github.com/nrasel/Filling-Water-Tank-with-PLC-and-HMI.git
    cd Filling-Water-Tank-with-PLC-and-HMI

## 📷 Project View
![Traffic Light Interface](https://github.com/nrasel/Filling-Water-Tank-with-PLC-and-HMI/blob/5f79fab69f99fdd8663d53bed441ae2cabd0044e/Filling%20Water%20Tank.PNG)

