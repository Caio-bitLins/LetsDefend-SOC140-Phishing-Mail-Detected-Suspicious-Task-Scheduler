![image](https://github.com/user-attachments/assets/e1af8764-a40b-417f-b4e9-b523d8d0898b)

## Let's Defend
>LetsDefend ajuda você a construir uma carreira na equipe azul com experiência prática, investigando ataques cibernéticos reais dentro de um SOC simulado.

## SOC140 - Phishing Mail Detected - Suspicious Task Scheduler

![Captura de Tela 2024-08-26 às 19 46 40](https://github.com/user-attachments/assets/70c6c77a-70f4-45af-b36b-0b2905df350c)

# Primeiro Passo 💻
Bom, nas primeiras impressões que tive sobre o caso foi:

- O Alarme foi acionado no dia **21 de março do ano de 2021 às 12:26PM**
- O endereço SMTP do e-mail é **189.162.189.159**
- Endereço de origem **aaronluo@cmail.carleton.ca**
- Endereço de destino **mark@letsdefend.io**
- O e-mail foi bloqueado antes de chegar

# Segundo Passo 💻
Analisando o e-mail é possível encontrar o hash infectado
![Captura de Tela 2024-08-27 às 18 44 37](https://github.com/user-attachments/assets/3f5fdcb1-2383-4eb8-9cb8-3ece4f4951fb)


# Terceiro Passo 🔎
Bom descobrindo o hash desse arquivo temos a opcão de analisar o arquivo em dois tipos de OSINT. A primeira é ***virus total*** e a segunda é a ***hybrid analysis.***
E na primeira suspeita o vírus total já deu como malicioso. Já no hybrid analysis deu como mesmo resultado de 100% de malware. Então não necessitou abrir uma analise mais profunda em abrir o arquivo para resolver o caso.

![Captura de Tela 2024-08-27 às 18 54 54](https://github.com/user-attachments/assets/68bc1de1-c660-4001-bd0c-707ce5ffae03)
![Captura de Tela 2024-08-27 às 19 00 29](https://github.com/user-attachments/assets/4963b7a3-7106-4d7b-8f69-5555dc25d50f)

Acrescentando outros pontos diferentes e interessantes são que:

- Jogando o SMTP no **log management** é possível encontrar o Endereço ip de destino.
- Caminhando no Endpoint security colocando o endereço ip de destino é possível encontrar as seguintes informações.
![Captura de Tela 2024-08-27 às 19 15 07](https://github.com/user-attachments/assets/56e2f48e-f741-40a7-8aad-005e6dc3c0a4)
![Captura de Tela 2024-08-27 às 19 17 07](https://github.com/user-attachments/assets/10dc701c-d78e-4d9f-baa7-efd17ce915ec)

# Último Passo 🚩
Para criar o playbook fiz o seguintes passos:

![Captura de Tela 2024-08-27 às 19 20 08](https://github.com/user-attachments/assets/941334c1-8d0a-4525-a5d5-06f6534f70c3)
![image](https://github.com/user-attachments/assets/87716569-8114-4c3c-99a2-c0b78aad8375)
![image](https://github.com/user-attachments/assets/428f9db4-0a9a-42b0-966f-a8cff7f014ae)
![Captura de Tela 2024-08-27 às 19 43 00](https://github.com/user-attachments/assets/cc5faec7-7a69-41a9-af74-17f02d3c80ad)
![Captura de Tela 2024-08-27 às 19 44 32](https://github.com/user-attachments/assets/d1608155-dd26-4aa0-aac7-17b561194062)
![Captura de Tela 2024-08-27 às 19 47 05](https://github.com/user-attachments/assets/88dd846f-c0f3-40f6-bafd-003c2a2342e0)


# Obrigado por ler até aqui! <3
<img src="https://media.tenor.com/qVKlQMB2DpsAAAAM/hacker-hacking.gif" width="230"></h2>













