  I have created a machine translation  model from scratch using base model encoder and decoder and t5 base model using Hugging face 
  
  
                                                            Machine Translation Using Encoder and Decoder
Machine translation is the process of using artificial intelligence to automatically translate text from one language to another without human involvement.


i have created a translation model which convert english language text to french text 
This notebook is an implementation of the article : https://blog.keras.io/a-ten-minute-introduction-to-sequence-to-sequence-learning-in-keras.html


In this project, Firstly i have uesd RNNs,LSTMs but the BLEU Score( Bilingual Evaluation Understudy) of model is decreases with increase in length of input data &suffer from long term dependecies to overcome from this problem there is another model which is design to handle  sequence to sequence prediction problem named encoder and decoder and model, model does not suffer from long term dependecies 

![BLEU Score](https://user-images.githubusercontent.com/102478403/193464482-3db5e993-2231-4ff8-808f-85c64bd70ba8.jpg)

i have created this project using encoder and decoder model & build it from scratch without using any specific library due to which the bleu score model is stable with increase in the length of text data


![BLEU score 1](https://user-images.githubusercontent.com/102478403/193464577-66e062f9-7c16-4088-bb74-a350fe8c59a0.png)


                                                                Encoder and decoder 
The encoder-decoder model is a way of using recurrent neural networks for sequence-to-sequence prediction problems.
The approach involves two recurrent neural networks, one to encode the input sequence, called the encoder, and a second to decode the encoded input sequence into the target sequence called the decoder.


![Encoder and decoder jpg](https://user-images.githubusercontent.com/102478403/193464509-66650403-e485-4b15-80ce-e11554230bb7.jpeg)



Here's the result of the model


![example](https://user-images.githubusercontent.com/102478403/193464545-96f8fcd6-7f13-4eb1-8680-6bd82b22e960.PNG)


                                        Machine translation using t5 base model 

Previously i have created a Language translation model using Encoder and Decoder model ,since encoder and decoder are base model and simple model and trained over small dataset due to which it cannot able to handle dynamic input

So, i have created another machine translation model using t5 base model which is pretrained model and able to handle dynamic inputs Thanks to Hugging Face library and hosted it using Gradio Library

![Screenshot (416)](https://user-images.githubusercontent.com/102478403/195020765-f4663210-8663-4028-915a-96cb283f18fe.png)

                                        
