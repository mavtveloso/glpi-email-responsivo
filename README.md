# glpi-email-responsivo
### Um código html para melhorar a aparência do e-mail responsivo do sistema de chamado <a href="https://glpi-project.org/">Glpi</a>.

## Sobre:
Editei o código _"Modelo de notificações"_ original do Glpi para facilitar a leitura/interação do e-mail pelo usuario. No caso da empresa onde utilizo o Glpi somente os técnicos possuem login e senha para acessar o sistema de chamado. Toda a interação como: abertura de chamado, acompanhamentos e solicitações é feita pelo usuário _(colaboradores de outros departamentos diferente do TI)_ através do e-mail. Então foi necessário simplificar e deixar a aparência das respostas mais agradável, para facilitar a leitura e interação do chamado.

## Antes _x_ Depois
<img src="https://user-images.githubusercontent.com/29666972/173641410-7c1cbf08-c6d4-4348-a04e-df0fcef03a1a.jpg" alt="antes" width="450px" /> <img src="https://user-images.githubusercontent.com/29666972/173640302-68b25a5b-8a95-48b0-99cc-1836f13ef7e3.jpg" alt="depois" width="380px" style="border:5px " />

O código ficou mais limpo, intuitivo e mais fácil de dar manutenção.

# Como alterar:
## Tradução de modelo

* No painel superior coloque o mouse em cima da aba **Configurar** > clique em **Notificações** > **Modelos de Notificações** > Filtre por _Tickets_ > Clique no item **"Tickets"**
<img src="https://user-images.githubusercontent.com/29666972/173658652-82220609-e775-473a-8bff-7ee67d80715f.jpg" alt="passo1" height="400px"/>

* Em **"Modelo de notificação"**. No campo **"Type"** preencha como Chamado e no campo **CSS** pode deixar em branco. **Salve**.

![image](https://user-images.githubusercontent.com/29666972/173659412-e99f58c0-cf14-46a5-9f0e-7e5f5b1d43de.png)

* No painel de opções na lateral esquerda da tela clique em **"Traduções de modelo"** > Entre em **"Tradução padrão"** ou caso não tenha tradução clique em "Adicionar uma nova tradução".

![image](https://user-images.githubusercontent.com/29666972/173659817-32248f5e-26ba-40d3-8957-effd27d3114f.png)

## Alterando as configurações da "Tradução do modelo":
* Em **idioma**, deixe sem nenhum idioma de tradução marcando a opção "-----".
* O campo **Assunto** vai ser sempre o assunto do e-mail que o Glpi vai retornar a cada acompanhamento ou chamado novo. Nesse campo preencha com ##ticket.action## ##ticket.title## .
* No campo **corpo do texto do e-mail** apague tudo e deixe em branco.
* Na barra de opçoes para formatação do texto clique no ícone "**< >**" (Código fonte). **_OBS.:Faça um backup desse código fonte para futuras manuteções ou correções._**
* Apague todo o código fonte e cole o código .html do arquivo <a href="https://github.com/mavtveloso/glpi-email-responsivo/blob/main/templateEmailGlpiResponsivo.txt">templateEmailGlpiResponsivo.txt</a> . **_OBS.: Susbtitua o endereço do seu Glpi nos campos (SEU ENDEREÇO) do código, para trazer as marcas d'agua dentro das caixas de diálogo._**

<img src="https://user-images.githubusercontent.com/29666972/173665429-4d13fa7f-5dfb-44a1-bbca-97d06bf21118.png" alt="print" width="600px"/> <img src="https://user-images.githubusercontent.com/29666972/173666553-c70301cf-66e7-4aba-976e-54a570bfc76d.png" alt="print2" width="350px"/>

* Clique em **OK** e depois em **Salvar** na parte inferior da página.

# Conclusão
A alteração da tradução de modelo está feita ✅. Agora é só enviar e receber alguns acompanhamentos nos chamados para testar as respostas por e-mail 😉.
