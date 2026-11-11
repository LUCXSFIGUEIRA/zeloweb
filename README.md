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
│   │   ├── style.css       # estilos da página (claro e escuro)
│   │   └── black-november.css  # tema da campanha de novembro (remover em dezembro)
│   ├── img/                # capturas do site real do Studio C Beauty
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

## Black November (novembro de 2026)

A página está no tema da campanha: site vitalício por R$ 249, domínio grátis, até 30/11.

- Visual: `assets/css/black-november.css`, carregado depois do `style.css`.
- Conteúdo: blocos marcados `BLACK NOVEMBER` no `index.html` (faixa do topo, letreiro, contagem regressiva).
- Prazo da contagem: constante `FIM` no script do fim do `index.html`. Quando o prazo passa, a contagem mostra "encerrada".
- Para encerrar a campanha: remova o `<link>` do `black-november.css` e volte os textos e preços pelo histórico do git.

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

- Exemplo real: [studiocbeauty.com.br](https://studiocbeauty.com.br)
- Ícones: [Phosphor Icons](https://phosphoricons.com)
- Fontes: Outfit e Source Sans 3 (Google Fonts)

© Zelo. Todos os direitos reservados.
