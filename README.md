3. Matriz 5W2H (Plano de Ação do Projeto)

O 5W2H é uma ferramenta de gestão. Você pode desenhar isso como uma tabela direta no seu trabalho, respondendo às 7 perguntas fundamentais sobre o sistema de vocês.

    What (O que será feito?): Desenvolvimento de um sistema web de gestão e agendamento para barbearias, composto por uma API REST no backend e uma interface gráfica no frontend.

    Why (Por que será feito?): Para resolver problemas de organização de agenda, mitigar o risco de sobreposição de horários e eliminar o tempo gasto pelo profissional no atendimento via telefone/mensagens durante o expediente.

    Where (Onde será feito/implementado?): O desenvolvimento ocorre em ambiente acadêmico/local, e a implementação será destinada à barbearia real do cliente, com o sistema hospedado em servidores em nuvem.

    When (Quando será feito?): Durante o decorrer do 3º semestre do curso superior (inserir os meses de início e fim da entrega do projeto).

    Who (Por quem será feito?): Pela equipe de desenvolvimento composta por dois alunos: Vitor (Responsável pela Arquitetura, Banco de Dados PostgreSQL e Backend em C++ com framework Drogon) e Thiago (Responsável pelo Frontend, UI/UX e consumo da API via requisições assíncronas).

    How (Como será feito?): Através da divisão de responsabilidades. O backend fornecerá endpoints via HTTP (operações CRUD) e se comunicará com um banco de dados relacional. O frontend consumirá esses dados via Javascript (Fetch API) para renderizar a interface do calendário e o painel administrativo.

    How Much (Quanto custará?): O custo financeiro é próximo a zero, utilizando ferramentas de código aberto (Open Source), IDEs com licença de estudante (CLion) e bancos de dados gratuitos para a construção do MVP (Produto Mínimo Viável). O custo principal é o tempo de desenvolvimento da equipe.
---

🐟 Parte 1: Árvore de Problemas (Ishikawa Tradicional)

Dica visual: Use a cor Vermelha ou Laranja para os contornos deste diagrama, pois representa os pontos de dor.
🛠️ Guia de Símbolos
Elemento do Peixe	Símbolo a usar	O que escrever	Posição no Canvas
Cabeça do Peixe	Retângulo Grande	Desorganização, falhas humanas e perda de tempo no processo manual.	Extrema Direita (Centro)
Espinha Dorsal	Seta Longa Horizontal	(Linha reta, sem texto)	Do centro-esquerda até a Cabeça
Categorias	Retângulos Médios	Métodos, Mão de Obra, Ferramentas, Meio Ambiente	Bordas superiores e inferiores
Espinhas Principais	Setas Diagonais	(Linhas que ligam as Categorias à Espinha Dorsal)	Inclinadas apontando para o centro
Causas Detalhadas	Texto sem borda ou pequenas setas horizontais	(As causas específicas listadas)	Ligadas nas laterais das setas diagonais
🗺️ Passo a Passo da Montagem (Problemas)

    O Efeito: Desenhe um grande Retângulo do lado direito da tela e escreva o problema principal (Desorganização, falhas humanas...).

    A Espinha Central: Puxe uma seta longa da esquerda da tela até encostar nesse Retângulo.

    As Categorias de Cima: Desenhe dois Retângulos na parte superior da tela. Escreva "Métodos" no primeiro e "Mão de Obra" no segundo. Puxe uma seta diagonal de cada um deles apontando para baixo, até tocar a seta central.

    Detalhando Cima: Puxe linhas horizontais saindo da seta diagonal de "Métodos" e escreva: Agendamento estritamente síncrono e Falta de validação lógica. Faça o mesmo na seta de "Mão de Obra" com as respectivas causas.

    As Categorias de Baixo: Desenhe dois Retângulos na parte inferior da tela. Escreva "Ferramentas" e "Meio Ambiente". Puxe setas diagonais subindo até tocar a seta central.

    Detalhando Baixo: Puxe linhas horizontais das setas de baixo e adicione os textos específicos (Dependência de cadernos físicos..., etc.).

🟢 Parte 2: Árvore de Objetivos (Ishikawa Reverso)

Dica visual: Use a cor Verde ou Azul para este diagrama, indicando solução, metas e um estado futuro positivo.

A estrutura geométrica é exatamente a mesma do diagrama anterior, o que muda é a direção psicológica (ao invés de mapear o que deu errado, mapeia o que precisamos fazer para dar certo).
🛠️ Guia de Símbolos
Elemento do Peixe	Símbolo a usar	O que escrever	Posição no Canvas
Cabeça do Peixe	Retângulo Grande	Sistema 100% automatizado, autônomo e zero choques de horário.	Extrema Direita (Centro)
Espinha Dorsal	Seta Longa Horizontal	(Linha reta, sem texto)	Do centro-esquerda até a Cabeça
Categorias	Retângulos Médios	Métodos, Mão de Obra, Ferramentas, Meio Ambiente	Bordas superiores e inferiores
Espinhas Principais	Setas Diagonais	(Linhas que ligam as Categorias à Espinha Dorsal)	Inclinadas apontando para o centro
Meios de Solução	Texto sem borda ou pequenas setas horizontais	(As soluções técnicas e práticas)	Ligadas nas laterais das setas diagonais
🗺️ Passo a Passo da Montagem (Objetivos)

    O Objetivo: Desenhe o grande Retângulo do lado direito e insira o objetivo central (Sistema 100% automatizado...).

    A Espinha Central: Puxe a seta longa horizontal da esquerda para a direita.

    Categorias de Cima (Soluções): Posicione os blocos "Métodos" e "Mão de Obra" no topo. Puxe as setas diagonais para o centro.

    Detalhando Cima: Nas linhas horizontais anexas à seta de "Métodos", escreva: Autoatendimento assíncrono e Restrições de banco de dados (UNIQUE). Na de "Mão de Obra", coloque a Liberação cognitiva e a Transferência do controle.

    Categorias de Baixo (Soluções): Posicione os blocos "Ferramentas" e "Meio Ambiente" na parte inferior. Puxe as setas diagonais para cima em direção ao centro.

    Detalhando Baixo: Preencha os detalhes técnicos: em "Ferramentas", adicione a API RESTful em C++ (Drogon) e a Aplicação Web (Mobile-first). Em "Meio Ambiente", coloque a Rotina contínua sem interrupções e o Painel administrativo em tempo real.
