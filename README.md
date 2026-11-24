# GlamGaze

A real-time, client-side computer-vision web application that analyzes facial landmarks and skin undertones in the browser to recommend personalized makeup styles and overlays.

> **Status:** Active Development (v0.1)

## How It Works
1. **Live Video Capture:** Uses the browser `MediaDevices` (`getUserMedia`) API to capture webcam frames locally without sending video data to any external server.
2. **Facial Landmark Extraction:** Runs **MediaPipe Face Mesh** in JavaScript to extract 468 3D facial landmarks in real time.
3. **Geometric & Undertone Analysis:** Computes facial-proportion ratios to classify face/eye shapes and samples cheek/forehead pixel RGB values to estimate skin undertones.
4. **Canvas Rendering:** Renders diagnostic markers and makeup overlays directly onto an **HTML5 Canvas** layer.

## Tech Stack
* **Computer Vision:** MediaPipe Face Mesh
* **Frontend & Graphics:** HTML5, CSS3, Vanilla JavaScript, HTML5 Canvas
* **Media Capture:** WebRTC (`getUserMedia` API)

## Roadmap
- [x] Real-time webcam capture and 468-point facial landmark mesh rendering
- [x] Geometric face-shape ratio classification and RGB undertone estimation
- [ ] Expanded eyeliner/lip shade overlays and lighting-normalization calibration
