# PedreiraFlix para TV

Site simples para baixar e instalar o `app.apk` (PedreiraFlix) direto pelo navegador da Smart TV (Android TV, Google TV ou Fire TV). A página foi feita para usar com o controle remoto: o botão de download já começa focado, então basta apertar **OK**.

## Arquivos

| Arquivo      | Para que serve                                    |
|--------------|---------------------------------------------------|
| `index.html` | Página principal (botão de download + passo a passo) |
| `style.css`  | Visual para TV: textos grandes, alto contraste, foco visível |
| `app.apk`    | O instalador (PedreiraFlix 1.4)                    |
| `README.md`  | Este guia                                          |

## Testar no computador

Abra o `index.html` no navegador. Use **Tab** e **Enter** para simular o controle remoto.

## Publicar grátis no GitHub Pages

1. Crie um repositório público no GitHub (ex: `instalar-tv`).
2. Envie os arquivos:

   ```bash
   git init
   git add index.html style.css app.apk README.md
   git commit -m "Site de instalação do PedreiraFlix"
   git branch -M main
   git remote add origin https://github.com/SEU_USUARIO/instalar-tv.git
   git push -u origin main
   ```

3. No repositório, vá em **Settings > Pages**.
4. Em *Build and deployment*, escolha **Deploy from a branch**, branch **main** e pasta **/(root)**. Clique em **Save**.
5. Em 1 a 2 minutos o site fica no ar em:
   `https://SEU_USUARIO.github.io/instalar-tv/`

Digite esse endereço no navegador da TV.

> **Dica:** o endereço é longo para digitar com o controle. Use um encurtador (ex: bit.ly) e digite só o link curto.

## Instalar na TV

1. Abra o endereço no navegador da TV e aperte **OK** em **Baixar APK**.
2. Se a TV pedir, permita que o navegador (ou o gerenciador de arquivos) **instale apps desconhecidos**:
   - **Android TV / Google TV:** Configurações > Apps > Segurança e restrições > Fontes desconhecidas (ou *Instalar apps desconhecidos*).
   - **Fire TV:** Configurações > Minha Fire TV > Opções do desenvolvedor > Instalar apps desconhecidos.
3. Abra o arquivo baixado e confirme **Instalar**.

**A TV não tem navegador?** Instale o app **Downloader** (AFTVnews) pela loja da TV, digite o endereço do site nele e baixe por lá.

## Atualizar o APK

Substitua o `app.apk` pela versão nova (mantendo o nome), atualize a versão e o tamanho no `index.html` e faça commit + push. O GitHub Pages republica sozinho.
