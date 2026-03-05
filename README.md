# Gender-Inclusive-Language-Generation LT-EDI-ACL
This paper presents our submissions to the LT-002
EDI @ ACL 2026 Shared Task on Gender-003
Inclusive Language Generation. The task fo-004
cuses on controlled text rewriting that reduces005
gender bias while keeping the original mean-006
ing and fluency intact. We participate in both007
subtasks and treat them independently, training008
separate instances of the instruction-tuned en-009
coder–decoder model google/flan-t5-base010
on the respective training data.011
For Subtask A (Gender-Inclusive012
Language Generation), we fine-tune013
google/flan-t5-base to rewrite gender-014
biased sentence into gender-neutral sentence015
using supervised sequence-to-sequence016
learning with instruction-style prompts. For017
the subtask A in English, our system obtains018
GA = 43.3750, GN = 49.0000, QR = 39.0000,019
and AVG = 43.7917.020
For Subtask B (Counterfactual Generation),021
we fine-tune google/flan-t5-base using bi-022
ased English statements paired with coun-023
terfactual responses as given in the dataset.024
This model reaches a score of PR: 88.7766,025
CCNC: 88.7766, QS: 70.3192290 and Average:026
82.6241.027
Overall, the experiments indicate that full fine-028
tuning of instruction-tuned transformers pro-029
vides an effective way to produce sentence030
in gender-neutral form and also producing031
counter-factual sentences for biased one, when032
each subtask is optimized on its own data.
