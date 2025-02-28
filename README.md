# exercicio_config
gherkin 

#language: pt

Funcionalidade: configurar produto 

Cenário: Adicionar Produto ao Carrinho
Quando o usuário selecionar a cor, tamanho, quantidade e clina em "adicionar ao carrinho"
E o número de produtos no carrinho é menor ou igual a 10
Então o produto é adicionado com as opções selecionadas e o valor total é atualizado
Quando o usuário clica em "Limpar"  
Então o carrinho é esvaziado e o usuário retorna ao estado original
    
    Exemplos:
    | cor      | tamanho | quantidade |
    | Azul     | XS      | 1          |
    | Vermelho | M       | 5          |
    | Laranja  | XL      | 10         |
    
