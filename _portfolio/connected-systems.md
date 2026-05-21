---
title: "Connected Systems"
excerpt: "<img src='/images/bss.png' width='300'>"
collection: portfolio
---

## BSS (Battery Swap Station) — DRIMAES

![BATTON BSS](/images/bss.png)

Battery Swap Station **[BATTON](https://drimaes.com/solution-bss/)** consists of four cradles communicating via **RS485** with a main **Linux system** that controls subsystems through an **MQTT server** and a **virtual MQ (Message Queue)**.

I was in charge of:
- **Cradle control via a private RS485 protocol.**
- **OTA firmware updates with AWS S3.**
- **Edge networking stations across districts.**
- **Internal MQ communication.**

## Leafeon — Personal IoT Project

An ESP32 FreeRTOS-based IoT indoor environment monitor that measures temperature, humidity, eCO2, eTVOC, particulate matter, and (less-accurately) altitude, then logs to a cloud server.

This was an end-to-end personal project. Leafeon includes the **ESP32 IoT device**, a **FastAPI server**, a **local OTA server**, an **AWS RDS** backend, and a simple dashboard.

![Leafeon system](/images/leaf_sys.png){: width="250" }

[GitHub: LeafeonIOTProject](https://github.com/wkdalswns0427/LeafeonIOTProject)

## EYE-Tuner — CatchVision Workstation

EYE-Tuner is a web-based personalized digital reading-comprehension tool.

Through eye tracking, it identifies the user's gaze speed and reading habits, displays text at a customized pace, monitors eye fatigue, and saves personalized screen settings.

![Workstation](/images/workstation.gif){: width="350" .align-center}

**Achievements**
1. **Minjun Chang**, Guiju Choi, Jungyoon Byun, Dongha Kim, "Eye Tuner: Media Literacy Program based on Pupil Tracking," C-2024-039138.
2. IHEI Show Off Festa 2, **Best Choice Award**, 2021, IHEI Yonsei.
3. [MEDICAL HACK 2021](https://www.all-con.co.kr/uni_contest/467239), **Excellence Prize**, 2021, Busan City.
4. Yonsei IHEI Workstation, **Impact Solution Award**, 2021, IHEI Yonsei.

[GitHub: Eye-Tuner](https://github.com/Eye-Tuner/Eye-Tuner)
