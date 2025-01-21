### Fluxo Principal

P1 Visualizar Carrinho
P1.1 O Cliente seleciona a opção "Carrinho";
P1.2 O Sistema exibe os itens adicionados no carrinho;
P1.3 O Sistema exibe valor dos itens + valor entrega;
P1.4 O Sistema exibe tempo estimado; A1 A2 A3 
P1.3 Caso de uso encerrado.

### Fluxo Alternativo

A1. Adicionar mais produtos
A1.1 O Cliente seleciona a opção "Continuar comprando";
A1.2 O Sistema retorna a tela anterior;

A2. Remover produtos
A2.1 O Cliente remove um produto;

A3. Cancelar compra
A3.1 O Cliente selecionar a opção "Cancelar";
A3.2 O Sistema esvazia o carrinho;
A3.3 O Sistema retorna para a tela inicial;
A3.4 Caso de uso encerrado.

A4. Finalizar Compra
A4.1 O Cliente seleciona a opção "Finalizar"; E2
A4.2 O Sistema exibe a tela para selecionar a forma de pagamento;
A4.3 O Cliente seleciona a forma de pagamento;
A4.4 O Serviço de Pagamento processa o pagamento; E1
A4.5 O Sistema confirma o pagamento;
A4.6 Caso de uso encerrado.

### Fluxo de Exceção

E1. Pagamento Não Autorizado
E1.1 O Serviço de Pagamento informa pagamento não autorizado;
E1.2 O Sistema informa ao Cliente: "Não foi possivel realizar o pagamento"; A4.3

E2. Item indisponível
E2.1 O Sistema informa que algum dos itens não estão mais disponíveis;
E2.1 O Sistema informa a remoção do item; P1.3