## UC01 - Visualizar Cardápio

### Atores

Cliente - usuário cliente do estabelecimento

### Pré-condição

Nenhuma

### Fluxo Principal

P1. Visualizar Cardápio A1 A3
P1.1 Sistema exibe uma lista de restaurantes recomendados;
P1.2 O Cliente seleciona um restaurante da lista;
P1.3 O Sistema exibe o cardápio do restaurante; A2
P1.4 Caso de uso encerrado.

### Fluxo Alternativo

A1. Visualizar Cardápio
A1.1 O Sistema exibe a lista de pratos recomendados; A2
A1.2 Caso de uso encerrado.

A2. Selecionar Item
A2.1 O Cliente seleciona um item para ser adicionado ao carrinho;
A2.2 O Sistema atualiza os itens do carrinho;
A2.3 Caso de uso encerrado.

A3. Buscar Restaurante
A3.1 O Cliente informa o nome de um restaurante;
A3.2 O Sistema exibe a lista de restaurantes; P1.2

A4. Buscar Prato
A4.1 O Sistema exibe a lista de pratos; A2

### Fluxo de Exceção

E1. Falha na comunicação
E1.2 O Sistema detecta falha de comunicação com o servidor;
E1.3 O Sistema exibe mensagem "Falha de comnicação. Tente novamente mais tarde." (adicionar cachorrinho)
E1.4 Caso de uso encerrado.

E2. Sistema Lento
E2.1 O Sistema detecta que operações estão demorando mais que o esperado;
E2.2 O Sistema exibe mensagem "A solicitação está demorando mais que o esperado"; E1
E2.3 Caso de uso encerrado.

### Pós-condições

Sistema exibe cardápio

### Regras do Negócio

RN01 - Apenas restaurantes abertos podem informar o cardápio;
RN02 - Os restaurantes disponíveis são apenas na cidade do Cliente;

### Histórico

21/01/2025 - Versão Inicial do documento

### Notas de Implementação

O sistema será desenvolvido como um app mobile utilizando as tecnologias React Native com backend em Node.js em nuvem AWS.
