# 🎞️ Video-Analysis : Motion-Based hidden letter detection, audio extraction, and interlaced video simulation

This project implements a multi-phase pipeline to analyze video content by detecting hidden letters through motion filtering, extracting and denoising audio, and simulating interlaced video scanning with enhancement effects.

---

## 📽️ Project Phases

### **Phase 1: Hidden Letter Detection (Motion-Based)**
- Reads a video (`video_with_letters.mp4`)
- Converts frames to grayscale and applies frame differencing
- Filters out noisy frames with high motion
- Saves only meaningful binary motion masks revealing hidden content

📁 Output: `motion_frames/mask_###.png`  
🕵️ Hidden Message Revealed: **Hello From Colab**

---

### **Phase 2: Audio Extraction & Denoising**
- Extracts audio from a video (`video_with_audio.mp4`)
- Reduces background noise using the `noisereduce` library
- Saves both original and denoised audio files

🎧 Output:
- `audio_extracted.wav`
- `audio_denoised.wav`

---

### **Phase 3: Interlaced Video Simulation + Bonus Effects**
- Simulates **odd/even field interlacing** by manipulating scanlines
- Applies a **zoom effect** for emphasis on regions
- Creates a **flicker effect** by alternating interlaced frames
- Saves final video outputs and a comparison image

📹 Output:
- `video_odd_interlaced.mp4`
- `video_even_interlaced.mp4`
- `video_flicker_effect.mp4`
- `extreme_zoom_interlaced_frame_comparison.png`

---

## 🧰 Tech Stack
<p align="left">
  <a href="https://www.python.org/" target="_blank" rel="noreferrer">
    <img src="https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue&font=blue" alt="Python ">
  </a>
  <a href="https://opencv.org/" target="_blank" rel="noreferrer">
    <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=OpenCV" alt="OpenCV">
 </a>
  <a href="https://matplotlib.org/" target="_blank" rel="noreferrer">
    <img src="https://custom-icon-badges.demolab.com/badge/Matplotlib-71D291?style=for-the-badge&logo=Matplotlib"alt="Matplotlib">
  </a>
  <a href="https://numpy.org/" target="_blank" rel="noreferrer">
    <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy" alt="NumPy">
  </a>
  
<a href="https://pypi.org/project/noisereduce/" target="_blank" rel="noreferrer">
    <img src="https://img.shields.io/badge/NoiseReduce-2D8CFF?style=for-the-badge&logo=soundcloud&logoColor=white" alt="NoiseReduce">
  </a>
  <a href="https://pypi.org/project/SoundFile/" target="_blank" rel="noreferrer">
    <img src="https://img.shields.io/badge/SoundFile-F28D35?style=for-the-badge&logo=audiomack&logoColor=white" alt="SoundFile">
  </a>
  <a href="https://docs.python.org/3/library/shutil.html" target="_blank" rel="noreferrer">
    <img src="https://img.shields.io/badge/OS%20%26%20Shutil-888888?style=for-the-badge&logo=files&logoColor=white" alt="shutil and os">
  </a>
  
  <a href="https://colab.research.google.com/" target="_blank" rel="noreferrer">
    <img src="https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=google-colab&logoColor=white" alt="Google Colab">
  </a>
</p>


### 🐍 Python Libraries Used:

* `cv2` (OpenCV) – for video processing and image analysis
* `matplotlib` – for visualization
* `numpy` – for numerical operations
* `moviepy` – for audio extraction from video
* `noisereduce` – for audio denoising
* `soundfile` – for reading/writing audio files
* `shutil`, `os` – for file handling and zipping directories
* `google.colab` – for file uploads/downloads in Colab environment

