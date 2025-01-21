1. Acesse o Azure Machine Learning Studio

    Vá até o portal Azure Machine Learning Studio.
    Faça login com sua conta da Microsoft Azure.

2. Crie um Workspace de Machine Learning (se necessário)

    No painel esquerdo, clique em "Workspaces" e crie um novo workspace, caso ainda não tenha.
    Preencha os campos necessários, como nome do workspace, assinatura, grupo de recursos, e região.

3. Configure o Ambiente de Trabalho

    No Workspace, clique em "Notebooks", "Datasets" ou diretamente em "Automated ML" no menu lateral, dependendo do fluxo desejado.

4. Carregue o Arquivo bike-rentals.csv

    No menu lateral, vá para "Datasets".
    Clique em "Create Dataset" e selecione "From Local Files".
    Escolha "Tabular" como tipo de dataset.
    Faça o upload do arquivo bike-rentals.csv:
        Clique em "Browse" e selecione o arquivo do seu computador.
        Preencha o nome do dataset (por exemplo: "Bike Rentals Dataset").
        Escolha um armazenamento vinculado ao workspace (Blob Storage ou Data Lake).
    Confirme e clique em "Next" até concluir a importação.

5. Crie uma Experiência de AutoML

    No menu lateral, clique em "Automated ML".
    Selecione "New Automated ML run".
    Escolha o dataset importado anteriormente (bike-rentals.csv).

6. Configure o Experimento

    Defina o Nome do Experimento:
        Exemplo: Bike_Rentals_Prediction.
    Escolha o Tipo de Tarefa:
        Para prever a quantidade de bicicletas alugadas, escolha "Regression".
    Selecione a Coluna-Alvo (Label):
        Escolha a coluna do dataset que representa o valor a ser predito (por exemplo, count ou rentals).
    Defina a Configuração de Execução:
        Escolha o cluster de computação (ou crie um novo):
            Vá em "Manage" > "Compute" > "New Compute Cluster".
            Escolha o tipo de cluster e o tamanho da máquina virtual (por exemplo, Standard_DS3_v2).

7. Personalize as Configurações de Treinamento

    Escolha as métricas de avaliação (ex.: R2 score, Mean Absolute Error).
    Defina o tempo máximo de execução para o experimento.
    (Opcional) Ative a Explicabilidade do Modelo para entender melhor as previsões.

8. Inicie o Treinamento

    Clique em "Start" para iniciar o treinamento automático.
    O Azure testará automaticamente vários modelos e hiperparâmetros para encontrar o mais adequado.

9. Analise os Resultados

    Após a conclusão do experimento, vá para "Best Model".
    Veja as métricas de desempenho do modelo (ex.: R2, MAE, RMSE).
    Clique em "Deploy" para publicar o modelo como um endpoint.

10. Implemente o Modelo (Opcional)

    No menu lateral, vá para "Endpoints" e configure o endpoint do modelo.
    Teste o endpoint enviando entradas de exemplo (como dados de aluguel de bicicletas).