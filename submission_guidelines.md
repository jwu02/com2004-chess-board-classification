# COM2004/3004 - Submission Guidelines

## 1. Overview

Your assignment submission will consist of four or fives files that need to be uploaded to MOLE. These are

- `system.py` (mandatory)
- `model.noisy.json.gz` (mandatory)
- `model.clean.json.gz` (mandatory)
- `report.txt` (mandatory)
- `requirements.txt` (optional)

No other files will be accepted. Make sure that they are uploaded with the names exactly as they appear above. Please upload them individually - do not zip or tar them.  Blackboard automatically packages submissions when we download them.

Test your `system.py` before submission by running the `train.py` and `evaluate.py` code provided. 

The files listed above are detailed below.

## 2. The files to submit

### system.py

This file stores your python code. All the python code that you have written must be in this file. It must work correctly when called from the `train.py` and `evaluate.py` programs provided.

### model.noisy.json.gz and model.clean.json.gz 

These are the files that are generated when you call `train.py` in conjunction with your own `system.py`. As stated in the assignment instructions they must not exceed the size limit of 3 MB each. Make sure that you submit the correct versions. i.e., we recommended rerunning `train.py` and `evaluate.py` immediately prior to submissions. If you submit an out of date model file your results will be incorrect when we test your solution and you may lose marks.

### requirements.txt

If you have developed your system outside of CoCalc or if you have installed any modules using pip then we will need to know which modules and module versions you have used. The easiest way to tell us this is to include a requirements file. This is generated by typing 'pip freeze' in your Python environment and saving the output into a file called requirements.txt. (If you have tested your code in CoCalc then there is no need to include this file.)

### report.txt

Your report must be concisely written in an ascii text file called 'report.txt'. It must *strictly* follow the format below. Cut and paste the text below or download the template from Blackboard. Replace the text in square brackets with your answers. The word limits are strict.

Be careful when entering your performance scores. We will in any case be rerunning your code. If our scores do not match your scores it will typically be an indication that there is something wrong with your code. 

```markdown
# Chess assignment report

(Replace the square-bracketed text with your own text. *Leave everything else unchanged.* Note, the reports are parsed to check word limits, etc. Changing the format may cause the parsing to fail.)

## Feature Extraction (Max 200 Words)

[Describe and justify the design of your feature extraction. Note, feature extraction includes all the steps that you have taken to produce the 10-dimensional feature vector starting from the initial image of the page.]

## Classifier (Max 200 Words)

[Describe and justify the design of your classifier and any associated classifier training stage.]

## Full Board Classification (Max 200 Words)

[Describe and justify any *additional* steps that you have taken to exploit the additional information available in full board classification mode.]

## Performance

My percentage correctness scores (to 1 decimal place) for the development data are as follows.

Clean data:

- Square mode: [Insert percentage here, e.g. 98.1% - remove brackets]
- Board mode: [Insert percentage here, e.g. 98.0% - remove brackets]

Noisy data:

- Square mode: [Insert percentage here, e.g. 83.3% - remove brackets]
- Board mode: [Insert percentage here, e.g. 58.1% - remove brackets]

## Other information (Optional, Max 100 words)

[Optional: highlight any significant aspects of your system that are NOT covered in the sections above]
```