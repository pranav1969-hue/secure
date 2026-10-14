# 🛡️ Secure Examination System (Python + Flask)

A fully functional web-based secure exam delivery system. This project demonstrates AES-256-GCM encryption, payload staging, and in-memory decryption for secure PDF delivery.

## Prerequisites
- Python 3.8+
- pip (Python package installer)

## Installation & Setup
1. **Extract the ZIP file** to a folder on your computer.
2. Open a terminal or command prompt in that folder.
3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

## Running the System
1. **Start the backend server:**
   ```bash
   python app.py
   ```
2. **Open your web browser** and navigate to:
   ```
   http://127.0.0.1:5000
   ```

## How to Test
1. **As the Examiner:** Go to the Examiner tab, select `sample_mock_exam.pdf` (or any PDF on your computer), and click **Encrypt & Stage PDF**.
2. **Copy the Key:** The system will generate a long AES-256 Hex key. Copy this code.
3. **As the Student:** Switch to the Student tab. Paste the key you copied.
4. **Unlock:** Click **Verify Key & Start Exam**. The system will decrypt the paper strictly in memory, display the PDF securely via a blob URL, and start the exam countdown timer.
