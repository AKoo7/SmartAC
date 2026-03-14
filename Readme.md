# H-Link-Docs

This repository documents my implementation of Lumixen's excellent ESPHome custom component: [lumixen/esphome-hlink-ac](https://github.com/lumixen/esphome-hlink-ac).

---

## Hardware

### Heat Pumpv- **Model Number:** RAS-I50E2

### Components

- **Salvaged Connector JST PA2.0 with broken tab - 6pin:**  
  

- **Logic Level Converter:**  
  [AliExpress Link](https://www.aliexpress.com/item/1005005984772131.html)

- **Buck Converter:**  
  [AliExpress Link](https://www.aliexpress.com/item/1005007031557776.html)

- **ESP32-C3:**  

---

## Instructions

### Step 1: Heat Pump Disassembly

1. **Power Off the Unit**  
   Turn off the heat pump at the main (master) switch. This is usually located near the outdoor unit. Ensure the green indicator light on the indoor unit is off.

2. **Remove Three Screws**  
   These screws are located along the bottom edge of the indoor unit. Plastic covers must be removed to access them.

   <img src="https://github.com/user-attachments/assets/fc4296af-6c1a-4fb5-a470-f3895c1baf4a" width="400"/>

3. **Release Six Clips**  
   Use a flathead screwdriver to release the four clips along the top, then two more under the filter cover.

   <img src="https://github.com/user-attachments/assets/e2d6db87-15da-46ed-9bfa-326974cd86db" width="400"/>  
   <img src="https://github.com/user-attachments/assets/04a918cd-8d9c-4bc8-bdd5-ced297b5f823" width="400"/>

4. **Remove Electronics Housing Cover**  
   Remove any tape if present and unscrew the three screws securing the electronics housing.

5. **Locate the H-Link Header**

   <img src="https://github.com/user-attachments/assets/ce5c5abe-a243-49ce-a749-ca0390d74fd2" width="400"/>

---

### Connector Modification

If using a PH2.0 connector, you will need to carefully file down both sides for it to fit.

---

### Determining Socket Orientation

Using a multimeter, identify the 12V and Ground pins. In my setup, the 12V pin was at the bottom:

<img src="https://github.com/user-attachments/assets/774b9f2d-0b40-4f59-9ab1-4998cb9af368" width="150"/>

---

### Wiring

Follow the reference wiring diagram. Use GPIO16 and GPIO17 for UART RX and TX respectively:

<img src="https://github.com/user-attachments/assets/f5737485-2d1a-44ac-94b3-189e04d45427" width="400"/>  
<img src="https://github.com/user-attachments/assets/4ce03b9a-939a-4480-a8fd-891162213673" width="400"/>

---

