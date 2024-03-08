# Atividade Ponderada - Cypress - Semana 5

## O que é o Cypress e para que serve?
O Cypress é uma ferramenta de teste de front-end construída visando a nova geração do desenvolvimento web. Ela é projetada para simplificar o processo de testes, permitindo aos profissionais a automatização de testes de unidade, testes de integração e testes de interface de usuário (UI) em um ambiente real de navegador. O que traz um diferencial diante de outras ferramentas de teste que operam por simulação em um navegador falso, o Cypress executa testes em um navegador real.

## Vantagens e desvantagens do Cypress em relação a outras ferramentas de teste

### Vantagens
A Facilidade de uso embutida no Cypress: A API é de um uso muito simples e compreensível, o que a torna acessível até mesmo para desenvolvedores e testers com pouca experiência em automação de testes.

Execução em navegadores que geralmente são utilizados: A execução de testes em um navegador real resulta em uma maior precisão nos testes de interface.

Interações instantâneas: O Cypress oferece feedback visual imediato das ações executadas nos testes, através da sua interface que roda os testes.

### Desvantagens

Pouca variedade de navegadores: Devido ao fato de ser uma ferramenta um pouco mais recente no mercado, o Cypress tem suporte limitado a navegadores quando comparado a outras ferramentas como Selenium.

Não suporta abas múltiplas: Cypress não permite testar a funcionalidade que envolve múltiplas abas do navegador de forma nativa.

## Arquitetura do Cypress

A arquitetura do Cypress é diferenciada, pois opera diretamente dentro do navegador. Isso permite que ele trabalhe em conjunto com o aplicativo sendo testado, oferecendo controle total sobre o DOM, os eventos, o armazenamento local e as chamadas de rede. O que o diferencias das demais ferramentas baseadas em Selenium que operam fora do navegador e se comunicam com o aplicativo através de um driver, o Cypress executa junto com o código do aplicativo, permitindo com que os testes fiquem mais rápidos e precisos.

## Seletores de elementos no Cypress

O Cypress utiliza seletores de elementos para interagir com os elementos da página web. Estes podem ser seletores CSS ou jQuery, permitindo que o usuário selecione elementos de forma interativa e flexível. Exemplos comuns incluem o uso de classes, IDs, atributos, entre outros.

## Comandos e asserções no Cypress

Os comandos no Cypress são usados para interagir com a página, navegando por ela, clicando em elementos e digitando em campos de formulário.
As asserções são usadas para verificar se o estado da aplicação é o esperado. O Cypress suporta asserções tanto de forma implícita quanto explícita, permitindo que os devs verifiquem propriedades como visibilidade, conteúdo de texto, atributos CSS, entre outros.

## Descrição das etapas de preparação de um testes de interface, execução e verificação no Cypress

### Preparação
Instalação e Configuração: Instalar o Cypress via npm e configurar o projeto conforme necessário.

Criação de Testes: Escrever os testes dentro da pasta cypress/integration, usando a sintaxe Mocha que o Cypress adota.

### Execução
Abrir o Test Runner: Usando o comando cypress open, o Test Runner do Cypress é iniciado, permitindo a seleção e execução de testes específicos.

Execução de Testes: Os testes são executados em um navegador real. O Cypress permite a execução de testes de linha de comando para integração contínua.

### Verificação
Verificar Resultados dos Testes: Os resultados são exibidos na interface que roda o teste, incluindo asserções falhas e representações visuais de testes falhos.

Debugging: Utilizar as ferramentas de debugging do Cypress e do navegador para investigar testes que não passaram.

## Como estruturar testes de forma eficiente no Cypress?

Organizar testes em arquivos bem definidos: Basear a separação em funcionalidades ou páginas da aplicação. Com isso, o entendimento e manutenção posterior ficarão mais palpáveis e fáceis de entender.

Uso de Hooks: Para preparar o estado necessário antes de cada teste ou limpar após cada teste.

Page Objects: Utilizar o padrão de Page Objects para encapsular comportamentos de páginas, tornando o código de teste mais reutilizável e fácil de manter.

Comentários e documentação: Documentar os testes claramente para facilitar a compreensão dos objetivos e etapas de cada teste.