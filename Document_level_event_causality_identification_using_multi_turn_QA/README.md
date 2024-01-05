# Event Causality Identification

## Setup
1. Put `EventStoryLine`, `CausalTM`, `EventCausalityData`, `SemEval`, and `FrameNet` datasets in the current directory.

2. Run `read_document.py` to build all intra-sentence examples for `EventStoryLine`.

3. Run `preprecess_*.py` to generate BERT-based examples for difference datasets and settings.

4. Run `train_mix.py` to train the model, with different settings.

## Datasets
- RAMS (Download at [https://nlp.jhu.edu/rams/])
- ACE05 (Access from LDC[https://catalog.ldc.upenn.edu/LDC2006T06] and preprocessing following OneIE[http://blender.cs.illinois.edu/software/oneie/])
- WikiEvents (Available here [s3://gen-arg-data/wikievents/])

You can download the data through the AWS CLI or AWS console. 
Alternatively, you can download individual files by 
- `wget https://gen-arg-data.s3.us-east-2.amazonaws.com/wikievents/data/<split>.jsonl` for split={train, dev,test}.
- `wget https://gen-arg-data.s3.us-east-2.amazonaws.com/wikievents/data/coref/<split>.jsonlines` for split={train, dev, test}.
  
Additional processed test files for RAMS can be downloaded by
- `wget https://gen-arg-data.s3.us-east-2.amazonaws.com/RAMS/test_head_coref.jsonlines`
- `wget https://gen-arg-data.s3.us-east-2.amazonaws.com/RAMS/test_head.jsonlines`