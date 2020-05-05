# NLA Project 
## English to Simple English Machine Translation - Text Simplification 


This is Implementation For the Course Project for NLA CS573  Spring 2020. 
English to Simple English - Machine translation 

Team: Karthikeyan and Suman 
Mentor : Prashant Kodali and Manish Shrivastava 

Data : https://cs.pomona.edu/~dkauchak/simplification/ 

Papers : 
1) Simple English Wikipedia: A New Text Simplification Task – William and Kauchak
https://cs.pomona.edu/~dkauchak/papers/kauchak11simple.short.pdf
2) Improving Text Simplification Language Modeling Using Unsimplified Text Data – David Kauchak - https://www.aclweb.org/anthology/P13-1151.pdf
3) Simple and Effective Text Simplification Using Semantic and Neural Methods – Elior et al – https://wwww.aclweb.org/anthology/P18-1016.pdf
4) Exploring Neural Text Simplification Models – Sergiu et al –
https://www.aclweb.org/anthology/P17-2014.pdf

Appraoch : 

Baseline SMT  : 
1) Create a word based Translation Probablity model 
2) Create a Language Model 
3) Combine Transaltion Probablity and Language model with H.M.M to Create a Functional SMT Model 
4) This model has Bleu Score of 0.1499

NMT Approach : 
1) Seq 2 Seq - Model Building Task Failed because of computational requirements. Unable to make the model converge to get a non giberrish results
2) Transformers Approach : Able to Build a Transformer model with ~12500 Sentence Pair sub data. 
We created two different runs of our transformer model with different number of epochs
  2.1) for First run with 20 Epochs - Model has Bleu Score of 0.2148
  2.2) for Second Run with 28 Epochs - Model has bleu Score of 0.2303
....
