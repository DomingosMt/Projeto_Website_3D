<img width="1911" height="857" alt="image" src="https://github.com/user-attachments/assets/d4aa1fe7-36ec-481c-9428-3e8982620c8e" />

# Projeto 3D - Landing Page

Uma landing page com animações de scroll, integração de visualização 3D e layout responsivo.

## Ferramentas e bibliotecas
- **HTML5** e **CSS3**
- **AOS (Animate On Scroll)** para animações ao rolar a página
  - CDN: `https://unpkg.com/aos@next/dist/aos.css` e `https://unpkg.com/aos@next/dist/aos.js`
- **Spline Viewer (@splinetool/viewer)** para incorporar cena 3D
  - CDN (module): `https://unpkg.com/@splinetool/viewer@1.10.89/build/spline-viewer.js`

## Características do código
- **Design responsivo** com media queries para tablet e mobile
- **Tipografia** com fonte de sistema e espaçamento de letras para navegação
- **Efeitos visuais**:
  - Imagem de gradiente (`gradient.png`) posicionada e com opacidade
  - Camada de desfoque com `box-shadow` inclinada
  - Botão e links com transições suaves
  - Caixa de tag com **gradiente animado** via `@keyframes`
  - Título com `text-shadow`
- **Animações on-scroll** usando atributos `data-aos` para header, navegação, título, descrição e botões
- **Integração 3D** com `<spline-viewer>` apontando para uma cena hospedada no Spline

## Estrutura de arquivos
- `index.html` – marcação principal com AOS e `<spline-viewer>`
- `style.css` – estilos globais, animações e responsividade
- `gradient.png` – ativo de fundo para efeito de gradiente

## Como executar
1. Abra o arquivo `index.html` em um navegador moderno.
2. É necessário acesso à internet para carregar as CDNs do **AOS** e do **@splinetool/viewer**.

## Desenvolvimento
- As animações AOS são inicializadas com `AOS.init()` no final do `index.html`.
- O componente `<spline-viewer>` é carregado via script `type="module"` e consome a URL da cena no atributo `url`.

## Autor

- Domingos Muratori.
