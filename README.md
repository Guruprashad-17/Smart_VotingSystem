# Smart Voting System

**Smart Voting System** is an intelligent and secure voting solution that modernizes traditional election procedures through facial recognition, machine learning–based voter authentication, fraud detection, and automated vote counting—all running on Python.

---

##  Technology Stack

- **Python** – Core programming language  
- **OpenCV–Python** – Real-time facial recognition and image processing  
- **scikit-learn** – Machine learning for voter authentication and fraud detection  
- **pywin32** – Windows automation for seamless OS-level interactions  
- **Other Dependencies** – Listed in `requirements.txt`  

---

##  Features

- **Facial Authentication**: Validate voter identity using facial recognition to ensure security and authenticity.
- **Fraud Detection**: Use machine learning techniques to flag and prevent suspicious voting behavior.
- **Automated Voting**: Smoothly add faces, verify voters, record votes, and count results with minimal manual intervention.
- **User-Friendly Scripts**:
  - `add_faces.py`: Register voter images into the system.
  - `give_vote.py`: Authenticate and record casted votes.

---

##  Project Structure

```

├── README.md
├── requirements.txt           # Python dependencies
├── data/                      # Dataset directory for storing voter images, metadata, etc.
├── add\_faces.py               # Script to register faces into the system
├── give\_vote.py               # Script to manage the actual voting process
├── Votes.csv                  # Log file recording votes
└── background.png             # UI/background image (optional/enhancement)

````

---

##  Installation & Setup

1. **Clone the repository**  
   ```bash
   git clone https://github.com/Guruprashad-17/Smart_VotingSystem.git
   cd Smart_VotingSystem
````

2. **Install dependencies**
   
   ```bash
   pip install -r requirements.txt

3. **Prepare your dataset**

   * Create a folder (e.g., `data/`) and populate it with facial images for each voter.
   * Ensure proper naming conventions (e.g., `voterID_name.jpg`) for easy mapping.

4. **Add voter faces**
   Run:

   ```bash
   python add_faces.py
   ```

   to register voter images into your system.

5. **Cast a vote**
   Run:

   ```bash
   python give_vote.py
   ```

   The system will authenticate the voter, record their vote, and log it in `Votes.csv`.

---

## Usage Guide

* **Registering Voters**:
  Execute `add_faces.py`, which captures or processes voter images and prepares the model for authentication.

* **Voting Process**:
  Run `give_vote.py`—the system performs facial recognition, validates the voter, records the vote digitally, and updates `Votes.csv`.

* **Vote Management**:
  Review `Votes.csv` to analyze vote counts, detect patterns, or run further audits or visualizations as needed.

---

## Contribution

Contributions, enhancements, and improvements are welcome!

To contribute:

1. Fork the repository.
2. Create a feature branch (e.g., `feature/my-new-feature`).
3. Make and commit your changes.
4. Push to your fork and submit a pull request.

---

## Future Enhancements (Ideas)

* **Multi-Factor Authentication**: Combine face recognition with biometric, PIN, or OTP for added security.
* **Cross-Platform Compatibility**: Modify to support Linux and macOS (remove or replace `pywin32`).
* **Robust Model Training & Evaluation**: Implement model validation and accuracy reporting.
* **Secure Backend Storage**: Move from flat files to encrypted databases for better data integrity.
* **Web Dashboard**: Develop a UI for deployment, monitoring, and live vote visualization.
* **Logging & Auditing**: Add detailed audit trails, timestamps, and logs for transparency.


---
