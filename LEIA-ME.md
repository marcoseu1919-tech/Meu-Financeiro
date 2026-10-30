# Meu financeiro

App de finanças pessoais (preto e amarelo): lançamentos, metas, contas a pagar e fluxograma do saldo.

## Como transformar em app (APK) usando só o site do GitHub

1. Extraia este zip no seu computador.
2. No GitHub, crie um repositório novo (botão **New**).
3. Dentro do repositório: **Add file → Upload files** e arraste TODO o conteúdo extraído
   (pasta `www`, pasta `.github`, `package.json`, `capacitor.config.json`, etc.). Depois clique em **Commit changes**.
   - Se a pasta `.github` não aparecer para arrastar (pastas com ponto ficam ocultas em alguns sistemas):
     use **Add file → Create new file**, digite no nome `.github/workflows/build-apk.yml`
     e cole o conteúdo do arquivo `build-apk.yml` deste zip. Depois **Commit changes**.
4. Abra a aba **Actions**. O fluxo **Gerar APK** roda sozinho (leva uns 5 a 10 minutos).
   Se não rodar, clique em **Gerar APK → Run workflow**.
5. Quando ficar com o ícone verde, abra a execução e, em **Artifacts**, baixe **meu-financeiro-apk**.
6. Extraia o zip baixado: dentro está o `app-debug.apk`. Passe para o celular Android e instale
   (o Android vai pedir para permitir instalação de fontes desconhecidas).

Se o fluxo falhar (ícone vermelho), abra a execução, copie o texto do erro e envie para quem está te ajudando.

Os dados do app ficam salvos no próprio aparelho.
