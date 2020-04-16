# AMPERSAND-EMNLP2019
Code and Data for EMNLP 2019 paper titled  AMPERSAND: Argument Mining for PERSuAsive oNline Discussions
These models were fintuned using older version of hugging face and not transformers package . used pytorch-pretrained-bert=0.4.0

There are two steps of fine tuning involved here. To load finetuned models on distantly labeled data IMHO (intra relation / claim - premise ) classification and QR for inter relation classification 

load respective models in this line
https://github.com/tuhinjubcse/AMPERSAND-EMNLP2019/blob/master/argmining/examples/run_classifier.py#L498


For Argumentative Component Prediction and Relation Prediction:
Link to FineTuned Pytorch Model using IMHO+Context as Intermediate Pretraining over BERT:

https://drive.google.com/file/d/11U_kLNn6ngPltWQ1raN16SSy8tQ9fpL5/view?usp=sharing


Link to QR fine-tuned model
https://drive.google.com/file/d/1wWs_0pb2N9dmXz6RjnW7TiJkV-b1m9Np/view?usp=sharing



Link to IMHO+Context dataset: 
You can choose to keep the IMO/IMHO keywords. We removed them based on Chakrabarty et al (2019)
https://drive.google.com/file/d/1HGInaDp6nlAZUfqU5V1BM8j4su3DKKsc/view?usp=sharing

Link to QR dataset
https://drive.google.com/file/d/10l96wL1VQlApC1h0LPOjUpGAtyRZvMPO/view?usp=sharing


To reproduce our results in paper follow the details in AMPERSAND_Supplementary.pdf uploaded

Load fine-tuned models instead of pretrained BERT and use the data mentioned below to further fine-tune
https://github.com/chridey/change-my-view-modes


For RST :

Use https://www.aclweb.org/anthology/D18-1116.pdf for EDU segmentation
Use for getting RST parse trees https://github.com/jiyfeng/DPLP
Once you have parse trees you can get features from them




For Summarization

https://github.com/nlpyang/BertSum
https://drive.google.com/file/d/1iyPb_z775V7qVRD8_kGXCFxGuSoku3Hr/view?usp=sharing (doc-summary pairs)



If you use any of these , please cite us

@inproceedings{chakrabarty-etal-2019-ampersand,
    title = "{AMPERSAND}: Argument Mining for {PERS}u{A}sive o{N}line Discussions",
    author = "Chakrabarty, Tuhin  and
      Hidey, Christopher  and
      Muresan, Smaranda  and
      McKeown, Kathy  and
      Hwang, Alyssa",
    booktitle = "Proceedings of the 2019 Conference on Empirical Methods in Natural Language Processing and the 9th International Joint Conference on Natural Language Processing (EMNLP-IJCNLP)",
    month = nov,
    year = "2019",
    address = "Hong Kong, China",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/D19-1291",
    doi = "10.18653/v1/D19-1291",
    pages = "2933--2943",
    abstract = "Argumentation is a type of discourse where speakers try to persuade their audience about the reasonableness of a claim by presenting supportive arguments. Most work in argument mining has focused on modeling arguments in monologues. We propose a computational model for argument mining in online persuasive discussion forums that brings together the micro-level (argument as product) and macro-level (argument as process) models of argumentation. Fundamentally, this approach relies on identifying relations between components of arguments in a discussion thread. Our approach for relation prediction uses contextual information in terms of fine-tuning a pre-trained language model and leveraging discourse relations based on Rhetorical Structure Theory. We additionally propose a candidate selection method to automatically predict what parts of one{'}s argument will be targeted by other participants in the discussion. Our models obtain significant improvements compared to recent state-of-the-art approaches using pointer networks and a pre-trained language model.",
}






