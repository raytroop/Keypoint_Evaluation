This code is updated by author to adapt to Python3. All the credit goes to [AI_Challenger_2017](https://challenger.ai/competition/keypoint/subject) and it's [repo](https://github.com/AIChallenger/AI_Challenger_2017)

---

# Human Skeleton System Keypoint Evaluation
Human Skeleton System Keypoint is a task of AI Challenger 全球AI挑战赛。This python script is used for calculating the final score (mAP) of the test result, based on your submited file and the reference file containing ground truth.
# usage
```bash
python keypoint_eval.py --submit SUBMIT_FILEPATH --ref REF_FILEPATH
```
A test case is provided, submited file is submit.json, reference file is ref.json, test it by:
```bash
python keypoint_eval.py --submit ./keypoint_predictions_example.json --ref ./keypoint_annotations_example.json
```
```bash
Complete reading annotation JSON file in 0.02 seconds.
Complete reading prediction JSON file in 0.02 seconds.
Complete evaluation in 0.44 seconds.
{'error': None,
 'score': 0.9967403114813471,
 'warning': ['d8eeddddcc042544a2570d4c452778b912726720 is not in the '
             'prediction JSON file.',
             '054d9ce9201beffc76e5ff2169d2af2f027002ca is not in the '
             'prediction JSON file.',
             'fa436c914fe4a8ec1ec5474af4d3820b84d17561 is not in the '
             'prediction JSON file.']}
Score:  0.99674031
```
The final score of the submited result, error message and warning message will be printed.
