# Zelo | Landing pages para profissionais liberais

Site da **Zelo**, que cria landing pages para profissionais da saúde, do direito e do bem-estar, com botão direto para o WhatsApp. Página pronta em até 3 dias, preço fixo.

HTML, CSS e JavaScript puros, sem etapa de build.

## Estrutura

```
.
├── index.html              # a landing page
├── assets/
│   ├── css/
│   │   ├── tokens.css      # tokens da marca (cores, fontes, espaços, raios)
│   │   └── style.css       # estilos da página (claro e escuro)
│   ├── img/                # capturas dos exemplos de portfólio
│   └── logo/               # logo, favicon e avatar em SVG
└── README.md
```

## Onde editar

| O quê | Onde |
|---|---|
| Preços e itens dos planos | `index.html`, seção `#precos` |
| Número do WhatsApp | links `https://wa.me/5515996529487?...` no `index.html` (cada botão tem a sua mensagem pronta) |
| Instagram | rodapé do `index.html` |
| Cores e fontes | `assets/css/tokens.css` |

## Como abrir localmente

Dê dois cliques no `index.html`, ou sirva a pasta:

```bash
python -m http.server 5173
```

e acesse `http://localhost:5173`.

## Publicação

Publicado pelo GitHub Pages a partir da branch `main`. Cada push atualiza o site em cerca de 1 minuto.

### Domínio próprio (zeloweb.com.br)

Depois de registrar o domínio no [registro.br](https://registro.br):

1. No registro.br, em **DNS**, crie os registros:
   - `A` para `zeloweb.com.br` apontando para `185.199.108.153`, `185.199.109.153`, `185.199.110.153` e `185.199.111.153`
   - `CNAME` para `www` apontando para `<seu-usuario>.github.io`
2. No GitHub, em **Settings > Pages > Custom domain**, digite `zeloweb.com.br` e salve (isso cria o arquivo `CNAME`).
3. Quando o certificado ficar pronto, marque **Enforce HTTPS**.

A propagação do DNS pode levar algumas horas.

## Créditos

- Exemplos de portfólio: [landing-psicologos](https://github.com/LUCXSFIGUEIRA/landing-psicologos)
- Ícones: [Phosphor Icons](https://phosphoricons.com)
- Fontes: Outfit e Source Sans 3 (Google Fonts)

© Zelo. Todos os direitos reservados.
