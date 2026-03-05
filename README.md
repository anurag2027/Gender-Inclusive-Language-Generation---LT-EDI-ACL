# Gender-Inclusive-Language-Generation LT-EDI-ACL
This paper presents our submissions to the LT-
EDI @ ACL 2026 Shared Task on Gender-
Inclusive Language Generation. The task fo
cuses on controlled text rewriting that reduces
gender bias while keeping the original mean
ing and fluency intact. We participate in both
subtasks and treat them independently, training
separate instances of the instruction-tuned en
coder–decoder model google/flan-t5-base
on the respective training data
For Subtask A (Gender-Inclusive
Language Generation), we fine-tune
google/flan-t5-base to rewrite gender-
biased sentence into gender-neutral sentence
using supervised sequence-to-sequence
learning with instruction-style prompts. For
the subtask A in English, our system obtains
GA = 43.3750, GN = 49.0000, QR = 39.0000,
and AVG = 43.7917.
For Subtask B (Counterfactual Generation),
we fine-tune google/flan-t5-base using bi
ased English statements paired with coun
terfactual responses as given in the dataset.
This model reaches a score of PR: 88.7766,
CCNC: 88.7766, QS: 70.3192290 and Average:
82.6241.
Overall, the experiments indicate that full fine-
tuning of instruction-tuned transformers pro
vides an effective way to produce sentence
in gender-neutral form and also producing
counter-factual sentences for biased one, when
each subtask is optimized on its own data.
We ranked 8th in Subtask A for english and 2nd for subtask B.
