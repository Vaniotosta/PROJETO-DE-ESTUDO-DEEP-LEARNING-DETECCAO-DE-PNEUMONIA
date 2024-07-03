# PROJETO-DE-ESTUDO-DEEP-LEARNING-DETECCAO-DE-PNEUMONIA
**Introdução ao Problema de Negócio de Detecção de Pneumonia**
A pneumonia é uma infecção respiratória aguda que afeta os pulmões, sendo uma das principais causas de morbidade e mortalidade em todo o mundo. Segundo a Organização Mundial da Saúde (OMS).

A detecção precoce da pneumonia é crucial para garantir um tratamento eficaz e reduzir o risco de complicações. No entanto, o diagnóstico clínico da pneumonia pode ser desafiador devido à sua semelhança com outras doenças respiratórias e à variabilidade nos sintomas apresentados pelos pacientes. Tradicionalmente, o diagnóstico é feito com base em sintomas clínicos, exames físicos e radiografias de tórax. No entanto, a interpretação das radiografias pode ser subjetiva e dependente da experiência do radiologista, levando a diagnósticos inconsistentes.

Importância da Detecção Automatizada de Pneumonia Com os avanços em inteligência artificial (IA) e aprendizado de máquina, há uma oportunidade significativa para melhorar a precisão e a rapidez do diagnóstico de pneumonia. A utilização de algoritmos de aprendizado profundo (deep learning) para a análise de imagens de radiografias de tórax pode proporcionar uma ferramenta poderosa para os profissionais de saúde. Esses algoritmos têm o potencial de:

Aumentar a Precisão Diagnóstica: Reduzir a variabilidade e subjetividade na interpretação de radiografias, proporcionando uma segunda opinião consistente e baseada em dados. Melhorar a Eficiência Clínica: Acelerar o processo de diagnóstico, permitindo que os médicos tomem decisões mais rápidas e iniciem o tratamento mais cedo. Acessibilidade: Levar diagnósticos precisos para regiões com escassez de radiologistas experientes, melhorando o acesso ao cuidado de saúde de qualidade em áreas remotas e subatendidas.

## Justificativa

Por isso se justifica esse, quanto ao conjunto de dados "Chest X-Ray Images (Pneumonia)", você pode encontrá-lo no Kaggle através do seguinte link: https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia

A URL acima levará você diretamente ao conjunto de dados. O nome do conjunto de dados é "Chest X-Ray Images (Pneumonia)" e foi criado por Paul Mooney.

Foi usado duas modelagens usando o algorítmos VGG16 com estratégias diferentes para melhor acuracidade 

## INSIGHTS DO MODELO 2
-Desempenho Geral:

- Acurácia Geral: O modelo possui uma acurácia de 59%, indicando que o modelo acerta ligeiramente mais da metade das previsões.
Desempenho por Classe:

Classe Normal:

- Precisão: 0.36
- Recall: 0.13
- F1-Score: 0.19

**Análise:**

Das 234 imagens normais, o modelo acertou 31 e errou 203.

A precisão de 0.36 indica que 36% das previsões de "Normal" são corretas.

O recall de 0.13 mostra que o modelo identifica corretamente apenas 13% das imagens que são realmente normais.

O modelo tem dificuldade em identificar corretamente as imagens normais, resultando em uma precisão e recall bastante baixos para esta classe.


Classe Pneumonia:

- Precisão: 0.62
- Recall: 0.86
- F1-Score: 0.72

**Análise:**

Dos 390 casos de pneumonia, o modelo acertou 336 e errou 54.

A precisão de 0.62 indica que 62% das previsões de "Pneumonia" são corretas.

O recall de 0.86 mostra que o modelo identifica corretamente 86% das imagens que são realmente pneumonia.

O modelo é significativamente mais eficaz em identificar corretamente as imagens de pneumonia em comparação à classe normal.

Conclusões e Recomendações:

Classe Normal: O modelo apresenta grandes dificuldades em identificar imagens normais, o que é evidente pelos valores baixos de precisão e recall. A grande quantidade de falsos positivos (203) e falsos negativos (54) para esta classe indica que há uma necessidade urgente de aprimoramento.

**Classe Pneumonia:** O modelo tem um desempenho relativamente bom na identificação de pneumonia, com uma precisão e recall muito melhores em comparação à classe normal. No entanto, ainda existem falsos negativos (54), onde o modelo falha em identificar pneumonia corretamente.
