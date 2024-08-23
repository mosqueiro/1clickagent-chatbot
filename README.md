
# Chatbot | 1Click Agent

Este é um projeto de chatbot simples desenvolvido com HTML, CSS e JavaScript, que se conecta a uma API usando um `agentID` específico. O projeto permite que o chatbot exiba sugestões e responda a perguntas feitas pelo usuário, interpretando markdown nas respostas e renderizando-o corretamente como HTML.

## Funcionalidades

- **Integração com a API**: Conecta-se a uma API externa usando um `agentID`.
- **Suporte a Markdown**: Interpreta e renderiza markdown básico como negrito, itálico e links.
- **Persistência de Conversa**: Salva e restaura o histórico de conversa usando o `localStorage`.
- **Temas**: Suporte para temas claro e escuro, com capacidade de alternar entre eles.
- **Respostas com Efeito de Digitação**: As respostas do chatbot são exibidas com um efeito de digitação para melhorar a experiência do usuário.

## Como Usar

1. **Clone o Repositório**

   Primeiro, clone o repositório para o seu ambiente local:

   ```bash
   git clone https://github.com/mosqueiro/1clickagent-chatbot
   ```

   Ou faça download do código diretamente : [Download](https://github.com/mosqueiro/1clickagent-chatbot/archive/refs/heads/main.zip)

2. **Obtenha o `agentID`**

   Acesse [1Click Agent](http://1clickagent.ai) e obtenha o `agentID` específico para o seu chatbot. Este `agentID` é necessário para que o chatbot se conecte à API correta.

3. **Atualize o `agentID` no HTML**

   No arquivo `index.html`, localize a seguinte linha de código:

   ```html
   <div class="chat-list" data-agent-id="f40715ce-963b-4ddd-b599-2bf234bb63c4"></div>
   ```

   Substitua o `agentID` (`f40715ce-963b-4ddd-b599-2bf234bb63c4`) pelo `agentID` que você obteve da plataforma. Certifique-se de que o `agentID` seja válido para que o chatbot funcione corretamente.

4. **Inicie um Servidor Local (Opcional)**

   Para testar o projeto localmente, é recomendável usar um servidor local. Se estiver utilizando o Visual Studio Code, você pode usar a extensão **Live Server**.

5. **Personalize o `data.json`**

   No arquivo `data.json`, você pode personalizar o conteúdo exibido no chatbot, incluindo o título, subtítulo, sugestões e aviso de isenção de responsabilidade.

6. **Execute o Projeto**

   Abra o arquivo `index.html` no navegador. O chatbot estará pronto para uso.

## Dependências

Este projeto não possui dependências externas. Toda a lógica de markdown e exibição está embutida no JavaScript incluído.

## Licença

Este projeto está licenciado sob a licença MIT. Consulte o arquivo `LICENSE` para mais informações.
