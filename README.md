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

No ar em **https://www.zeloweb.com.br**, publicado pelo GitHub Pages a partir da branch `main`. Cada push atualiza o site em cerca de 1 minuto.

### Domínio (zeloweb.com.br)

- DNS no [registro.br](https://registro.br): quatro registros `A` para `zeloweb.com.br` (`185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`) e um `CNAME` de `www` para `lucxsfigueira.github.io`.
- No GitHub, **Settings > Pages > Custom domain** está como `www.zeloweb.com.br` (arquivo `CNAME` na raiz). O endereço sem `www` redireciona para ele.
- Não apague o arquivo `CNAME`: sem ele o domínio deixa de funcionar.

## Créditos

- Exemplos de portfólio: [landing-psicologos](https://github.com/LUCXSFIGUEIRA/landing-psicologos)
- Ícones: [Phosphor Icons](https://phosphoricons.com)
- Fontes: Outfit e Source Sans 3 (Google Fonts)

© Zelo. Todos os direitos reservados.
