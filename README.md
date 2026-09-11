# Site para Psicólogo — HTML, CSS e JavaScript

Landing page responsiva e sem framework, pronta para GitHub Pages.

## Estrutura

```text
site-psicologo/
├── index.html
├── README.md
└── assets/
    ├── css/
    │   └── style.css
    ├── js/
    │   └── script.js
    └── img/
        └── psicologo.jpg   ← coloque a foto aqui
```

## Personalização rápida

### 1. Nome e CRP
No `index.html`, procure por:
- `Rafael Almeida`
- `CRP 00/00000`

### 2. Foto
Coloque a foto do profissional em:

`assets/img/psicologo.jpg`

Pode usar JPG, PNG ou WebP. Se mudar o nome/extensão, altere também o `src` da imagem no HTML.

### 3. WhatsApp
No `index.html`, procure por:

`https://wa.me/5500000000000`

Troque pelo número no formato internacional, sem espaços, parênteses ou hífen.

Exemplo:
`https://wa.me/5548999999999`

### 4. Frases
A frase principal fica no `<h1>` e a frase sobre a foto fica no `.quote-card`.

### 5. Cores
As cores principais estão no começo de `assets/css/style.css`, dentro de `:root`.

## Publicar no GitHub Pages

Conta: `ademilton-mariano`. Repositório previsto: `site-psicologo`.

Domínio personalizado: `psicologo.adriano.a-mariano.com.br`.

1. Crie um repositório no GitHub.
2. Envie todos os arquivos mantendo a estrutura de pastas.
3. Vá em **Settings → Pages**.
4. Em **Build and deployment**, selecione **Deploy from a branch**.
5. Escolha `main` e `/ (root)`.
6. Salve e aguarde o GitHub publicar.

O projeto não precisa de Node, Angular, build ou servidor.

### Domínio e DNS no Cloudflare

Em **Settings → Pages → Custom domain**, informe `psicologo.adriano.a-mariano.com.br` e salve.

Na zona `a-mariano.com.br` do Cloudflare, crie o registro:

| Campo | Valor |
| --- | --- |
| Tipo | CNAME |
| Nome | psicologo.adriano |
| Destino | ademilton-mariano.github.io |
| Proxy | Somente DNS (nuvem cinza) |
| TTL | Automático |

Depois que o GitHub validar o DNS e emitir o certificado, ative **Enforce HTTPS**.
O Registro.br permanece como registrador; os registros DNS são gerenciados no Cloudflare.

## Observação profissional

Antes de publicar, substitua os textos fictícios, CRP, dados de contato e informações de atuação pelos dados reais do profissional.
