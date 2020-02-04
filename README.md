# AMPERSAND-EMNLP2019
Code and Data for EMNLP 2019 paper titled  AMPERSAND: Argument Mining for PERSuAsive oNline Discussions
These models were fintuned using older version of hugging face and not transformers package . used pytorch-pretrained-bert=0.4.0

For Argumentative Component Prediction and Relation Prediction:
Link to FineTuned Pytorch Model using IMHO+Context as Intermediate Pretraining over BERT:
To reproduce our results in paper follow the details in AMPERSAND_Supplementary.pdf uploaded

https://drive.google.com/file/d/11U_kLNn6ngPltWQ1raN16SSy8tQ9fpL5/view?usp=sharing


Link to IMHO+Context dataset: 
You can choose to keep the IMO/IMHO keywords. We removed them based on Chakrabarty et al (2019)
https://drive.google.com/file/d/1HGInaDp6nlAZUfqU5V1BM8j4su3DKKsc/view?usp=sharing

Link to QR dataset
https://drive.google.com/file/d/10l96wL1VQlApC1h0LPOjUpGAtyRZvMPO/view?usp=sharing

Link to QR fine-tuned model
https://drive.google.com/file/d/1wWs_0pb2N9dmXz6RjnW7TiJkV-b1m9Np/view?usp=sharing


Load fine-tuned models instead of pretrained BERT and use the data in
https://github.com/chridey/change-my-view-modes


For RST :

Use https://www.aclweb.org/anthology/D18-1116.pdf for EDU segmentation
Use for getting RST parse trees https://github.com/jiyfeng/DPLP
Once you have parse trees you can get features from them

For BERT 

use this code (Hugging face code used during time of publication)
https://drive.google.com/file/d/1nc0A4C7RTGnDpsDtP3UwddXoOIRT_06-/view?usp=sharing


For Summarization

https://github.com/nlpyang/BertSum
https://drive.google.com/file/d/1iyPb_z775V7qVRD8_kGXCFxGuSoku3Hr/view?usp=sharing (doc-summary pairs)









