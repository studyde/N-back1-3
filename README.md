Color-based N-back Task for Cognitive Workload Assessment
Overview
This repository contains a standardized Color N-back Task implemented in PsychoPy. The experiment is designed to measure working memory capacity and cognitive performance. By varying the "N" (1-back, 2-back, or 3-back), researchers can manipulate cognitive load to study human performance in various environments, such as smart lighting conditions or confined spaces.

Experimental Paradigm
Participants are presented with a continuous sequence of color stimuli. Their task is to determine if the current color matches the one presented N steps earlier in the sequence.

1-back: Low cognitive load (Match with the immediate previous stimulus).

2-back: Moderate cognitive load.

3-back: High cognitive load.

Visual Stimuli
The task utilizes seven distinct colors:

Red, Blue, Green, Cyan, Magenta, Yellow, and White.

Key Features
Multi-Level Difficulty: Includes ColourTesting_easy (1-back) and ColourTesting (up to 3-back).

Precise Timing: Leverages the PsychoPy backend for millisecond-accurate Reaction Time (RT) and Accuracy (ACC) logging.

Configurable Sequences: Trial orders are managed via external .csv or .xlsx files for easy modification without touching the code.

Cross-Platform: Runs on Windows, macOS, and Linux via PsychoPy.

File Structure
Plaintext
├── ColourTesting.psyexp        # Task Difficulty Increasing Experiment
├── ColourTesting_easy.psyexp   # Task Difficulty Reduction Experiment
├── ColourTesting_lastrun.py    # Generated Python script for execution
├── ColourTest1.xlsx            # Trial sequence for 1-back
├── ColourTest2.xlsx            # Trial sequence for 2-back
├── ColourTest3.xlsx            # Trial sequence for 3-back
└── data/                       # Directory where experimental results are saved
Getting Started
Prerequisites
PsychoPy: Version 2024.2.4 or later is recommended.

Download PsychoPy

How to Run
Clone this repository:

Bash
git clone https://github.com/YourUsername/Color-N-back-Task.git
Open ColourTesting.psyexp in the PsychoPy Builder.

Click the Run button (green arrow).

Enter participant details (ID, Age, Gender) in the dialogue box.

Press Space when the current color matches the N-back target.

Data Analysis
The experiment outputs .csv files in the data/ folder. Key variables for analysis include:

colourtest: The color stimulus presented.

corresp: The ground truth (whether a response was expected).

key_resp.keys: The key pressed by the participant.

key_resp.rt: Reaction time for the trial.

key_resp.corr: Correctness of the response (1 = Correct, 0 = Incorrect).

Citation
If you use this project in your academic work, please cite it as follows:
Optimizing lighting environments and task sequences in confined spaces: A multimodal data-driven framework for enhanced human performance and well-being
In this paper, we used this paradigm for the experiment, and you can increase or decrease the color highlights in Excel according to your needs.
