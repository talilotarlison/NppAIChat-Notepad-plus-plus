# Instalação do NppAIChat

Este guia explica como instalar o plugin NppAIChat no Notepad++ usando o pacote disponibilizado neste repositório.

## Requisitos

- Windows e uma versão compatível do Notepad++.
- O pacote [`NppAIChat_v1.0.0.zip`](../NppAIChat_v1.0.0.zip).
- Acesso à internet e uma chave de API válida do provedor de IA que você pretende usar.

## Passo a passo

1. **Feche o Notepad++.** Isso evita que arquivos do plugin estejam em uso durante a instalação.
2. **Baixe o pacote do plugin.** Na página do repositório, abra `NppAIChat_v1.0.0.zip` e faça o download.
3. **Extraia o arquivo ZIP** para uma pasta temporária. Não copie o ZIP sem descompactar.
4. **Localize a pasta de plugins do Notepad++.** Em uma instalação padrão do Windows, ela fica em:
   - `C:\Program Files\Notepad++\plugins` (instalação de 64 bits); ou
   - `C:\Program Files (x86)\Notepad++\plugins` (instalação de 32 bits).

   Se o Notepad++ estiver instalado em outro local, procure a pasta `plugins` dentro da pasta de instalação correspondente.
5. **Copie a pasta do NppAIChat** extraída para dentro da pasta `plugins`. A estrutura deve ficar semelhante a esta:

   ```text
   Notepad++/
   └── plugins/
       └── NppAIChat/
           └── ... arquivos do plugin ...
   ```

   Se o ZIP já tiver uma pasta `NppAIChat`, copie essa pasta. Evite criar uma pasta duplicada como `plugins/NppAIChat/NppAIChat/`, a menos que essa seja a estrutura que o pacote já fornece.
6. **Autorize a cópia**, se o Windows pedir permissão de administrador para gravar na pasta de instalação.
7. **Abra novamente o Notepad++.** Procure o NppAIChat no menu **Plugins**. Se não aparecer, confira se a pasta foi copiada para a instalação correta e se a arquitetura do plugin é compatível com a do Notepad++.
8. **Abra o painel do chat** pelo menu do plugin e configure o provedor, o modelo e a chave de API solicitados. A configuração necessária depende do serviço de IA escolhido; consulte o [manual do projeto](Handbook.md).
9. **Teste a instalação** enviando uma mensagem no chat. Para usar um serviço online, confirme que há conexão com a internet e que a chave de API é válida.

## Segurança da chave de API

Trate sua chave de API como uma senha: não a compartilhe nem a publique em arquivos, capturas de tela ou repositórios. O uso da API pode estar sujeito às tarifas e aos limites definidos pelo provedor.

## Solução de problemas

- **O plugin não aparece no menu Plugins:** confirme que a pasta `NppAIChat` está dentro da pasta `plugins` da mesma instalação do Notepad++ que você abriu. Verifique também se não foi criada uma pasta duplicada.
- **Não é possível copiar os arquivos:** feche o Notepad++ e tente novamente com as permissões necessárias.
- **O plugin aparece, mas a solicitação falha:** verifique a conexão, a URL/modelo configurados e a validade da chave de API.
- **O plugin não carrega:** confira a compatibilidade entre a arquitetura do plugin e a versão do Notepad++ instalada.
