# ActiveOVR-LIC
The code for Agent as Student: Learning from Informative Cues for Active Open-Vocabulary Recognition (RAL2026)


## DC-AOVR dataset

Our proposed DC-AOVR dataset is placed in the dataset folder. We have constructed an active open-vocabulary recognition dataset containing 77 base categories and 56 novel categories. During the construction process, we ensured that there are no in-duplicate instances across the base and novel categories. A complete category list and the corresponding train/test split files are also included for full reproducibility. The overall dataset structure is organized as follows:

Category lists:
- DC_AOVR_all_classname.txt: contains both base and novel categories (133 categories)
- DC_AOVR_base_classname.txt: contains base categories (77 categories)
- DC_AOVR_novel_classname.txt: contains novel categories (56 categories)

Eposide data folders: DC_AOVR_train and DC_AOVR_test represent the training and testing datasets respectively. In each eposide file ({scene_name}/episodes.json.gz), it contains numerous episode data, each entry is composed of:
- episode_id: the id of the current episode
- scene_id: the id of the simulated scene
- start_position: the initial position of the agent
- start_rotation: the initial rotation of the agent
- target_category: the category name of the target object
- target_id: the id of the target object in the simulated scene
- target_center: the center of the 3D bounding box of the target object in the scene
