# Classifica-o-de-imagem-com-Deep-Learning  
Projeto para classificar 128 imagens de pelúcias em duas classes, Patinho e Lilica.  
Foram criados dois modelos de Deep Learning,  
um criado do zero e outro usando Transfer Learning com Fine Tuning, tendo como base o VGG16.  

Surpreendente, durante o treinamento, o modelo criado do zero teve melhor acurácia ao longo  
do treinamento, uma curva de aprendizado mais rápida  
e estavel e uma validation loss menor em todas as épocas.  
Enquanto isso, o modelo de transferência estagnou a validation loss próximo de 40% e  
teve uma acurácia bem instável, variando drasticamente entre 60% e 100% em  
épocas consecutivas.  

No resultado do teste final, após 20 épocas, o modelo de Transfer Learning  
superou em acurácia o modelo "from scratch", 100% contra 95%, contudo,  
A perda desse modelo mais elaborado foi bem maior, 40% contra 25%, mostrando  
que provavelmente a rede mais complexa sofreu overfiting e que o resultado  
superior na acurácia é mais um fruto do dataset pequeno do que de um desempenho  
melhor.  
 
A explicação para isso foi que o modelo maior do Transfer Learning   
tinha uma complexidade desnecessária, uma vez que foi criado para classificar  
dezenas de classes e milhares de imagens,  
de modo que meu pequeno dataset com duas classes rapidamente levava ao  
overfitting do modelo.  
Por conta disso, o modelo simples que foi criado do zero perfomou muito melhor  
por ter mais compatibilidade com o pequeno dataset, demonstrando, pela curva de aprendizado e pelo validation loss,  
que realmente estava reconhecendo os padrões e não apenas decorando as respostas.  

Ferramentas:  
Torch, Keras, VGG16, Matplotlib, Numpy.  
Keywords:  
Machine Learning, Deep Lerning, Transfer Lerning, classificação de imagens, Data Science, Python.
