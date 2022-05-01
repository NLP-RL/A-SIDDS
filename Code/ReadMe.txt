*** Association Guided Symptom Investigation and Diagnosis Dialogue System (A-SIDDS) ***


A. main file  : /src/dialogue_system/run/run.py

For DQN based dialogue agents :

	dqn_type = DQN

For DDQN based dialogue agents :

	dqn_type = DoubleDQN


B.For different varients of A-SIDDS

There are 6 different varients of dialogue manager in dialogue_manager (src/dialogue_system/dialogue_manager)

	1. A-SIDDS :    dialogue_manager_hrl (default)
	2. A-SIDDS_AM : dialogue_manager_hrl_A-SIDDS_AM.py
	3. A-SIDDS_RM : dialogue_manager_hr_A-SIDDS_RM.py
	4. PR-SIDDS :   dialogue_manager_hrl_PR-SIDDS.py
	5. PR-SIDDS_AM :dialogue_manager_hrl_PR-SIDDS_AM.py
	6. PR-SIDDS_RM : dialogue_manager_hrl_PR-SIDDS_RM.py

C.For Testing

	run_for_test.py

Please train before testing as there is not saved model weight (model/higher and lower policy network weight(including disease classifier weight) is 1.2 GB.
