# Analise-de-Sentimento
Trabalho final da matéria de BI na Pós Graduação em BI-Master na PUC-RJ

## Trabalho Proposto
- Desenvolver modelo preditivo para classificar como POSITIVOS ou NEGATIVOS os comentários redigidos em texto livre por clientes de um hotel
- Foi disponibilizada base de dados com vários comentários de clientes já classificados como POSITIVOS ou NEGATIVOS para servir como base de treino e teste do modelo
- Segue, abaixo, amostra de parte da base de dados apresentando comentários e as respectivas classificações:

  | Comentário    | Classificação | 
  | ------------- |:-------------:| 
  | Os quartos são limpos, possuem um excelente Ocean View, serviço de quarto, O hotel no geral é bem grande e confortável, há diversos tipos de piscinas para todas as idades, com entretenimento dos monitores | 	Positivo |
  | Os atendentes são muito corteses e estão sempre dispostos a ajudar |	Positivo |
  | Superou as expectativas, principalmente quanto a comida e estrutura. Excelente piscina, ótimos restaurantes e drinks | Positivo |
  | Excelente, serviço impecável comida maravilhosa | Positivo |
  | O hotel é excelente em diversos aspectos, desde a localização até o serviço geral. A comida é muito boa e variada. As bebidas são de boa qualidade e de marcas conhecidas. O serviço de quarto e a limpeza também são quase impecáveis | Positivo |
  | Foi algo deplorável | Negativo |
  | As habitações são velhas e sem nenhum cuidado | Negativo |
  | Nunca imaginei que a rede Othon mantivesse uma unidade em tão mau estado e com atendimento tão precário | 	Negativo |
  | hotel é muito antigo e com equipamentos muitos velhos, mesmo na taxa superior |	Negativo |
  | difícil é falar de um hotel ruim. Preço elevadíssimo considerando o péssimo nível de serviço e qualidade das instalações | 	Negativo |
  | Quero deixar registrado aqui minha profunda insatisfação com os serviços prestados |	Negativo |


## Resumo do Trabalho Desenvolvido

- O trabalho foi desenvolvido em [RapidMiner](https://rapidminer.com/)

- Dentre as simulações realizadas a que proporcionou o melhor desempenho conta com a aplicação das seguintes técnicas:
  - Tokenização
  - Filtragem de StopWords
  - Stemização (SnowBall)
  - TF-IDF com aplicação de Método Prune
  - Seleção de Atributos pelo Peso da Correlação deles com o Atributo Label (resultado esperado) 
  - Aplicação do Modelo SVM 

- O melhor desempenho obtido teve Acurácia de 97,07% e Kappa de 0,941

- O arquivo [Trabalho Final - BI(LEONARDO) - Fernando Mauro Buleo Barbosa.docx](https://github.com/buleo/Analise-de-Sentimento/blob/main/Trabalho%20Final%20-%20BI(LEONARDO)%20-%20Fernando%20Mauro%20Buleo%20Barbosa.docx) em anexo contém relatório detalhando o modelo desenvolvido e os experimentos realizados

## Arquivos
- "Trabalho Final - BI(LEONARDO) - Fernando Mauro Buleo Barbosa.docx" - Relatório detalhando o modelo desenvolvido e os experimentos realizados
- "Hoteis - TextProcessing-PassoAPasso.rmp" - Arquivo em [RapidMiner](https://rapidminer.com/) com o modelo desenvolvido
- "hoteis.arff" - Arquivo com a base de comentários classificados para treino e teste do modelo
- "StopWords.txt" - Arquivo com a relação de StopWords consideradas no modelo
