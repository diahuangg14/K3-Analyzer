K3 LLM Analyzer
# Description
This module combines:
- Rule-based PPE analysis
- LLM-based scene understanding and safety reasoning

# Input
List of detected object classes from YOLO.

Example:
```python
["person", "helmet", "vest"]

# Output
Dictionary containing:

rule-based caption & risks
LLM-generated analysis

# Usage
from analyzer import k3_object_analyzer
result = k3_object_analyzer(detected_objects)

requirements.txt
openai>=1.0.0
