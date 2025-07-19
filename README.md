# Unified Transport Card Prototype

This prototype demonstrates a **unified smart card system** for public transport payments, aimed at integrating all modes of urban transit — including **Metro Rail**, **Public Buses (RTC)**, **MMTS Trains**, and **Toll Gates** — into a single, RFID-based payment solution.

Designed for **policy and infrastructure innovation**, this system encourages seamless, cashless travel experiences for citizens across socio-economic classes, fostering both convenience and financial awareness.

---

## Project Objective

To propose and demonstrate a **Unified Transport Smart Card System** that:

- Enables commuters to use a **single card across all transit systems**
- Encourages **upper-middle class** users to opt for **premium transit options** (e.g., metro rail) for comfort and speed
- Empowers **lower-middle class** users to **monitor and manage transit spending** across all modes
- Establishes the foundation for a **cashless, digital-first** public transport infrastructure

---

##  How the Prototype Works

###  Hardware Used

- Arduino UNO/Nano
- 4x4 Matrix Keypad
- UART-based RFID Reader (simulated via Serial Monitor)
- Serial Monitor (simulates RFID scan input)

###  Key Features

- **Multi-mode Transit Selection** via keypad:
  - `A` – Metro Rail
  - `B` – Public Bus (RTC)
  - `C` – MMTS Train
  - `D` – Toll Gate
- **RFID-based Identity Verification** (simulated)
- **Personalized Balances** per user
- **Fare Deduction** with insufficient balance check
- **Balance Display** after each transaction

---

## Demonstration Flow

1. User selects mode of transport by pressing a key on the keypad.
2. System displays the selected mode (e.g., "YOU ARE TRAVELLING IN METRO RAIL").
3. User is prompted to **tap the card** (enter a 12-character RFID UID via Serial Monitor).
4. System checks UID:
   - Displays user name
   - Deducts fare if balance is sufficient
   - Displays remaining balance
   - Alerts if balance is insufficient

---

##  Sample UIDs and Users

| UID             | User       | Initial Balance |
|----------------|------------|-----------------|
| 4B007012C5EC    | Dheeraj    | ₹500            |
| 4B00C99D5C43    | Harshitha  | ₹10             |

---

##  Fare Mapping

| Transit Mode      | Key | Fare (₹) |
|-------------------|-----|----------|
| Metro Rail        | A   | 30       |
| RTC Bus           | B   | 15       |
| MMTS Train        | C   | 10       |
| Toll Gate Entry   | D   | 50       |

---

##  Policy Impact & Societal Value

### For Upper-Middle Class Citizens:
- Encourages shift from road congestion and public buses to **premium metro services**
- **One card** for metro, train, and road travel — unified and easy
- Appeals to tech-savvy, convenience-focused commuters

### For Lower-Middle Class Citizens:
- Offers visibility into remaining travel budget
- Promotes **cautious and planned spending**
- Avoids cash dependency and fare confusion

### For Government & Transit Authorities:
- Facilitates **data-driven policy making**
- Enables **real-time fare analytics** and demand modeling
- Reduces fare evasion and fraud
- Lays the groundwork for **interoperable transit systems**

---

##  Future Enhancements

- Integration with actual RFID readers (e.g., MFRC522)
- Real-time balance sync with cloud or mobile app
- Support for recharge via UPI or NFC
- Touchscreen interface and ticket generation
- LCD/OLED display integration for kiosk-like setup
- Persistent user data with EEPROM or database

---

## License

This prototype is open-source and intended for research, academic, and policy demonstration purposes. Please credit the author when using or modifying the code.

---

##  Author

**Dheeraj Lagishetty**  
*Embedded Systems | IoT | Smart City Innovation*  
Reach out to me at lagishettydheeraj@gmail.com


