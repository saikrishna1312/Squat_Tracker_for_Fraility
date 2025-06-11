# Squat Tracker for Frailty Assessment

A real-time computer vision application that monitors squat performance using pose estimation to assess physical frailty. This tool tracks joint angles—specifically the knee and back—over time to determine squat quality and consistency, offering insights into posture, mobility, and muscular strength.

## 🚀 Features

- Real-time squat detection using webcam
- Calculates knee angle and back (normal) angle using Mediapipe landmarks
- Classifies squats as correct or incorrect based on posture and alignment
- Plots time-series data of joint angles
- Designed to assess physical frailty using visual movement patterns

## 🧠 How It Works

1. Extracts key landmarks (hip, knee, ankle, shoulder) using Mediapipe.
2. Calculates joint angles using inverse cosine of 3D vectors.
3. Detects stages of squat (standing, squatting, returning).
4. Flags poor form using thresholds for back angle and knee alignment.
5. Records time, joint angles, and transitions for plotting and analysis.

## 📦 Tools Used

- **Mediapipe** – Pose estimation
- **OpenCV** – Video capture and annotation
- **NumPy** – Vector operations and angle calculations
- **Matplotlib** – Graphical visualization of angles
- **Python** – Core programming language

## Output
- Knee Angle and Normal Angle over time (line plots)
- Count of correct vs. incorrect squats
- Real-time display with angle overlays

## Future Work
- Integrate heart rate and breathing sensors for physiological frailty markers
- Train ML models to classify frailty severity
- Add voice-based or visual feedback for real-time coaching
- Export results to PDF or cloud dashboard for healthcare use
