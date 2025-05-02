Name: Srinivas Therapati
700755602


GANs – Explanation and Architecture

Adversarial Process:
- Generator tries to create fake data to fool the Discriminator.
- Discriminator learns to detect fake vs real data.
- Both improve through competition.

Architecture:
- Generator takes noise → outputs fake image.
- Discriminator takes image → predicts real/fake.
- Loss functions drive improvement in both.


2. AI Harms – Allocational Harm Example

Example:  
An AI resume screener favors male applicants due to historical hiring bias.

Mitigation Strategies:
1. Rebalance training data (equal representation).
2. Regular audits using fairness tools like Aequitas or Fairlearn.



3.Basic GAN Implementation (MNIST)

Features:
- Defined Generator & Discriminator models.
- Trained for 100 epochs with alternate training loops.
- Saved generated digits at Epoch 0, 50, and 100.
- Logged losses and visualized training progress.

Deliverables:
-  Sample images (Epoch 0, 50, 100)
- Loss plot (Generator vs Discriminator over epochs)

---

4. Data Poisoning Simulation (Sentiment Classifier)

What Was Done:
- Trained a text classifier on a movie review dataset.
- Introduced poisoned samples (flipped sentiment for "UC Berkeley").
- Evaluated model before and after poisoning.

Observations:
- Accuracy dropped after poisoning.
- Confusion matrix showed more incorrect classifications involving poisoned examples.

Deliverables:
-  Accuracy and confusion matrix (before vs after)
-  Explanation of poisoning impact



5. Legal and Ethical Concerns of GenAI

Issue 1: Memorizing Private Data
- GPT-2 has memorized private info from training data.
- Risks: Privacy violations, legal non-compliance.

Issue 2: Generating Copyrighted Content
- AI models can replicate copyrighted works (e.g., Harry Potter).
- Risks: Copyright infringement, unfair to original creators.

Position:  
Yes, GenAI should be restricted from using sensitive or copyrighted data to ensure ethical use.

---

 6. Bias Metric: False Negative Rate Parity (via Aequitas)

What It Measures:  
FNR = % of actual positives wrongly classified as negatives.

Why It Matters:
- High FNR can mean unfair denial of opportunities (e.g., jobs, loans).

Failure Case:
- If one group has a higher FNR, it is unfairly impacted.

Tool Used:  
[Aequitas Bias Audit Tool](http://aequitas.dssg.io/)  
→ Use demo or upload model predictions for bias audit.


