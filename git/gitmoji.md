# Gitmoji

# **Manual de Instalação e Uso do Gitmoji-CLI**

Este manual fornece instruções detalhadas para instalar e usar o Gitmoji-CLI, uma ferramenta que permite adicionar emojis às mensagens de commit do Git, tornando-as mais informativas e visuais.

## **Passo 1: Instalar o Gitmoji-CLI**

### **Opção 1: Usando npm**

1. **Verificar Node.js**:
    - Abra o terminal e digite:
        
        ```
        node -v
        ```
        
    - Se o Node.js estiver instalado, você verá a versão instalada. Caso contrário, instale-o a partir do site oficial [Node.js](https://nodejs.org/).
2. **Verificar npm**:
    - No terminal, digite:
        
        ```
        npm -v
        ```
        
    - Se o npm estiver instalado, você verá a versão instalada. Caso contrário, ele será instalado automaticamente com o Node.js.
3. **Instalar Gitmoji-CLI**:
    - No terminal, execute o comando:
        
        ```
        npm install -g gitmoji-cli
        ```
        

### **Opção 2: Usando Homebrew (Indicado para quem usa Mac)**

1. **Instalar Homebrew** (se ainda não estiver instalado):
    - Abra o terminal e execute o seguinte comando:
        
        ```bash
        /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
        ```
        
    - Após a instalação, adicione o Homebrew ao seu PATH conforme instruções fornecidas pelo instalador.
2. **Instalar Gitmoji-CLI com Homebrew**:
    - No terminal, execute o comando:
        
        ```bash
        brew install gitmoji
        ```
        

---

## **Passo 3: Configurar Gitmoji-CLI**

1. **Configuração Inicial**:
    - No terminal, execute:
        
        ```css
        gitmoji -i
        ```
        
    - Isso inicializa o gitmoji-CLI para ser usado em seu repositório.

---

## **Passo 4: Fazer um Commit com Gitmoji**

1. **Adicionar Arquivos ao Staging**:
    - No terminal, adicione os arquivos que deseja commitar:
        
        ```csharp
        git add <caminho_do_arquivo>
        ```
        
2. **Fazer o Commit com Gitmoji**:
    - Execute o comando para iniciar o processo de commit com Gitmoji:
        
        ```r
        gitmoji -c
        ```
        
    - Você verá um menu interativo onde pode escolher o emoji que representa a alteração que está sendo feita. Use as setas do teclado para navegar e pressione Enter para selecionar.
    - Após selecionar o emoji, você será solicitado a adicionar uma mensagem de commit. Escreva uma mensagem descritiva e pressione Enter.

---

## **Passo 5: Push do Commit para o Repositório Remoto**

1. **Enviar Commit para o Repositório Remoto**:
    - Execute o comando:
        
        ```perl
        git push origin <nome-da-branch>
        ```
        
    - Substitua `<nome-da-branch>` pelo nome da branch em que você está trabalhando.

---

### **Exemplo Completo**

Vamos ilustrar com um exemplo completo:

1. **Verificar Node.js e npm**:
    
    ```bash
    node -v
    npm -v
    ```
    
2. **Instalar Gitmoji-CLI**:
    - Com npm:
        
        ```bash
        npm install -g gitmoji-cli
        ```
        
    - Com Homebrew:
        
        ```bash
        brew install gitmoji
        ```
        
3. **Adicionar Arquivos ao Staging**:
    
    ```bash
    git add <nome_do_arquivo>
    ```
    
4. **Commit com Gitmoji**:
    
    ```bash
    gitmoji -c
    ```
    
    - Selecione o emoji correspondente (por exemplo, `🐛` para correção de bug).
    - Adicione uma mensagem descritiva (por exemplo, "Corrigido erro no cálculo de descontos").
5. **Push do Commit**:
    
    ```bash
    git push origin main
    ```
    
    - Substitua `main` pelo nome da sua branch, se for diferente.