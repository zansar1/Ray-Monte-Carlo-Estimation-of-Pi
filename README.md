# Ray-Monte-Carlo-Estimation-of-π

This is a Python application that uses Ray, a distributed computing framework, to estimate the value of π using the Monte Carlo method.
Getting Started

To run this application, you will need to have Ray installed on your machine. You can install it using pip:

pip install ray

Usage

    Clone the repository to your local machine.
    Open a terminal and navigate to the directory containing the Python script.
    Run the following command: python ray_pi_estimation.py
    The estimated value of π will be displayed in the console.

Description

This script generates NUM_SAMPLING_TASKS parallel tasks, each of which generates NUM_SAMPLES_PER_TASK random points in the unit square and computes the fraction of them that lie inside the unit circle. The total number of generated samples is TOTAL_NUM_SAMPLES.

The progress of the computation is reported by an actor, which collects the number of samples completed by each task and computes the overall progress. The progress is displayed in the console every second, until the computation is complete.

Finally, the script computes the estimated value of π as 4 * (number of points inside the unit circle) / (total number of points).
Dependencies

This application requires Ray and Python 3.
License

This project is licensed under the MIT License - see the LICENSE file for details.
