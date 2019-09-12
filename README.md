# EhrBERT

EhrBERT is fine-tuned based on [BioBERT](https://github.com/dmis-lab/biobert) using 500K and 1M EHR notes. It is developed by the [UMASS BioNLP team](http://bio-nlp.org). Currently it's not available due to the risk of privacy leak. If you are interested in clinical version of BERT, we recommend using ClinicalBERT(https://github.com/EmilyAlsentzer/clinicalBERT) which was trained using public MIMIC data.

Prerequisite
-----
Please download [the huggingface implementation of BERT](https://github.com/huggingface/pytorch-pretrained-BERT).

Usage
-----
1. Download the EhrBERT and unzip it into <bert_directory>.

2. Install the environment that the huggingface needs. 

3. Taking classification as example, you just need to write one line to load the model.

```
model = BertForSequenceClassification.from_pretrained(<bert_directory>)
```

4. For more information, you can refer to these [examples](https://github.com/huggingface/pytorch-pretrained-BERT/tree/master/examples).
