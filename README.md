# Design and Construction of Examination Countdown Time Management System

Final-year project, B.Eng Electrical and Electronics Engineering, Abubakar Tafawa Balewa University, Bauchi.

A 192 × 32 pixel LED display that counts down three examinations at once and keeps correct time through power cuts. Each countdown is stored as an absolute end time and compared with a battery-backed DS1307 real-time clock.

Live page: https://philip561.github.io/exam-countdown-system/

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

## Publishing on GitHub Pages

1. Create a new public repository, for example `exam-countdown-system`.
2. Upload `index.html`, the `assets` folder and this README (drag the unzipped files into the repository page, then commit).
3. Open Settings, then Pages. Under Build and deployment, choose Deploy from a branch, pick `main` and `/ (root)`, and save.
4. After a minute or two the page is live at `https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`.

## Adding your links

Open `index.html` and find the `LINKS` block near the end:

```js
var LINKS = { report:"", code:"", video:"", article:"" };
```

- `report`: `"docs/Project_Report.pdf"` after you upload the PDF, or any full web address.
- `code`: `"firmware/"` or the full address of your firmware folder.
- `video`: the YouTube video ID only, the part after `v=` in the address.
- `article`: the address of your LinkedIn or other article.

Anything left empty stays hidden, so nothing looks unfinished while you prepare it.

## Link previews on social media

Near the top of `index.html`, change the `og:image` line to the full address of `assets/preview.png` on your published site. LinkedIn and others need the full address to show the preview picture.
