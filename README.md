# Airline-Drilldown-ALV-Report

This SAP ABAP project is a classical report that provides a drilldown ALV interface for airline data. It allows users to explore airline details, flight schedules, flight details, and individual flight bookings in an interactive and modular way.

## Features

- Modular programming using INCLUDE programs and subroutines.
- Custom selection screen for user inputs.
- Multi-level drilldown navigation through ALV grids.
- Usage of standard SAP tables like SCARR, SPFLI, SFLIGHT, and SBOOK.
- Clean separation of data declaration, screen logic, and processing logic.

## Project Structure

- `zairlince_clis_report` : Main report program.
- `ZAIRLINCE_CLIS_REPORT_TOP` : Data declarations and global structures.
- `ZAIRLINCE_CLIS_REPORT_SCR` : Selection screen logic.
- `ZAIRLINCE_CLIS_REPORT_F01` : Main processing and ALV display logic.

## How to Use

1. Upload all programs and includes in your SAP system.
2. Execute report `zairlince_clis_report`.
3. Enter selection criteria on the screen.
4. Navigate through airline data using drilldown ALV grids.

## Technologies

- SAP ABAP
- ALV Grid Control
- Modular programming with INCLUDEs
- Subroutines (PERFORM)
- Selection Screen Events


# Airline Drilldown ALV Report - SAP ABAP Project

This SAP ABAP classical report provides a **multi-level drilldown ALV interface** to display detailed airline data. The report starts by showing **Airline Master Details** and allows users to **drill down step-by-step** into **Flight Schedules**, then into **Flight Details**, and finally into **Passenger Bookings** — all using **interactive ALV Grids**.

---

##  Key Features

✅ **Multi-Level Drilldown Navigation**  
✅ **ALV Grid Display (CL_GUI_ALV_GRID)**  
✅ **Modular Code using INCLUDE Programs**  
✅ **Custom Selection Screen**  
✅ **Event-based Report Flow**  
✅ **Clean Subroutine (PERFORM) Structure**  
✅ **Standard SAP Tables (SCARR, SPFLI, SFLIGHT, SBOOK)**  

---

##  Technologies & Concepts Used

| Concept | Description |
|--------|-------------|
| `EVENTS` | Used `START-OF-SELECTION`, `END-OF-SELECTION` to manage report flow |
| `SELECTION-SCREEN` | Custom input screen for filtering data |
| `INCLUDE` Programs | Code split into logical units: TOP, SCR, F01 |
| `PERFORM` / Subroutines | For reusability and clarity of logic |
| `ALV Grid` | Interactive output using `CL_GUI_ALV_GRID` |
| `Modularisation` | Clean, maintainable architecture |
| `Function Modules` | (Optional) For handling special tasks if needed |

---

##  SAP Tables Used

- **SCARR** – Airline Master
- **SPFLI** – Flight Schedule
- **SFLIGHT** – Flight Details
- **SBOOK** – Flight Bookings (Passenger Details)

---

##  Project Structure

```text
zairlince_clis_report
├── INCLUDE ZAIRLINCE_CLIS_REPORT_TOP   → Data declarations (internal tables, types)
├── INCLUDE ZAIRLINCE_CLIS_REPORT_SCR   → Custom selection screen design
├── INCLUDE ZAIRLINCE_CLIS_REPORT_F01   → Business logic + ALV display + drilldown logic

## Navigation Flow:
1. Airline List (SCARR)
2. Flight Schedule (SPFLI)
3. Flight Details (SFLIGHT)
4. Passenger Bookings (SBOOK)

##  Prerequisites

- SAP NetWeaver system with demo flight data.
- SE38/SE80 to import the includes and program.


