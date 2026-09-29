---
title: MeterLink Privacy Policy
---
# MeterLink Privacy Policy

**Last updated:** September 13, 2026

**Developer:** Onur İmeci

**Privacy contact:** onurimeci.dev@gmail.com

## 1. Scope and purpose

MeterLink is a field application for reading compatible IEC 62056-21 electricity meters through Bluetooth Classic or USB Serial optical probes. This policy describes how the application processes data on the device.

## 2. Data processed and stored on the device

During use, the application may process and store meter serial and installation information, IEC identification data, OBIS and load-profile values, reading metadata, saved optical-probe configuration, user-provided names and settings, optional exact RAW communication and TX/RX diagnostic records, and exports explicitly created by the user.

This data is stored locally in the Room database and Android-protected app-private files. Large RAW and log evidence is not stored as database BLOB data.

## 3. Automatic transfer and third parties

The current version does not use network communication and does not request the INTERNET permission. It contains no analytics, advertising, crash-reporting, or cloud-upload SDK. Meter and device data is not automatically sent to the developer or third parties.

When the user explicitly chooses **Share** or **Save As**, selected data is passed through Android's sharing or Storage Access Framework interface to a destination chosen by the user. That destination's own privacy policy applies.

## 4. Bluetooth, location, and USB access

- Bluetooth permissions are used to discover and connect to Bluetooth Classic probes.
- Android 12 and later request separate scan and connection permissions. Scanning is not used to infer physical location.
- Android 11 and earlier require Fine Location for Bluetooth discovery; MeterLink does not store location data.
- USB access uses Android's device-specific permission flow for the connected USB Serial probe.

## 5. Retention and deletion

RAW and diagnostic files may be cleaned according to the selected 7-day, 30-day, 90-day, or indefinite retention policy. Structured reading history remains until the user deletes the related reading or load profile. Deleting an optical-probe record does not automatically delete history.

Android removes local app data when the app is uninstalled, and Android backup is disabled. Files previously exported elsewhere are outside the app's control and must be deleted from their destination separately.

## 6. Security

Operational data is stored in app-private storage by default. Only temporary files under `cache/exports/` are shared for export, using time-limited read access through `content://` URIs. Cleartext network traffic is disabled. No electronic storage method can guarantee absolute security; users remain responsible for device screen-lock and physical-access protection.

## 7. Children

MeterLink is a professional operational tool and is not designed for children.

## 8. Policy changes and contact

This policy may be updated when app behavior or legal requirements change. The current date and text will be available in the app and on the public policy page linked from Google Play. Questions and data requests may be sent to onurimeci.dev@gmail.com. 
