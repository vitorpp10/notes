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

1. Árvore de Problemas (Modelo Ishikawa)

Este diagrama mapeia as causas raízes que geram o problema atual da barbearia.

    Cabeça do Peixe (O Problema Principal / Efeito): Desorganização, falhas humanas e perda de tempo no processo manual de agendamentos.

    Espinhas Superiores (Causas - Categorias 1 e 2):

        Métodos (Processos):

            Agendamento estritamente síncrono (depende de resposta em tempo real).

            Falta de validação lógica (risco de anotar dois clientes no mesmo horário).

        Mão de Obra (Pessoas):

            Acúmulo de funções (o barbeiro atua como prestador de serviço e recepcionista simultaneamente).

            Cliente sem autonomia para consultar a agenda por conta própria.

    Espinhas Inferiores (Causas - Categorias 3 e 4):

        Ferramentas (Tecnologia/Materiais):

            Dependência de cadernos físicos e anotações manuais sujeitas a rasuras.

            Uso de aplicativo de mensagens pessoal (WhatsApp) para fins corporativos misturados.

        Meio Ambiente (Contexto do Salão):

            Interrupções constantes do serviço físico para checar o smartphone.

            Quebra de foco do profissional durante cortes complexos.

2. Árvore de Objetivos (Modelo Ishikawa Reverso)

A Árvore de Objetivos é a inversão exata da Árvore de Problemas. As causas negativas viram os meios de solução, e o problema principal vira o objetivo central.

    Cabeça do Peixe (O Objetivo Principal / Efeito Desejado): Sistema de agendamento 100% automatizado, autônomo e com integridade de dados (zero choques de horário).

    Espinhas Superiores (Meios de Solução - Categorias 1 e 2):

        Métodos (Processos):

            Implementação de autoatendimento assíncrono (disponível 24/7).

            Garantia de integridade via restrições de banco de dados (Constraint UNIQUE em data e hora).

        Mão de Obra (Pessoas):

            Liberação cognitiva do profissional (foco total na execução do corte).

            Transferência do controle de escolha diretamente para o cliente.

    Espinhas Inferiores (Meios de Solução - Categorias 3 e 4):

        Ferramentas (Tecnologia/Materiais):

            Desenvolvimento de API RESTful em C++ (Drogon) para alta performance.

            Aplicação Web intuitiva e responsiva (Mobile-first).

        Meio Ambiente (Contexto do Salão):

            Rotina de atendimento contínua, sem interrupções por notificações de celular.

            Acompanhamento visual em tempo real através de um painel administrativo.
