# Notepad++ — Dracula Theme + VS Code Style

Personalização do Notepad++ com inspiração visual no Visual Studio Code, utilizando o tema Dracula, fontes monoespaçadas e configurações voltadas ao desenvolvimento de software.

O objetivo é proporcionar um ambiente de programação moderno, confortável e organizado, mantendo a leveza e a simplicidade do Notepad++.

---

## 1. Tema Dracula

O [Dracula Theme](https://draculatheme.com/) é um tema escuro bastante utilizado em editores de código e ferramentas de desenvolvimento.

Sua paleta combina fundo escuro, cores vibrantes e bom contraste, proporcionando uma experiência visual agradável durante longas sessões de programação.

### Instalação do tema

**Passo 1 — Baixar o tema**

Acesse o repositório oficial:

[Dracula Theme — Notepad++](https://github.com/dracula/notepad-plus-plus)

Também é possível baixar diretamente o arquivo:

[Dracula.xml — Download](https://raw.githubusercontent.com/dracula/notepad-plus-plus/main/generated/Dracula.xml)

**Passo 2 — Localizar a pasta de temas**

Pressione `Win + R` e digite:

```text
%AppData%\Notepad++\themes
```

Se a pasta `themes` não existir, crie-a manualmente.

**Passo 3 — Instalar o tema**

Copie o arquivo `Dracula.xml` para dentro da pasta `themes`.

A estrutura deverá ficar assim:

```text
Notepad++
│
├── config.xml
├── stylers.xml
├── stylers.model.xml
├── shortcuts.xml
│
└── themes
    └── Dracula.xml
```

**Passo 4 — Ativar o tema**

Abra o Notepad++ e acesse:

```text
Settings
   └── Style Configurator
         └── Select Theme
               └── Dracula
```

Selecione `Dracula` e clique em **Save & Close**.

Reinicie o Notepad++ caso as alterações não sejam aplicadas imediatamente.

---

## 2. Fontes recomendadas

A escolha da fonte influencia diretamente a legibilidade do código e o conforto durante a programação.

Considerando o desenvolvimento com PHP, JavaScript, TypeScript, HTML, CSS e Python, estas são as recomendações:

| Fonte | Recomendação |
|---|---|
| Bitstream Vera Sans Mono | Boa |
| Consolas | Muito boa |
| Cascadia Code | Excelente |
| JetBrains Mono | Excelente |

### Minhas recomendações

**JetBrains Mono**

Minha principal recomendação. Desenvolvida para programação, possui excelente legibilidade e caracteres bem diferenciados.

Download: https://www.jetbrains.com/lp/mono/

**Cascadia Code**

Fonte desenvolvida pela Microsoft, com aparência moderna e excelente integração visual com o ecossistema Windows.

Download: https://github.com/microsoft/cascadia-code

**Consolas**

Uma opção clássica, leve e bastante confortável para desenvolvimento.

### Configuração recomendada

| Propriedade | Configuração |
|---|---|
| Fonte | JetBrains Mono |
| Tamanho | 11 ou 12 pt |
| Estilo | Regular |
| Ligaduras | Desativadas |
| Indentação | 4 espaços |
| Codificação | UTF-8 |

Para configurar, acesse:

```text
Settings → Style Configurator → Global Styles
```

Selecione `Default Style` e escolha a fonte desejada.

---

## 3. Paleta de cores Dracula

A paleta Dracula é composta por cores que diferenciam elementos do código sem comprometer a leitura.

| Elemento | Cor | Código HEX |
|---|---|---|
| Background | Fundo principal | `#282A36` |
| Current Line | Linha atual | `#44475A` |
| Foreground | Texto principal | `#F8F8F2` |
| Comment | Comentários | `#6272A4` |
| Cyan | Propriedades e tipos | `#8BE9FD` |
| Green | Variáveis e funções | `#50FA7B` |
| Orange | Destaques | `#FFB86C` |
| Pink | Palavras-chave | `#FF79C6` |
| Purple | Números | `#BD93F9` |
| Yellow | Strings | `#F1FA8C` |
| Red | Alertas e erros | `#FF5555` |

### Exemplo visual da paleta

| Cor | Visualização |
|---|---|
| Background | <span style="color:#282A36">`#282A36`</span> |
| Foreground | `#F8F8F2` |
| Comment | `#6272A4` |
| Cyan | `#8BE9FD` |
| Green | `#50FA7B` |
| Orange | `#FFB86C` |
| Pink | `#FF79C6` |
| Purple | `#BD93F9` |
| Yellow | `#F1FA8C` |
| Red | `#FF5555` |

---

## 4. Arquivos de configuração

O Notepad++ utiliza diferentes arquivos para armazenar preferências, estilos e atalhos.

| Arquivo | Responsabilidade |
|---|---|
| `config.xml` | Preferências gerais e interface |
| `stylers.xml` | Estilos e configurações de cores |
| `stylers.model.xml` | Modelo de estilos |
| `shortcuts.xml` | Atalhos personalizados |
| `Dracula.xml` | Tema visual Dracula |

### 4.1. Como instalar o config.xml

O arquivo `config.xml` armazena diversas preferências do Notepad++, como configurações da interface e comportamento do editor.

**Instalação:**

1. Feche completamente o Notepad++.
2. Pressione `Win + R`.
3. Digite:

```text
%AppData%\Notepad++
```

4. Faça uma cópia de segurança do `config.xml` original.
5. Copie o novo arquivo para essa pasta.
6. Abra novamente o Notepad++.

**Importante:** não utilize um `config.xml` genérico sem verificar sua compatibilidade com a versão instalada. O arquivo pode conter configurações específicas da instalação, plugins e preferências pessoais.

### 4.2. Como instalar o stylers.xml

O arquivo `stylers.xml` armazena configurações de estilos do editor e de seus componentes.

**Instalação:**

1. Feche o Notepad++.
2. Acesse `%AppData%\Notepad++`.
3. Faça backup do `stylers.xml` existente.
4. Substitua-o somente por um arquivo compatível com sua versão.
5. Abra novamente o programa.

**Atenção:** o arquivo `stylers.model.xml` não deve ser confundido com o arquivo de estilos efetivamente utilizado. Alterar o modelo não significa necessariamente alterar a aparência do editor.

Para utilizar o Dracula, prefira instalar o arquivo oficial `Dracula.xml` na pasta `themes` e ativá-lo pelo Style Configurator. Não é necessário substituir manualmente todos os estilos.

### 4.3. Como instalar o shortcuts.xml

Esse arquivo armazena os atalhos personalizados do Notepad++.

Localização:

```text
%AppData%\Notepad++\shortcuts.xml
```

Faça backup antes de substituir o arquivo, pois você pode perder atalhos personalizados.

---

## 5. Configurações recomendadas do editor

Para aproximar a experiência do VS Code, recomendo as seguintes configurações:

| Recurso | Configuração |
|---|---|
| Tema | Dracula |
| Modo escuro | Ativado |
| Numeração de linhas | Ativada |
| Destaque da linha atual | Ativado |
| Indentação automática | Ativada |
| Quebra automática de linha | Ativada |
| Autocompletar | Ativado |
| Barra de status | Visível |
| Abas | Ativadas |
| Codificação padrão | UTF-8 |
| Largura de indentação | 4 espaços |

---

## 6. Plugins recomendados

Acesse `Plugins → Plugins Admin` para pesquisar e instalar os plugins disponíveis.

| Plugin | Funcionalidade |
|---|---|
| Explorer | Navegação por arquivos |
| ComparePlus | Comparação de arquivos |
| JSON Viewer | Formatação e visualização de JSON |
| XML Tools | Formatação e validação XML |
| NppFTP | Transferência de arquivos por FTP/SFTP |

A disponibilidade pode variar conforme a versão e a arquitetura do Notepad++.

---

## 7. Atalhos úteis

| Atalho | Função |
|---|---|
| `Ctrl + N` | Novo arquivo |
| `Ctrl + O` | Abrir arquivo |
| `Ctrl + S` | Salvar |
| `Ctrl + Shift + S` | Salvar como |
| `Ctrl + F` | Localizar |
| `Ctrl + H` | Substituir |
| `Ctrl + Tab` | Próxima aba |
| `Ctrl + Shift + Tab` | Aba anterior |
| `Ctrl + D` | Duplicar linha ou seleção |
| `Ctrl + G` | Ir para linha |

---

## 8. Estrutura final

Após a personalização, a estrutura esperada dos arquivos será:

```text
%AppData%\Notepad++
│
├── config.xml
├── stylers.xml
├── stylers.model.xml
├── shortcuts.xml
│
├── themes/
│   └── Dracula.xml
│
└── plugins/
    └── Config/
        └── NppFTP/
```

Os arquivos de plugins serão criados conforme as extensões instaladas.

---

## 9. Referências oficiais

- Dracula Theme: https://draculatheme.com/
- Dracula para Notepad++: https://github.com/dracula/notepad-plus-plus
- Notepad++: https://notepad-plus-plus.org/
- Manual do Notepad++: https://npp-user-manual.org/
- JetBrains Mono: https://www.jetbrains.com/lp/mono/
- Cascadia Code: https://github.com/microsoft/cascadia-code

---

**Projeto:** Notepad++ — Dracula + VS Code Style

**Objetivo:** proporcionar uma experiência visual moderna, organizada e confortável para desenvolvimento de software, preservando a leveza do Notepad++.
