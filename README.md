
# 3dCyberFiction-Clone

A portfolio / interactive demo clone featuring a 3D-style rotating character animation.  
Based on a sequence of image frames (`male0001.png…`) to create a cinematic / cyberfiction-style effect.

---

## 🧰 Features

- Uses a flipbook/image-sequence animation (multiple PNG frames) rather than a full 3D model.  
- Scroll (or other input) can be used to control the animation / frame index.  
- Lightweight dependency usage (just JS / HTML / CSS) for smoother load times.  
- Dark / high-contrast / futuristic UI vibe.

---

## 📁 File Structure

```

/
├── index.html           ← Entry point, contains canvas tag etc.
├── male0001.png         ← Image frames for animation
├── male0002.png
├── …
├── male0098.png
└── aaaaaaaaaaaa.png     ← Example additional image (maybe placeholder / test)

````

---

## 🚀 How to Run Locally

1. Clone this repo:

   ```bash
   git clone https://github.com/pranavv00/3dCyberFiction-clone.git
   cd 3dCyberFiction-clone
````

2. Serve the files (you can use a simple local server). For example, with Python:

   ```bash
   # Python 3.x
   python -m http.server 8000
   ```

   Or using VS Code Live Server / any web-server of your choice.

3. Open `http://localhost:8000/index.html` in your browser.

---

## ⚙️ How It Works

* A `<canvas>` is used to display frames sequentially.
* JavaScript loads the image frames into memory.
* User scroll (or another interactive control) maps to which frame is shown.
* On each “frame render,” the correct `maleXXXX.png` file is drawn to canvas to simulate rotation / animation.

---

## 🛠️ To Customize

* Replace the image frames with your own sequence (must be named in a predictable pattern, like `male0001.png`, `male0002.png` ...).
* Update the JS code to match the number of frames in your sequence.
* You can adjust canvas size, scale, positioning in CSS / JS.
* Add easing / smoother transitions if needed (e.g., between frames).

---

## ✅ Known Limitations

* Large number of image frames → potential heavy memory usage / load time.
* No free-form 3D rotation (only what the frames allow).
* Not interactive in the sense of real 3D (lighting, shading cannot change dynamically).

---

## 📜 License & Attribution

[MIT License](LICENSE) — feel free to use / modify / share.

Original image sequence credits: *\[your name / source if any]*.

---

