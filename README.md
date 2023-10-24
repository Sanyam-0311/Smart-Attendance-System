# Smart-Attendance-System
An automated attendance system which marks the attendance automatically using a unique smart ID card when scanned on a RFID scanner.
# RFID Card Scanner

Welcome to the RFID Card Scanner project! This project is designed to read RFID card UIDs using an RFID reader (MFRC522) and communicate them to a PC for data logging. It provides an easy way to track card IDs and timestamps.

## Introduction

This project uses an RFID reader (MFRC522) to scan RFID cards and retrieve their UID (Unique Identification). The UID is then sent to a connected PC via the serial interface, where it can be logged and processed.

## Components

- **MFRC522 RFID Reader**: To read the RFID cards.
- **Arduino (or compatible microcontroller)**: To interface with the RFID reader and communicate with the PC.
- **Serial Interface**: To send UID and timestamps to a PC.

## Setup

### Pin Configuration

- **SS_PIN**: 10
- **RST_PIN**: 9

### Software Requirements

- Arduino IDE with the MFRC522 library installed.

## Usage

1. Connect the RFID reader to the Arduino according to the specified pin configuration.
2. Upload the code to the Arduino using the Arduino IDE.
3. Open the Arduino Serial Monitor.
4. Scan an RFID card to read its UID.
5. The UID and the current date and time will be sent to the Serial Monitor.
6. The data can be logged and processed on your PC.

## Code Explanation

- The code initializes the RFID reader and serial communication.
- It continuously checks for new RFID cards and reads their UID when detected.
- The UID is sent to the PC via the serial interface.

## Data Format

The data sent to the PC is in CSV format and includes the date, time, and the RFID card's UID.

## Acknowledgments

- Special thanks to the creators of the MFRC522 library and Arduino for enabling RFID card scanning with ease.
