📧 AI Based Spam Filter (Naive Bayes from Scratch)

A lightweight, transparent, and fully functional Spam Filter built entirely in Python without using external Machine Learning libraries (like scikit-learn). This project demonstrates the fundamental mathematics behind Natural Language Processing (NLP) and Bayes' Theorem.

📖 Overview

Topic: AI Spam Filter (Manual Implementation)

Subject: Fundamentals in AI and ML

Technique: Naive Bayes Classifier (Multinomial)

Input: Text Messages (SMS/Email)

Output: Classification (SPAM or NOT SPAM) with Confidence Score.

Unlike commercial "black-box" models, this project manually implements:

Tokenization: Breaking text into a "bag of words".

Probability Calculation: Using Bayes' Theorem.

Laplace Smoothing: Handling unknown words ($\alpha=1$).

Log-Likelihood: Preventing arithmetic underflow.

🚀 Features

Zero Dependencies: Runs on standard Python (math, re only).

Instant Training: Includes a hardcoded dataset for immediate demonstration.

Interactive Interface: CLI-based tool to test custom messages in real-time.

Educational Code: Heavily commented to explain the math behind every function.

🛠️ Installation & Usage

Prerequisites

Python 3.8 or higher.

How to Run

Clone the repository or download the files.

Navigate to the folder containing the script.

Run the following command:

python manual_spam_filter.py


The system will train instantly and prompt you for input.

Type a message (e.g., "Win a free cash prize") to see the result.

Type exit to close the program.

📂 Project Structure

├── manual_spam_filter.py      # Main source code (The Algorithm)
├── project_documentation.pdf  # Formal Project Report (B.Tech submission)
└── README.md                  # Project Overview (This file)


🧠 The Math Behind It

The core formula used to classify a message is Bayes' Theorem:

$$P(Spam | W) = \frac{P(W | Spam) \cdot P(Spam)}{P(W)}$$

To prevent the "Zero Frequency Problem" (where a new word crashes the probability to 0), we use Laplace Smoothing:

$$P(w|c) = \frac{\text{count}(w, c) + 1}{\text{count}(c) + |V| + 1}$$

📊 Sample Output

=== Custom Spam Filter (No External Libraries) ===
Training model from scratch (calculating probabilities)...
Learned 154 unique words.
System ready. Type a message to check.

Enter message: Urgent! Claim your lottery reward now
Result: SPAM (Score: -14.52)
------------------------------
Enter message: Hey, are we still meeting for lunch?
Result: NOT SPAM (Score: -12.30)
------------------------------


👤 Author Details

Submitted By:

Name: Rajdeep Kumar

Roll Number: 25BCY10190

Degree: B.Tech

Institution: VIT BHOPAL UNIVERSITY
