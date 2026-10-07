# Hackathon do Projeção 2026 (Edição Halloween)

Site de divulgação do Hackathon do Projeção: 30/10/2026, a partir das 08:00.

## Estrutura

```
index.html        página completa (HTML, CSS e JS num único arquivo)
assets/chamada.jpg  arte oficial do evento
assets/og.jpg       imagem de prévia para WhatsApp/redes sociais
.nojekyll           faz o GitHub Pages servir os arquivos como estão
```

## Colocar o link do formulário

Abra `index.html`, procure por `FORM_URL` (perto do final) e cole o link:

```js
const FORM_URL = "https://forms.gle/SEU-LINK-AQUI";
```

Todos os botões "Inscreva-se" passam a abrir o formulário em nova aba.
Enquanto o link estiver vazio, os botões mostram o aviso "As inscrições abrem em breve".

## Publicar no GitHub Pages

1. Crie um repositório no GitHub (ex.: `hackathon-projecao`).
2. Envie todos os arquivos desta pasta para a raiz do repositório.
3. Vá em **Settings > Pages**.
4. Em **Source**, escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`, e salve.
5. Em 1 ou 2 minutos o site estará em `https://SEU-USUARIO.github.io/hackathon-projecao/`.

Pelo terminal:

```bash
git init
git add .
git commit -m "Site do Hackathon do Projeção"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/hackathon-projecao.git
git push -u origin main
```

## Ajustes rápidos

- Data/hora da contagem regressiva: `EVENT_DATE` no `index.html`.
- Cores: variáveis no início do `<style>` (`--orange`, `--green`, `--cyan`...).
- Prêmios: seção `id="premiacao"`.
