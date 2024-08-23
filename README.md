
# Chatbot | 1Click Agent

![agentID](https://i.imgur.com/JDYlKTA.png)

Este é um projeto de chatbot desenvolvido com HTML, CSS e JavaScript, que se conecta a uma API da 1ClickAgent usando um `agentID` específico. O projeto permite que o chatbot exiba sugestões e responda a perguntas feitas pelo usuário, interpretando markdown nas respostas e renderizando-o corretamente como HTML.

## Como Usar

1. **Clone o Repositório**

   Primeiro, clone o repositório para o seu ambiente local:

   ```bash
   git clone https://github.com/mosqueiro/1clickagent-chatbot
   ```

   Ou faça download do código diretamente : [Download](https://github.com/mosqueiro/1clickagent-chatbot/archive/refs/heads/main.zip)

2. **Obtenha o `agentID`**

   Acesse [1Click Agent](http://1clickagent.ai) e obtenha o `agentID` específico para o seu chatbot. Este `agentID` é necessário para que o chatbot se conecte à API correta.

   ![agentID](https://i.imgur.com/JzFEbC5.png)

4. **Atualize o `agentID` no HTML**

   No arquivo `index.html`, localize a seguinte linha de código:

   ```html
   <div class="chat-list" data-agent-id="f40715ce-963b-4ddd-b599-2bf234bb63c4"></div>
   ```

   Substitua o `agentID` (`f40715ce-963b-4ddd-b599-2bf234bb63c4`) pelo `agentID` que você obteve da plataforma. Certifique-se de que o `agentID` seja válido para que o chatbot funcione corretamente. (não é necessário conectar no WhatsApp para que seu chatbot funcione)

5. **Inicie um Servidor Local (Opcional)**

   Para testar o projeto localmente, é recomendável usar um servidor local. Se estiver utilizando o Visual Studio Code, você pode usar a extensão **Live Server**.

6. **Hospede o Código no Seu Servidor (Opcional)**

   Se preferir, você pode hospedar o código no seu próprio servidor, por exemplo, em um subdomínio como `chat.seudominio.com`. Isso permitirá que o chatbot esteja acessível online e possa ser utilizado por qualquer usuário diretamente pelo navegador.

7. **Personalize o `data.json`**

   No arquivo `data.json`, você pode personalizar o conteúdo exibido no chatbot, incluindo o título, subtítulo, sugestões e aviso de isenção de responsabilidade.

```json
{
   "title": "Olá, tudo bem!",
   "subtitle": "Como posso ajudar hoje?",
   "pageTitle": "Chatbot | Assistente iFood",
   "disclaimer": "O Assistente iFood pode exibir informações imprecisas, incluindo sobre pessoas, portanto, verifique suas respostas.",
   "suggestions": [
      {
         "text": "Quais são as melhores opções de restaurantes próximos a mim?",
         "icon": "restaurant"
      },
      {
         "text": "Como posso usar cupons de desconto no iFood?",
         "icon": "local_offer"
      },
      {
         "text": "Qual é o tempo estimado de entrega do meu pedido?",
         "icon": "timer"
      },
      {
         "text": "Como posso rastrear o meu pedido no iFood?",
         "icon": "map"
      }
   ]
}
```

9. **Execute o Projeto**

   Abra o arquivo `index.html` no navegador. O chatbot estará pronto para uso.

## Dependências

Este projeto não possui dependências externas. Toda a lógica de markdown e exibição está embutida no JavaScript incluído.

## Licença

Este projeto está licenciado sob a licença MIT. Consulte o arquivo `LICENSE` para mais informações.
