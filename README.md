# AMPERSAND-EMNLP2019
Code and Data for EMNLP 2019 paper titled  AMPERSAND: Argument Mining for PERSuAsive oNline Discussions
These models were fintuned using older version of hugging face and not transformers package . used pytorch-pretrained-bert=0.4.0

There are two steps of fine tuning involved here. To load finetuned models on distantly labeled data IMHO (intra relation / claim - premise ) classification and QR for inter relation classification 

load respective models in this line
https://github.com/tuhinjubcse/AMPERSAND-EMNLP2019/blob/master/argmining/examples/run_classifier.py#L498


For Argumentative Component Prediction and Relation Prediction:
Link to FineTuned Pytorch Model using IMHO+Context as Intermediate Pretraining over BERT:
https://drive.google.com/file/d/16TmUPPl4xyvkOmqINkc4kHS54TOXPUZI/view?usp=sharing


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

        @article{chakrabarty2020ampersand,
        title={AMPERSAND: Argument Mining for PERSuAsive oNline Discussions},
        author={Chakrabarty, Tuhin and Hidey, Christopher and Muresan, Smaranda and Mckeown, Kathy and Hwang, Alyssa},
        journal={arXiv preprint arXiv:2004.14677},
        year={2020}
      }






