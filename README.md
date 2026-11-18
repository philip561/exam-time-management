# Design and Construction of Examination Countdown Time Management System

Final-year project, B.Eng Electrical and Electronics Engineering, Abubakar Tafawa Balewa University, Bauchi.

A 192 × 32 pixel LED display that counts down three examinations at once and keeps correct time through power cuts. Each countdown is stored as an absolute end time and compared with a battery-backed DS1307 real-time clock.

Live page: https://philip561.github.io/exam-time-management/

## Suggested repository layout

```
index.html          the project page
assets/             photos, diagram and the invigilator guide (PNG and PDF) used by the page
firmware/
  master/           master ATmega328P sketch (keypad, RTC, buzzer, top row)
  slave/            slave ATmega328P sketch (bottom row)
docs/
  Project_Report.pdf
media/              extra photos and videos (large videos are better on YouTube)
README.md
```
