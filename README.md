# Capstone project: Towards more robust definition and detection of system prompt leaks
## Abstract: 
The rapid adoption of large language models (LLMs) in various applications has introduced several
challenges in safeguarding against adversarial attacks. One critical threat is system prompt leakage,
where an attacker manipulates the model to reveal its internal instructions. Such leaks can lead to
privacy violations, unauthorized access, and exploitation of proprietary logic. Recent literature on
system prompt leakage focuses on the generation of system prompt attacks but overlooks detection
methods and the diverse ways in which leaks can happen. This paper works with this gap. First, this
paper defines prompt exfiltration, distinguishing between "hard" and "soft" forms. Second, it creates
a dataset of diverse exfiltration variants of system prompts and suggests a set of 4 heuristics (Rouge-L
score, Levenshtein distance, Jaccard similarity, and cosine similarity) to be used for prompt leak
detection. Finally, these heuristics are used as features to train a decision tree classifier that could be
used as an output filter for prompt leaks in practice. The findings emphasize the limitations of simple
substring matching for leak detection. Additionally, the paper examines LLMs’ decoding abilities in
cases where prompt leaks are obfuscated using encoding algorithms
