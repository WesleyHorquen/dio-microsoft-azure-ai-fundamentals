# Explore o Machine Learning Automatizado no Azure Machine Learning

## Preparando o ambiente do Azure Machine Learning

- Criar um espaço de trabalho do Azure Machine Learning através do link https://portal.azure.com
- Vá em **Criar um recurso**, pesquise por **Machine Learning** e crie um novo recurso seguindo os seguintes passos:

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/d55dc457-aaee-4615-b670-a10acdbe2f1c)
- Selecione **Criar**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/49e2df6e-f28e-4fad-aa82-e422baa815ef)
- Em **Grupo de recursos** escolha um grupo, ou **Crie novo** clicando abaixo, **Nome** defina um de sua preferência, **Região** pode deixar essa mesmo, após isso apenas apertar em **Examinar + Criar** depois **Criar** novamente

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/25a210de-ea41-4d59-84f5-0f84c1f5207d)
- Feito isso vamos **Ir para o recurso**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/bb4c8740-70e0-4307-bbe3-1a74cf5dfb57)
- E posteriormente **Iniciar o estúdio**, você será redirecionado para a página de Estúdio de Aprendizado de Máquina

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/10feb17d-ec80-49fe-bbd1-ac5d604e7ea6)


## Usando o aprendizado de máquina automatizado para treinar um modelo

- No canto esquerdo vamos em **ML automatizado**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/d09f9a65-8bc3-43bc-9fe8-3e16622674fd)
- Depois em **+ Novo trabalho de ML automatizado**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/2003e712-643f-4a99-b5b9-97120023c0a6)
- Devemos preencher da seguinte maneira e depois clicar **Avançar**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/6214b289-364d-4cfd-a359-709df9dfa5f6)
- Em **Tipo de Tarefas de Dados** devemos colocar em **Regressão** e depois em **+ Criar**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/cf643125-a0d3-4969-9540-6246fb5c5fb0)
- Devemos preencher da seguinte maneira e depois clicar **Avançar**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/3aba430d-8171-4cfc-bf9c-89ab9026d0ed)
- Selecionaremos **De arquivos Web** e depois **Avançar**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/c7871e81-e722-411a-831e-1ecc0e6b410d)
- Preencher com a *URL da Web** https://aka.ms/bike-rentals e depois avançar

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/f6698b35-ff24-4c7b-b396-c758fba0ab86)
- Manter as opções **Delimitado**, **Vírgula** e **UTF-8** e alterar a aba **Cabeçalhos de coluna** para **Somente o primeiro arquivo tem cabeçalho** e após **Avançar**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/55c40bd8-4d4a-4fe5-84b6-b9b97f8c79c0)
- Deixar todas as opções marcadas exceto **Path** depois **Avançar**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/bf1be5c7-b0fd-41eb-bdd4-f7967332cbfd)
- Examinar e **Criar**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/768d6015-307b-41f8-88cd-866daa6cd226)
- Após criado selecionamos na bolinha ao lado no nome que demos aluguel-de-bicicletas e **Avançar**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/a97c1734-860f-4e3a-bd98-1f09abcd1335)
- Em **Coluna de destino** selecionamos a última opção **rentals (Integer)**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/ffd71fa8-1f72-4c2d-b4bb-a9b5c04edf1a)
- Após isso clicamos em **Exibir definições de configuração adicionais** e deixar exatamente assim, **Méttrica primária** NormalizedRootMeanSquaredError, as caixas todas desmarcadas, **Modelos permitidos** apenas RandomForest, LightGBM, e salvamos

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/b5d7d958-e731-4f02-b134-0f65506a8ac0)
- Em **Limites** preencheremos desta maneira e após habilitamos a caixinha também

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/f00622cf-224f-4aff-899f-a2045833873b)
- Em **Tipo de validação** escolher a opção **Divisão de validação de treinamento** e deixar a caixa em 10 por padrão e clicar em **Avançar**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/9c0687ec-b8d4-4d47-a2f3-74d0c5586a90)
- Nesta parte deixamos exatamente como está e clicamos em **Avançar**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/07523b64-83f0-497e-b610-b098dc058c99)
- Revisamos os dados e clicamos em **Enviar trabalho de treinamento**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/7a061839-e4a3-4feb-9fb4-f771601ad400)
- Nessa parte era para estar **Status concluído** porém tem apresentado erro conforme outros colegas comunicaram via fórum

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/e36ed9bb-0289-4c88-8c5f-a1131d2a1dce)



# Para conseguir o resultado **CONCLUÍDO** eu tive que alterar a parte de Servidor em **Computação**

- Em **Selecione o tipo de computação** mudei para **Cluster de Cálculo** e após apertei em **+ Novo**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/9e3fe3a0-3ad5-4b75-9a31-11fe78c669e3)
- Mantive tudo exatamente como está

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/066e7dc6-a795-4026-a7b5-ad99b1d5b190)

- Na próxima página apenas criei um nome em **Nome da computação** e apertei em **Criar**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/4f17f87f-3739-4f01-8327-6466d83ad057)
- E assim chegamos ao mesmo resultado esperado **Concluído**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/d598ea57-e5e9-413e-ab7c-39d52aeaa895)

## Para testar e implementar o modelo

- Em **Saídas** iremos acessar o modelo

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/1e56a7e3-825d-40a2-a700-d45169ec93a3)
- Acessamos o **Criado por trabalho**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/2c004953-067d-46dc-a18d-148751d90560)
- Vamos em **Implementar** depois em **Serviço Web**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/3bcb44cc-c2f5-4077-ba68-83df7a4d1c88)
- Devemos preencher desta forma e clicar em **Implantar**

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/b8888143-84b4-4cd2-b6ba-2ea1effdae91)

- Porém tem apresentado erro também e não consegui passar daqui

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/0f7d7aa2-5f9c-4a28-a9d8-0d0c97629941)


# Segue abaixo o passo a passo que era para ocorrer


- Era para ter concluído a Implementação

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/4fdc6639-0c8c-4476-9e9e-bd37b917660c)
- Depois abriríamos a parte de teste

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/e254e2f5-8ca2-4118-8dee-9e4d8314f923)
- Trocaríamos o json pelo que é entregue pela documentação

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/c08f0e17-a7d5-47cc-ae5d-a2dddace8e0c)
- E esse deveria ser o resultado do teste

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/dd78dcc6-ed9c-47ec-b409-38adb51db20d)

# Imput

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/b550976a-ec24-4fa9-94b2-095aa19554c4)

# Resultado

![image](https://github.com/WesleyHorquen/dio-microsoft-azure-ai-fundamentals/assets/89001286/1e8b94cb-3fa2-4f25-b381-87eae2b1b96f)


 
