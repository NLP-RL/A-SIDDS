## Association Guided Symptom Investigation and Diagnosis Dialogue System (A-SIDDS)

The repository contains code and dataset for research article titled 'Towards Symptom Assessment Guided Symptom Investigation and Disease Diagnosis' published at IEEE Transactions on Artificial Intelligence, 2023.

### Abstract
Automatic Disease Diagnosis (ADD) has gained immense popularity and demand over the past few years, and it is emerging as an effective diagnostic assistant to doctors. Diagnosis assistants assist clinicians in conducting a thorough symptom investigation and identifying possible diseases. Doctors correctly diagnose patients by observing only a few symptoms in most cases, even though the diagnosed disease has numerous symptoms. Also, some common symptoms, such as fever and headache, usually emerge due to other symptoms, which do not play a major role in identifying suffering diseases. In this work, we investigate the role of symptom importance in disease diagnosis through several feature engineering techniques and propose a novel symptom assessment incorporated symptom investigation and disease diagnosis (SA-SIDD) assistant using hierarchical reinforcement learning. The proposed SA-SIDD assistant first collects an adequate set of symptoms/sign information through conversing with users and then diagnoses a disease based on the extracted symptoms. We incorporated a symptom assessment module with the diagnosis framework that evaluates the relevance of current inspected symptom at each turn and reinforces the assistant to investigate distinctive and context-aligned symptoms using an assessment critic. The proposed methodology outperforms the state-of-the-art method, HRL, on two publicly available datasets, which firmly establishes the crucial role of symptom importance in disease diagnosis and the need for the proposed symptom assessment incorporated disease diagnosis framework. Furthermore, we have also conducted a human evaluation, revealing that the diagnosis method greatly enhances end-user satisfaction because of context-aligned relevant and minimal symptom investigation.

![Working](https://github.com/NLP-RL/A-SIDDS/blob/main/SASIDD.jpg)

#### Full Paper: https://www.computer.org/csdl/journal/ai/2023/06/10017134/1JU06Aq9Z2U

### Experiments

#### (a) main file  : /src/dialogue_system/run/run.py

For DQN based dialogue agents :

	dqn_type = DQN

For DDQN based dialogue agents :

	dqn_type = DoubleDQN


#### (b) For different varients of A-SIDDS

There are 6 different varients of dialogue manager in dialogue_manager (src/dialogue_system/dialogue_manager)

	1. A-SIDDS :    dialogue_manager_hrl (default)
	2. A-SIDDS_AM : dialogue_manager_hrl_A-SIDDS_AM.py
	3. A-SIDDS_RM : dialogue_manager_hr_A-SIDDS_RM.py
	4. PR-SIDDS :   dialogue_manager_hrl_PR-SIDDS.py
	5. PR-SIDDS_AM :dialogue_manager_hrl_PR-SIDDS_AM.py
	6. PR-SIDDS_RM : dialogue_manager_hrl_PR-SIDDS_RM.py

#### (c) For Testing

	run_for_test.py
 
## Citation Information 
If you find this code useful in your research, please consider citing:
~~~~
@article{tiwari2023towards,
  title={Towards Symptom Assessment Guided Symptom Investigation and Disease Diagnosis},
  author={Tiwari, Abhisek and Raj, Rishav and Saha, Sriparna and Bhattacharyya, Pushpak and Tiwari, Sarbajeet and Dhar, Minakshi},
  journal={IEEE Transactions on Artificial Intelligence},
  year={2023},
  publisher={IEEE}
}

Please contact us @ abhisektiwari2014@gmail.com for any questions, suggestions, or remarks.
