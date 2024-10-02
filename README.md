# Symptoms are known by their companies: Towards Association guided Disease Diagnosis Assistant

The repository contains code and dataset for research article titled 'Symptoms are known by their companies: Towards Association guided Disease Diagnosis Assistant' published at BMC Bioinformatics (2022).

### Abstract
Over the last few years, dozens of healthcare surveys have shown a shortage of doctors and an alarming doctor-population ratio. With the motivation of assisting doctors and utilizing their time efficiently, automatic disease diagnosis using artificial intelligence is experiencing an ever-growing demand and popularity. Humans are known by the company they keep; similarly, symptoms also exhibit the association property, i.e., one symptom may strongly suggest another symptom’s existence/non-existence, and their association provides crucial information about the suffering condition. The work investigates the role of symptom association in symptom investigation and disease diagnosis process. We propose and build a virtual assistant called Association guided Symptom Investigation and Diagnosis Assistant (A-SIDA) using hierarchical reinforcement learning. The proposed A-SIDDA converses with patients and extracts signs and symptoms as per patients’ chief complaints and ongoing dialogue context. We infused association-based recommendations and critic into the assistant, which reinforces the assistant for conducting context-aware, symptom-association guided symptom investigation. Following the symptom investigation, the assistant diagnoses a disease based on the extracted signs and symptoms. The assistant then diagnoses a disease based on the extracted signs and symptoms. In addition to diagnosis accuracy, the relevance of inspected symptoms is critical to the usefulness of a diagnosis framework. We also propose a novel evaluation metric called Investigation Relevance Score (IReS), which measures the relevance of symptoms inspected during symptom investigation. The obtained improvements (Diagnosis success rate-5.36%, Dialogue length-1.16, Match rate-2.19%, Disease classifier-6.36%, IReS-0.3501, and Human score-0.66) over state-of-the-art methods firmly establish the crucial role of symptom association that gets uncovered by the virtual agent. Furthermore, we found that the association guided symptom investigation greatly increases human satisfaction, owing to its seamless topic (symptom) transition.

![Working](https://github.com/NLP-RL/A-SIDDS/blob/main/A-SIDD.jpg)

#### Full Paper: https://link.springer.com/article/10.1186/s12859-022-05032-y

### Experiments

#### (a) main file  : Code/src/dialogue_system/run/run.py

For DQN based dialogue agents :

	dqn_type = DQN

For DDQN based dialogue agents :

	dqn_type = DoubleDQN


#### (b) For different varients of A-SIDDS

There are 6 different varients of dialogue manager in dialogue_manager (Code/src/dialogue_system/dialogue_manager)

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
@article{tiwari2022symptoms,
  title={Symptoms are known by their companies: towards association guided disease diagnosis assistant},
  author={Tiwari, Abhisek and Saha, Tulika and Saha, Sriparna and Bhattacharyya, Pushpak and Begum, Shemim and Dhar, Minakshi and Tiwari, Sarbajeet},
  journal={BMC bioinformatics},
  volume={23},
  number={1},
  pages={556},
  year={2022},
  publisher={Springer}
}

Please contact us @ abhisektiwari2014@gmail.com for any questions, suggestions, or remarks.
