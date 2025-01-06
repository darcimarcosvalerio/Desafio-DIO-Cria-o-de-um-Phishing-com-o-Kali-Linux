# Desafio DIO Criaco de um Phishing no Kali Linux com SEToolkit 
Passo a Passo: Criação de um Phishing com Kali Linux
Ferramentas Necessárias
1.	Kali Linux (sistema operacional voltado para testes de penetração).
2.	SEToolkit (Social-Engineer Toolkit, uma ferramenta para testes de engenharia social).
________________________________________
Passo 1: Acessando o Kali Linux
1.	Certifique-se de estar no Kali Linux. Se não estiver, inicialize-o.
2.	Abra o terminal no Kali Linux.
________________________________________
Passo 2: Obtenha acesso root
O SEToolkit exige privilégios de administrador.
┌──(aluno㉿kali)-[~]
└─$ sudo su
Digite a senha do administrador e pressione Enter.
 
________________________________________
Passo 3: Inicie o SEToolkit
Execute o comando abaixo para iniciar o SEToolkit:
┌──(root㉿kali)-[~]
└─# setoolkit

...

Do you agree to the terms of service [y/n]: y


O menu inicial do SEToolkit será exibido.
 
________________________________________
Passo 4: Configure o Phishing
1.	Escolha Social-Engineering Attacks digitando o número correspondente no menu e pressionando Enter.
 
2.	No próximo menu, escolha Web Site Attack Vectors.
 
3.	Selecione a opção Credential Harvester Attack Method.
 
4.	Escolha Site Cloner como método de ataque.
 
________________________________________
Passo 5: Configure o endereço IP
1.	No terminal, digite o comando abaixo para identificar o IP da máquina:
ifconfig
 
________________________________________
Passo 6: Clone o site do Facebook
1.	Quando solicitado pelo SEToolkit, insira o URL do site que deseja clonar.
No caso, use: http://www.facebook.com
 
2.	O SEToolkit criará uma réplica do site do Facebook na sua máquina.
 
________________________________________
Passo 7: Teste o Phishing
1.	Distribua o endereço IP gerado no formato http://www.facebook.compara as vítimas em um ambiente autorizado (simulado, como um laboratório).
2.	Quando a vítima acessar e inserir suas credenciais, o SEToolkit capturará os dados de login.
________________________________________
Passo 8: Verifique os resultados
1.	No terminal do Kali Linux, observe os dados capturados no console do SEToolkit.
2.	As informações inseridas pelas vítimas, como e-mails e senhas, aparecerão no terminal.
________________________________________
Restrições Éticas
•	Esse projeto deve ser realizado somente em um ambiente controlado.
•	Não use ferramentas de phishing para atividades ilegais.
•	Considere alternativas éticas, como testes de segurança em sistemas próprios.
________________________________________
Código Referenciado
O arquivo com os comandos detalhados pode ser acessado no GitHub:
GitHub - Cibersecurity Desafio Phishing

