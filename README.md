# Plugin FollowUser para Vencord

## 📝 Descrição
Este plugin permite que você "siga" outros usuários em canais de voz no Discord. Quando você segue um usuário, o plugin automaticamente o move para o mesmo canal de voz que o usuário seguido quando ele muda de canal.

## ✨ Funcionalidades
- Adiciona uma opção "Seguir Usuário" no menu de contexto do usuário
- Mostra um indicador na barra de ferramentas quando você está seguindo alguém
- Automaticamente o move para o mesmo canal de voz que o usuário seguido
- Opção para desconectar quando o usuário seguido sai do canal de voz
- Opção para voltar automaticamente ao canal do usuário seguido se você for movido
- Tenta entrar no canal quando ele não estiver mais cheio

## 🚀 Como Usar
1. Clique com o botão direito em um usuário
2. Selecione "Seguir Usuário" no menu
3. Um ícone aparecerá na barra de ferramentas indicando que você está seguindo o usuário
4. Para parar de seguir, clique com o botão direito no ícone ou selecione "Deixar de Seguir Usuário" no menu de contexto

## ⚙️ Configurações
| Configuração | Descrição |
|-------------|-----------|
| **Entrar no mesmo canal ao seguir** | Automaticamente entra no canal de voz do usuário quando você começa a segui-lo |
| **Apenas ativar manualmente** | Só segue o usuário quando você clica no indicador, não automaticamente |
| **Sair quando o usuário sair** | Desconecta você do canal de voz quando o usuário seguido sair |
| **Voltar automaticamente** | Se você for movido para outro canal, volta automaticamente para o canal do usuário seguido |
| **Tentar entrar quando o canal não estiver cheio** | Se o canal estiver cheio, tenta entrar quando houver espaço |

## 🛠️ Instalação
### Instalando o Vencord
⚠️ **IMPORTANTE:** O Vencord deve ser instalado manualmente na pasta `Documentos`. Não use a versão instalada por executável!

Se você ainda não tem o Vencord instalado, siga estas etapas:
1. Instale as dependências necessárias:
   - [Baixe e instale o Git](https://git-scm.com/downloads)
   - [Baixe e instale o Node.js](https://nodejs.org/)
   - [Baixe e instale o pnpm](https://pnpm.io/installation)
   - Certifique-se de que todos estão adicionados ao PATH do sistema.

2. Para verificar a instalação, execute os seguintes comandos no terminal:
   ```sh
   git --version
   node --version
   pnpm --version
   ```
   Se todos retornarem uma versão válida, a instalação foi bem-sucedida.

3. Clone o repositório do Vencord dentro da pasta `Documentos`:
   ```sh
   cd Documentos
   git clone https://github.com/Vendicated/Vencord
   ```

4. Acesse a pasta clonada:
   ```sh
   cd Vencord
   ```

5. Instale as dependências:
   ```sh
   pnpm install --frozen-lockfile
   ```

6. Compile o Vencord:
   ```sh
   pnpm build
   ```

7. Injete o Vencord no Discord:
   ```sh
   pnpm inject
   ```

### Instalando o Plugin FollowUser
1. **Abra a pasta de plugins do Vencord:**
   - No Discord, vá para as configurações do Vencord
   - Clique em **Plugins** e depois em **Abrir pasta de plugins**

2. **Baixe o código do plugin:**
   - Crie uma pasta chamada `FollowUser`
   - Coloque o arquivo `index.tsx` dentro da pasta `FollowUser`

3. **Ative o plugin:**
   - Volte para as configurações do Vencord
   - Na aba **Plugins**, ative o **FollowUser**

### Instalando Plugins Personalizados
Se quiser adicionar plugins personalizados ao Vencord:
1. Acesse a pasta do Vencord e crie uma nova pasta para plugins personalizados:
   ```sh
   cd Vencord/src
   mkdir userplugins
   ```

2. Adicione seu plugin dentro da pasta `userplugins`. Ele pode ser um arquivo único (`meuPlugin.tsx`) ou uma pasta com um arquivo `index.tsx`.
   ```sh
   mv meuPlugin.tsx Vencord/src/userplugins/
   ```

3. Para aplicar as mudanças, reconstrua o Vencord:
   ```sh
   pnpm build
   ```

## 📝 Licença
Este plugin é parte do Vencord e está licenciado sob GPL-3.0-or-later.

---

Criado com ❤️ por **guihzzy**

