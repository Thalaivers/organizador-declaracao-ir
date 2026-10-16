# Organizador de Declaração de Imposto de Renda

## Sobre o projeto

Este projeto foi desenvolvido como parte do curso **Analista de Dados com Excel com auxílio de IA e Claude**, oferecido pela DIO.

O objetivo é construir uma ferramenta no Excel para organizar informações cadastrais, informes de rendimentos bancários e registros de entradas financeiras que podem auxiliar na preparação dos documentos para a declaração do Imposto de Renda.

A proposta é centralizar informações em uma única pasta de trabalho, facilitando o preenchimento, a consulta e a organização dos dados por meio de abas estruturadas, listas de opções e cálculos automáticos.

## Objetivos do projeto

- Centralizar informações cadastrais do titular.
- Organizar valores e informações de informes de rendimentos bancários.
- Registrar entradas financeiras por data, categoria e valor.
- Padronizar informações por meio de tabelas de referência.
- Automatizar a soma de valores registrados.
- Facilitar a navegação e a organização das informações em uma única ferramenta.

## Estrutura da planilha

O arquivo está organizado em quatro abas principais:

### 1. TITULAR

Esta aba reúne os dados cadastrais do contribuinte, incluindo nome, CPF, data de nascimento, título de eleitor, endereço, telefone, celular e e-mail.

Também contém campos para registrar informações complementares, como alterações em relação à entrega anterior, dependência do cônjuge e residência no exterior.

Foram utilizadas listas de validação de dados com as opções "SIM" e "NÃO" para padronizar as respostas dos campos correspondentes na planilha de TITULAR e formatação personalizada dos campos CPF, CEP, Telefone e Celular.

A validação de dados permite restringir ou orientar as informações inseridas pelo usuário, conforme as opções configuradas.

### 2. INFORMES

Esta aba permite registrar informações de até três informes de rendimentos bancários, incluindo:

- Banco;
- Valor atual;
- Nome do arquivo utilizado como anexo.

O campo de totalização utiliza a função SOMA para calcular automaticamente o valor agregado dos registros bancários.

A fórmula utilizada na célula C7 é:

`=SOMA(D12,D17,D22)`

Essa fórmula soma os valores informados nas células D12, D17 e D22, facilitando a visualização do total registrado, esse recurso reduz a necessidade de somar os valores manualmente e facilita a conferência do total informado.

 Foi utilizado validação de dados com as opções de bancos na planilha INFORMES cujo os dados estão puxando as informações da tabela ocultada na planilha 4.

### 3. NOTAS

Esta aba organiza as entradas financeiras do titular, permitindo registrar:

- Data;
- Categoria da entrada;
- Valor.

Foi configurada uma lista de validação para o campo de categoria, com opções como holerite, CNPJ e freelance. O objetivo é padronizar os registros e facilitar sua identificação e organização.

### 4. TABELAS

Esta aba contém uma lista de instituições bancárias, organizada para servir como referência para os dados registrados na ferramenta.

A utilização de uma tabela de referência contribui para a padronização dos nomes dos bancos e para a organização das informações, facilitando a manutenção e atualização da lista.

### Organização por abas

A divisão da ferramenta em quatro abas separa as informações cadastrais, bancárias, financeiras e de referência. Essa estrutura facilita a localização dos dados e torna o arquivo mais organizado.

## Como utilizar a ferramenta

1. Preencher os dados cadastrais na aba TITULAR.
2. Registrar as informações dos informes bancários na aba INFORMES.
3. Informar os valores e os dados correspondentes aos registros financeiros na aba NOTAS.
4. Consultar o total calculado automaticamente na aba INFORMES.

Recomenda-se revisar os dados inseridos e conferir os documentos originais antes de utilizar as informações na preparação da declaração.

## Aprendizados e aplicação prática

O desenvolvimento deste projeto permitiu aplicar conhecimentos de Excel em uma situação prática de organização de dados financeiros e cadastrais.

Entre os principais aprendizados estão a estruturação de informações em abas, a criação de um menu que linka as abas correspondentes, a utilização de fórmulas para automatizar cálculos, a aplicação de validações de dados e a organização de tabelas de referência.

O projeto também reforça a importância de documentar uma ferramenta de maneira clara, permitindo que outras pessoas compreendam seu objetivo, sua estrutura e seus recursos.

## Limitações e considerações

Esta ferramenta tem finalidade organizacional e educacional. Ela auxilia na reunião e na conferência de informações, mas não substitui o programa oficial da Receita Federal, não realiza por si só a declaração do Imposto de Renda e não determina automaticamente todas as obrigações tributárias do contribuinte.

Os dados registrados devem ser conferidos com os documentos oficiais e com as orientações vigentes da Receita Federal.

O arquivo disponibilizado para demonstração deve utilizar dados fictícios, preservando a privacidade e a segurança das informações pessoais e financeiras.
