# Site-AuAu-Shop

# 🐾 AuAu Shop - Seu Pet, Nosso Amor (E-Commerce / PDV WhatsApp)

Um sistema web completo no formato Single Page Application (SPA) desenvolvido para gerenciar a vitrine de produtos, carrinho de compras e integracao direta de pedidos para o WhatsApp de uma pet shop. O sistema conta com recursos de acessibilidade e foi projetado para ser rapido, responsivo (mobile-friendly) e totalmente testado de forma automatizada.

## 🚀 Funcionalidades Principais

O sistema e dividido em modulos integrados na mesma interface:
* 🛒 Vitrine Dinamica de Produtos: Catalogo moderno com 8 produtos em destaque, organizados em formato de grade simetrica com imagens otimizadas e efeitos visuais ao passar o mouse.
* 🛍️ Carrinho de Compras Inteligente: Sistema interativo que permite adicionar itens, calcula automaticamente o valor total da compra em tempo real e atualiza o contador de itens no topo da pagina.
* 🗑️ Modulos de Seguranca e Confirmacao: Caixa de dialogo (modal) customizada que exige a confirmacao do usuario antes de remover qualquer item do carrinho, evitando exclusoes acidentais.
* 💬 Finalizacao via WhatsApp: Integracao automatica que gera uma mensagem formatada profissionalmente contendo a lista de produtos pedidos, os precos individuais e o valor total, direcionando o tutor direto para o contato da loja.
* ♿ Acessibilidade Integrada (VLibras): Ferramenta oficial instalada e configurada para permitir a traducao instantanea de todo o conteudo do site para a Lingua Brasileira de Sinais (Libras).

## 🛠️ Tecnologias Utilizadas

Este projeto foi construido focando no dominio das linguagens base da web e na automacao de testes de software:
* Frontend: HTML5, CSS3 (com variaveis CSS para controle de paleta de cores e layout responsivo Flexbox) e JavaScript puro (Vanilla JS) para a logica do carrinho de compras.
* Ferramenta de Testes (QA): Cypress (versao 15.17.0) para automacao e execucao de testes de ponta a ponta (E2E).
* Ambiente de Execucao: Node.js (gerenciador de pacotes npm) para controle das dependencias de desenvolvimento.

## 🧪 Casos de Teste Automatizados (Cypress)

O projeto conta com uma suite completa de testes automatizados para garantir a qualidade do software e a experiencia do usuario:
* Caso de Teste 1: Adicionar Produto ao Carrinho - Valida se o clique no botao injeta o item corretamente, se a notificacao de sucesso e disparada e se o contador do topo incrementa.
* Caso de Teste 2 e 3: Calculo do Total e Remocao com Confirmacao - Testa a soma automatica de múltiplos produtos no carrinho e simula o fluxo do modal de confirmacao ao clicar no botao remover.
* Caso de Teste 4: Finalizar Compra pelo WhatsApp - Utiliza tecnicas de espionagem de codigo (stubs) para interceptar e validar se o link final gerado contem o numero internacional correto da loja e os dados do pedido.

## 💻 Como rodar este projeto localmente

Para executar este projeto e rodar a suite de testes na sua maquina para apresentacoes:

1. Baixe os arquivos do projeto para uma pasta no seu computador.
2. Abra o terminal do seu editor de codigo (ex: VS Code) dentro da pasta raiz do projeto.
3. Certifique-se de ter o Node.js instalado e rode o comando abaixo para instalar as dependencias:
   ```bash
   npm install
