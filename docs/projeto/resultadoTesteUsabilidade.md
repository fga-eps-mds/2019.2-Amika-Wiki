## Introdução
Teste de usabilidade é uma técnica de caixa-preta, com objetivo de observar como usuários reais interagem com sua aplicação e através disto buscar pontos de melhoria.

## Participantes
- Professor da disciplna de Felicidade de Universidade de Brasilia(Professor Wander)
- Mediador do teste: Mateus de Oliveira


## Teste de Usabilidade presencial

* Métricas utilizadas no teste de usabilidade:
    - Número de etapas para executar um pedido específico
    - Tempo médio gasto pelo usuário em uma sessão

* Objetivos da aplicação do teste de usabilidade:
    - Identificar se o caminho que o usuário precisa percorrer está claro
    - Identificar se o usuário está satisfeito durante a utilização da aplicação
    - Identificar se as funcionalidades solicitadas para o administrador estão de acordo
    - Identificar bugs durante interação


### Atividades a serem executadas para realização do teste de usabilidade do professor

* Público: O teste de usabilidade será aplicado para o professor Wander, da disciplina de Felicidade.

* Local: ITRAC - UnB.

* Horário: 16:30h

* Logistica de aplicação: Um membro da equipe acompanhará a interação do participante com a aplicação a fim de anotar as observações resultantes.


    #### Atividade 1
    - Usuário fazer o download da aplicação no celular
        * Colher dados como: 
            - Se a experiencia foi agradável
            - Se o usuário se sentiu perdido ou não soube o que fazer
            - Se possui alguma sugestão de melhoria
            - Se o aplicativo foi baixado corretamente na homepage
            - Se o usuário teve interesse imediato de baixar a aplicação
            
    #### Resultado:
    - Passos para realizar: 2(Abrir aplicação no celular, apertar no banner para efetuar download)
    - Tempo de execução: 7 segundos
    - Problemas na realização: Na primeira tentativa o usuário clicou para adicionar aplicação na tela inicial, porém antes de confirmar já saiu da tela para verificar se havia efetuado o download
    - Considerações sobre o erro: Por se tratar de uma medida de segurança padrão recomendada pelo próprio PWA, o popup de confirmação é necessário, logo para este caso não podem ser tomadas medidas quanto a isto, talvez uma resposta mais rápida do pop-up auxiliaria.
    - Experência do Usuário: O usuário não demonstrou qualquer insatisfação ou dúvida além do problema citado acima, o banner para download apareceu imediatamente e o download foi realizado corretamente, o usuário não exitou e nem precisou de qualquer comentário adicional para realizar o download, o fez por conta própria.


    #### Atividade 2
    - Criar uma agenda da felicidade
        - Analisar se o usuário conseguiu criar rapidamente uma das agendas da disciplina
        - Analisar se o usuário conseguiu editar rapidamente uma das agendas da disciplina
        - Analisar se o usuário conseguiu excluir rapidamente uma das agendas da disciplina
        - Analisar quantos caminhos foram necessários até realizar a atividade

    #### Resultado 
    - Passos para realizar: 7(Abrir a aplicação, efetuar o login, navegou pela homepage, navegou pela sidebar, digitou o caminho na URL, preencheu os dados, clicou para enviar)
    - Tempo de execução: 1 minuto e 57 segundos
    - Problemas na realização: A homepage que aparece ao efetuar o login não será mais utilizada, logo seus links em maioria não estavam funcionando o que causou uma certa duvida do usuário, por ser um primeiro contato deste com a aplicação em si ele teve uma certa curiosidade para navegar pelas outras páginas antes de realizar a atividade estimada e com isto relatou também uma necessidade ou vontade de retornar rapidamente para a página inicial. Outro problema relatado foi devido a esta página da atividade em si ainda não possuir um link direto, logo ele necessitou digitar o caminho na URL da aplicação.
    - Considerações sobre o erro: Os links para navegação devem ser revistos, a homepage deve ser removida e trocada imediatamente, e deve-se fornecer um botão de fácil acesso na aplicação para retornar sempre para a página inicial.
    - Experência do Usuário: Além dos comentários de erro citados acima, o usuário achou interessante a funcionalidade em si, mas gostaria que um certo conjunto de atividades já estivessem criados na aplicação pois são padrões da disciplina, logo deve-se considerar adicionar estas em um seed para que sempre tenha elas em mãos.

    #### Atividade 3
    - Criar turma
      * Pedir que o usuário crie uma nova turma
        - Analisar quantas etapas o usuário precisou para criar uma turma
        - Analisar os alunos daquela turma
        - Colher sugestões de melhorias
        - Colher dificuldades encontradas

    #### Resultado 
    - Passos para realizar: 3(Entrar na tela de turmas, digitou o nome da turma, clicou no botão para enviar)
    - Tempo de execução: 13 segundos
    - Problemas na realização: O usuário digitou a primeira vez "Felicidade" e como a turma só aceita no máximo 2 caracteres, a turma não foi criada, porém não houve nenhum feedback para o usuário, o erro aparece somente no console, causando assim uma confusão se a funcionalidade estava funcionando.
    - Considerações sobre o erro: Este campo deveria estar mais claro para o usuário e deveriam ser emitidos feedbacks instantaneos em casos de erro ou sucesso.
    - Experiência do usuário: Usuário não compreendeu muito bem a funcionalidade de inicio, imaginou que ao clicar nas turmas iriam aparecer todos os alunos daquela turma, porém no ocorreu. Entendeu um pouco melhor ao ver o gráfico de humor da turma.

    #### Atividade 4
    - Ver gráfico humor do dia
        * Induzir usuário a vero gráfico de humor do dia
            - Analisar se o usuário achou intuitivo o uso do gráfico
            - Analisar se a informação do gráfico foi útil
            - Analisar se o usuário teve dificuldades para realizar a atividade
            - Recolher sugestões de melhorias do usuário
            
    #### Resultado
    - Passos para realizar: 4(clicar na janela de turma, apertou na turma em si, apertou no ícone de editar, apertou no ícone para visualizar)
    - Tempo de execução: 48 segundos
    - Problemas na realização: O usuário executou passos demais para realizar a atividade, logo esta não estava bem intuitiva.
    - Considerações sobre o erro: Adicionar tooltips sobre os botões poderia auxiliar na experiência do mesmo.
    - Experiência do usuário: O usuário achou o gráfico interessante porém acabou possuindo este problema de não ter sido tão intuitivo os ícones para encontrar a tela.

    #### Atividade 5
    - Gerar Grupos
      * Pedir que o usuário gere os grupos da disciplina
        - Analisar quantas etapas o usuário precisou para gerar os grupos
        - Analisar quantos grupos foram formados
        - Analisar se a quantidade de alunos por grupo foi de acordo
        - Analisar se a listagem de grupos foi correta
        - Colher sugestões de melhorias
        - Colher dificuldades encontradas
        
     #### Resultado        
    - Passos para realizar: 2(Entrar na tela de grupos, clicar para gerar grupos)
    - Tempo de execução: 26 segundos
    - Problemas na realização: Ao clicar para gerar os grupos o tempo de carregamento foi alto(cerca de 7 segundos) e sem nenhum feedback para o usuário de que os grupos estavam sendo gerados, deixando o usuário confuso sem saber se a ação estava realmente sendo executada.
    - Considerações sobre o erro: Deve ser adicionado um alerta de sucesso ou erro em todas as atividades para fornecer para o usuário sempre algum feedback sobre o que está acontecendo, o tempo de carregamento deve ser diminuido.
    - Experiência do usuário: Após os grupos serem gerados(com o desconforto devido ao tempo de carregamento sem o feedback) o usuário foi visualizar os alunos de cada grupo, porém acabou apertando para editar o grupo e não imediatamente no painel colapsado para expandir e apresentar o restante das informações, um dos motivos que pode ter ocasionado neste erro foi o da tela anterior de turmas, na qual clicar diretamente no painel que é semelhante não gerava nenhum tipo de interação, logo podem ser levadas em consideração algum tipo diferente de design para telas que tenham este menu colapsado e telas que não tenham.
