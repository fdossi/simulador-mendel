# Simulador da Primeira Lei de Mendel

Simulador educacional, responsivo e offline sobre a Primeira Lei de Mendel, usando um modelo hipotético de milho com grãos azuis e amarelos.

## Versão web

O arquivo `index.html` pode ser publicado diretamente pelo GitHub Pages.

Após ativar o GitHub Pages nas configurações do repositório, o endereço será:

`https://fdossi.github.io/simulador-mendel/`

## Aplicativo para Windows 11

O projeto desktop usa Electron e gera:

- instalador para Windows;
- versão portátil sem instalação.

### Compilação online

Acesse a aba **Actions**, abra o fluxo **Gerar aplicativo Windows** e clique em **Run workflow**. Ao terminar, baixe o artefato `simulador-mendel-windows`.

### Execução local

```bash
npm install
npm start
```

### Compilação local

```bash
npm install
npm run dist
```

Os executáveis serão criados na pasta `dist`.

## Estrutura

- `index.html`: versão web para GitHub Pages;
- `app/index.html`: simulador incorporado ao aplicativo;
- `main.js`: janela do Electron;
- `package.json`: dependências e configuração de empacotamento;
- `.github/workflows/build-windows.yml`: compilação online dos executáveis;
- `.github/workflows/pages.yml`: publicação automatizada no GitHub Pages.

## Observação didática

O modelo é deliberadamente simplificado. A cor dos grãos representa uma característica monogênica hipotética com dominância completa, utilizada para investigar segregação alélica, fecundação aleatória e comparação entre frequências observadas e proporções mendelianas esperadas.
