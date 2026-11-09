# Hi, I'm Finn 👋

MSc Robotics & AI student at UCL, with a BEng in Mechanical Engineering from UEA. I like building things that move, and writing the software that makes them do something useful.

Based in London 🇬🇧

## 🏆 Featured project: Nudge (Agent Verse 2026)

**[Agentverse_26](https://github.com/finnmg2004-bit/Agentverse_26)**: a local-AI assistance dog for deaf, blind and deafblind people.

🥇 **Winner, Google DeepMind Gemini prize** (best use of AI / Google DeepMind)\
🥈 **2nd place, Robotics Track**\
*Agent Verse hackathon, 7–8 Nov 2026*

A Unitree Go2 quadruped in MuJoCo that **hears the house for its owner** (doorbell, knock, kettle, smoke alarm, and sounds it has no rule for), **finds them**, **nudges** them, tells them what happened through a vibrating handle, light bar, screen and voice, then **leads them by the handle** to the door, or out of the house in a fire. Everything runs **locally** on a laptop, with no cloud calls.

- 👂 **Hearing:** simulated stereo ears → YAMNet + spectral rules, with sound direction triangulated as the robot moves
- 👀 **Finding the owner:** YOLOv8n on the head RGB-D camera, a probability map over rooms, and the owner's voice
- 🧠 **Deciding:** local Gemma 4 (via Ollama) picks from a menu of legal actions built from live perception, behind hard-coded safety reflexes and a watchdog on every LLM call
- 🔁 **Adapting:** re-searches when the owner moves, re-plans around blocked doorways, tells a doorbell on the TV from the real front door, and learns rules and tasks from one spoken sentence (Whisper + Piper TTS)

**Measured results:** Gemma decisions in **0.19 s** median (93% correct on logged decisions) · **96%** of household sounds alerted over 1,000 random trials, **smoke alarm never missed**, **0%** false alerts from background noise · owner detected in **97–98%** of camera views · **8 cm** localisation error where odometry alone drifts up to 4 m

## 🔭 What I'm up to

- 🎓 Studying Robotics & AI (MSc) at UCL, with a focus on ROS 2, simulation, and robot learning
- 🛠️ Making things at the UCL Institute of Making

## 🧰 Tech & tools

**Languages:** C++ · Python · C# (.NET) · Arduino/C\
**Robotics:** ROS 2 · Gazebo · MuJoCo · SLAM & navigation · motor control\
**AI & perception:** Gemma / Ollama (local LLMs) · YOLO · YAMNet · Whisper\
**Dev environment:** Linux · Docker · pixi · Git · ZeroMQ\
**Hardware & making:** CAD · stepper motors · microcontrollers · 3D printing & prototyping

## 💼 Experience

- **Fluke** (Norwich), Summer 2026: developed an automated robotics system for a manufacturing line, covering motion control, sensing, and the software that ties them together

## 🌱 Currently learning

- Deepening my C++ (LeetCode practice) and Python for robotics
- Robot learning and VLA models
- SLAM and navigation on real hardware

## 📫 Get in touch

- LinkedIn: [finn-m-gorman](https://www.linkedin.com/in/finn-m-gorman)
- Email: [finnmg2004@gmail.com](mailto:finnmg2004@gmail.com)
