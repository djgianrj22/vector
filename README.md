# Vetorizador

Site estático (um único `index.html`). Converte imagens em vetor no navegador e exporta SVG, PDF e EPS (abre no CorelDRAW).

## Publicar na Vercel

**Pelo terminal**
```
cd vetorizador-vercel
npx vercel --prod
```
(Na primeira vez, faça login e aceite os padrões: sem framework, diretório raiz `./`.)

**Pelo GitHub**
1. Suba esta pasta para um repositório.
2. Em vercel.com, clique em Add New > Project e importe o repositório.
3. Framework Preset: Other. Não precisa de build command nem output directory.

## Observações
- A biblioteca ImageTracer.js é carregada por CDN (jsDelivr, com fallback para unpkg).
- PDF e EPS são gerados à mão, sem bibliotecas, com curvas vetoriais reais.
- O formato .cdr é proprietário: abra o EPS ou SVG no Corel e use Salvar como.
