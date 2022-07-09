# Teste de seleção para vaga de Java
- ## Definição do projeto
    - Nome : SigaBem Cargas
    - Descrição : Aplicação para cálculo do preço do frete
    - Objetivo : Torna mais pratico o repasse para o cliente o valor do frete, padronizando e tornando um atendimento mais rapido.
- ## Requisitos do projeto
    - ### Entidades :
        1.  Origem :
            - Cep
            - Estado
            - DDD 
        2. Destino : 
            - Nome Destinatario      
            - Cep 
            - Estado
            - DDD
            - Peso 
        3. Transporte :
            - Valor Frete por km
            - Valor total do frete
            - Data solicitação
            - Data prevista para Entrega 
            - Data da Consulta    
    - ### Requisitos :
        1. Permitir Criar Um Transporte
        2. Permitir visulizar Valor Toal do frete
        3. Permitir Visualizar Data prevista para entrega
        4. permitir Visualizar Cep Origem e Cep Destino
    - ### Regras de negocio :
        1. Não tem um sistema de login.
        2. Não tem conceito de usuario
        3. CEPs com DDDs iguais tem 50% de desconto no valor do frete e entrega prevista de 1 dia
        4. CEPs de estados iguais tem 75% de desconto no valor do frete e entrega prevista de 3 dias
        5. CEPs de estados diferentes não deve ser aplicado o desconto no valor do frete e entrega prevista de 10 dias
        6. O valor do frete é cobrado pelo peso da encomenda, o valor para cada KG é R$1,00
        7. Endpoint pode ser público Response/Output deve possuir: “vlTotalFrete” e “dataPrevistaEntrega”, “cepOrigem” e “cepDestino” Deve ser persistido no banco os valores da cotação os valores consultados: “peso”, “cepOrigem”, “cepDestino”, “nomeDestinatario”, “vlTotalFrete”, “dataPrevistaEntrega” e “dataConsulta”
    - ### Definição da tecnologia
        1. Java (Liguagem)
        2. Mysql (Banco de Dados)
        3. API Viacep
