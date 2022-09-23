# Introdução à segurança ofensiva | TryHackMe

![image](https://user-images.githubusercontent.com/98756562/191946070-feb61a9b-973e-4148-83e1-b8a792163a2d.png)


Acesso ao laboratório: https://tryhackme.com/room/introtooffensivesecurity

![image](https://user-images.githubusercontent.com/98756562/191946150-10da43a1-87e5-40b6-bfd8-3585d252afbc.png)

**1º — Abra um terminal**

Podemos interagir com um computador sem usar uma interface gráfica de usuário usando um terminal, geralmente conhecido como linha de comando. Usando o ícone Terminal no sistema, abra o terminal:

![image](https://user-images.githubusercontent.com/98756562/191946246-a4aaef3c-d036-426c-b857-4ec6e770cd9a.png)
Ícone do terminal do Kali Linux

**2º — Encontre as páginas do site que foram ocultadas**

A razão para isso é que muitas empresas terão seu próprio portal de administração, que dará a seus funcionários acesso a controles administrativos básicos para atividades do dia-a-dia.

``Exemplo: Um funcionário do banco pode transferir fundos de investimento ou outro tipo para contas de clientes.``

Essas páginas geralmente não são privadas , permitindo que invasores descubram páginas ocultas que exibem ou fornecem acesso a controles administrativos ou dados confidenciais.

``Comando:  gobuster -u <target> -w wordlist.txt dir 
-u = para indicar o site que estamos verificando 
-w = uma lista de palavras para percorrer para encontrar páginas ocultas``

![image](https://user-images.githubusercontent.com/98756562/191947478-4eb88592-1c9e-4147-b06d-720bec7952bd.png)


Você notará que o GoBuster examina o site para cada termo na lista, localizando as páginas existentes.

Na lista de nomes de páginas/diretórios , o GoBuster informará as páginas encontradas (indicadas por Status: 200 ).

**3º – Hackear o banco**

Você deve ter descoberto uma página de transferência bancária oculta ( /bank-transfer ) que permite transferir dinheiro entre contas bancárias. Na máquina, digite a página oculta no site do FakeBank.

Esta página permite que um invasor roube dinheiro de qualquer conta bancária, representando um sério risco para a organização. Como um hacker ético, você descobriria falhas em seu programa (com permissão) e as enviaria ao banco para que pudessem ser corrigidas antes que um hacker as explorasse.

[Pergunta 1.1] Depois de transferir dinheiro para sua conta, volte para a página da sua conta bancária. Qual é a resposta mostrada na sua página de saldo bancário?

Você verá a página abaixo depois de inserir o endereço IP fornecido.

![image](https://user-images.githubusercontent.com/98756562/191947730-59b9ad26-fb92-437f-ac4e-1082f5cb72cb.png)

Em seguida, vá para o “diretório oculto” que você descobriu e procure a “conta pessoal”, que é o “portal de administração” para onde você pode transferir o dinheiro.

![image](https://user-images.githubusercontent.com/98756562/191947853-f603ae8a-6460-44a2-b6bc-2391a08ba3dc.png)

![image](https://user-images.githubusercontent.com/98756562/191947872-fefafbb5-3078-4049-a782-dd68ca16a100.png)

Quando terminar, você verá "Sucesso, transferência concluída" na tela.

![image](https://user-images.githubusercontent.com/98756562/191947963-3983158b-db9b-4028-ab74-b06d1b730cc5.png)

Finalmente, quando você retornar à página principal, você verá “Funcionários do FakeBank” transferindo $ 2.000 para sua conta, seguido pelo sinalizador da pergunta.

![image](https://user-images.githubusercontent.com/98756562/191948036-b5f9a254-3116-43b1-8077-d27e16727a31.png)

Resposta: BANCO HACKEADO

[Pergunta 1.2] Se você fosse um testador de penetração ou consultor de segurança, este é um exercício que você faria para as empresas testarem vulnerabilidades em seus aplicativos da web; encontre páginas ocultas para investigar vulnerabilidades.

Resposta: Nenhuma resposta é necessária.

[Pergunta 1.3] Encerre a máquina clicando no botão vermelho “Encerrar” na parte superior da página.

Resposta: Nenhuma resposta é necessária.

![image](https://user-images.githubusercontent.com/98756562/191948086-c7d17f8a-1a8b-42a3-9e92-c7fb44b73f29.png)

Segurança ofensiva — É o processo de obter acesso não autorizado a sistemas de computador, invadindo-os , explorando defeitos de software e identificando brechas nos programas.

``Para derrotar um hacker, você deve agir como um hacker, identificando falhas e oferecendo patches antes de um cibercriminoso.``

Segurança defensiva — Por outro lado, é o ato de proteger a rede e os sistemas de computador de uma organização, avaliando e protegendo quaisquer possíveis ameaças digitais .

Você pode estar analisando sistemas ou dispositivos infectados para descobrir como eles foram invadidos , perseguindo cibercriminosos ou monitorando a infraestrutura em busca de atividades perigosas em uma posição cibernética defensiva.

[Pergunta 2.1] Leia o acima.

Resposta: Nenhuma resposta é necessária.

![image](https://user-images.githubusercontent.com/98756562/191948181-5182b872-136c-4be6-8b41-fdaf0f95fac0.png)

GRANDE PERGUNTA - Como posso começar a aprender?

As pessoas costumam perguntar como outros se tornaram hackers (consultores de segurança) ou defensores (analistas de crimes cibernéticos), e a solução é simples. Divida-o, escolha um tópico de segurança cibernética que lhe interesse e pratique com exercícios práticos regularmente. Crie o hábito de aprender algo novo no TryHackMe todos os dias e você terá as habilidades necessárias para conseguir seu primeiro emprego na área.

Que carreiras existem?

A sala de carreiras cibernéticas aprofunda as diferentes carreiras cibernéticas. No entanto, aqui está uma breve descrição de algumas funções de segurança ofensivas:

Penetration Tester — Responsável por testar produtos de tecnologia para encontrar vulnerabilidades de segurança exploráveis.
Red Teamer — Desempenha o papel de um adversário, atacando uma organização e fornecendo feedback da perspectiva de um inimigo.
Engenheiro de segurança — Projete, monitore e mantenha controles de segurança, redes e sistemas para ajudar a evitar ataques cibernéticos.
[Pergunta 3.1] Leia o acima e continue com a próxima sala!

Resposta: Nenhuma resposta é necessária.

Felicidades! ◡̈
