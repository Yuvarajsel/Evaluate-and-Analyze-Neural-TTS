# 🎙️ Neural TTS System Performance: Comprehensive Evaluation and Analysis

## 📝 Executive Summary
This project focuses on the detailed evaluation of high-performance **Neural Text-to-Speech (TTS)** systems. It analyzes key performance characteristics including **latency**, **Real-Time Factor (RTF)**, **expressivity control via SSML**, and subjective quality assessment using **Mean Opinion Score (MOS)**.

## 🚀 Key Objectives
1.  **Metric Measurement:** Benchmarking generation time and RTF for various speech scenarios.
2.  **Expressivity Analysis:** Evaluating the effectiveness of prosody control (speed, emphasis) using SSML.
3.  **Qualitative Assessment:** Comparing synthesized audio quality across different configurations.
4.  **Stress Testing:** Assessing system stability with high-volume text inputs.

## 🛠️ Technologies Used
- **Python** (Core Logic)
- **OpenAI API** (Neural TTS Engine)
- **Librosa & Soundfile** (Audio Analysis)
- **Pandas** (Data Management)
- **Matplotlib & Seaborn** (Visualization)
- **Jupyter Notebook** (Interactive Environment)

## 📁 Project Structure
- `Evaluate_and_Analyze_Neural_TTS.ipynb`: Main research and evaluation notebook.
- `input_text.txt`: Evaluation corpus used for testing.
- `reference_results.txt`: Baseline results for comparison.
- `*.wav`: Synthesized audio samples (Normal, Slow, Fast, Expressive).

## 📊 Metrics Explained
- **Latency:** The time taken to generate speech from text.
- **Real-Time Factor (RTF):** Generation Time / Audio Duration. (Lower is better, < 1.0 is real-time).
- **Inverse RTF:** Audio Duration / Generation Time. (Higher is better).
- **MOS (Mean Opinion Score):** Subjective quality rating (1-5).

## 📈 Sample Results
| Version | Audio Duration (s) | Generation Time (s) | RTF | MOS |
| :--- | :--- | :--- | :--- | :--- |
| Normal | 329.21 | 57.54 | 0.17 | 4 |
| Slow | 340.46 | 53.32 | 0.16 | 5 |
| Fast | 318.46 | 48.04 | 0.15 | 3 |
| Expressive | 330.96 | 58.44 | 0.18 | 4 |

## ⚙️ How to Run
1.  Clone the repository:
    ```bash
    git clone https://github.com/Yuvarajsel/Evaluate-and-Analyze-Neural-TTS.git
    ```
2.  Open `Evaluate_and_Analyze_Neural_TTS.ipynb` in Google Colab or a local Jupyter environment.
3.  Install dependencies:
    ```python
    !pip install openai soundfile librosa pandas matplotlib seaborn
    ```
4.  Set up your API keys in the notebook (Colab Secrets recommended).
5.  Run all cells to regenerate metrics and audio.

---
Built with ❤️ for Voice AI Research.
