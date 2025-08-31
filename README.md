# Classifica-o-de-imagem-com-Deep-Learning
Projeto para classificar imagens de pelúcias em duas classes.  

Foram criados dois modelos de Deep Learning,  

um criado do zero e outro usando Transfer Learning com Fine Tuning, tendo como base o VGG16.  

Surpreendente mesmo o modelo criado do zero teve melhor acurácia, com 95%  

após 20 epócas  

Já o criado com Transfer Learning não convergiu bem e terminou 20 épocas  

com 74% de precisão.  

A explicação para isso foi que o modelo maior do Transfer Learning  

tinha uma complexidade desnecessária, uma vez que foi criado para classificar  

dezenas de classes com dezenas de imagens,  

de modo que meu pequeno dataset com duas classes rapidamente levava ao  

overfitting do modelo.  

Por conta disso, o modelo simples que foi criado do zero perfomou muito melhor,  

por ter mais compatibilidade com o pequeno dataset.  

Ferramentas:  

Torch, Keras, VGG16, Matplotlib, Numpy.  

Keywords:  

Machine Learning, Deep Lerning, Transfer Lerning, classificação de imagens, Data Science, Python.



