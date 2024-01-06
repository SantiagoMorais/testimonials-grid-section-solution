# Desafio Frontend Mentor - Testimonials grid section solution

Essa é uma solução do desafio [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7).

<img src="assets/design/desktop-preview.jpg" alt="imagem do projeto">

## Sumário
- [Visão Geral](#visão-geral)
  - [O desafio](#o-desafio)
  - [Screenshots](#screenshots)
- [Meu processo](#meu-processo)
  - [Tecnologias utilizadas](#tecnologias-utilizadas)
  - [O que aprendi?](#o-que-aprendi-?)
  - [Desenvolvimento contínuo](#desenvolvimento-contínuo)
  - [Recursos úteis](#recursos-úteis)
- [Autor](#autor)


## Visão Geral

### O desafio

Os usuários devem ser capazes de:

- Ver o layout ideal para o site dependendo do tamanho da tela do dispositivo;

### Screenshot

<img src="assets/screenshots/gif-do-projeto.gif">

**Responsividade do projeto**

## Meu processo

### Built with

- HTML5
- CSS
- Flexbox
- CSS Grid

### O que aprendi?

Pude utilizar meus conhecimentos com ```display:grid``` para manter as janelas de cada usuário na posição correta. Foi utilizado o ```grid-template-areas``` e media queries para reorganizar o número de colunas a medida que a tela diminuia. Dessa forma, o projeto se adapta aos vários tamanhos dos dispositivos.

```css
.windows {
    display: grid;
    grid-template-areas: "daniel daniel jonathan kira"
                         "jeanette patrick patrick kira";
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    width: 80%;
    transition: .3s;
}
```

O projeto também foi organizado de forma que facilite a manutenção e a compreensão de terceiros ao visualizar o código. Foi utilizado, por exemplo, um arquivo próprio para separar as variáveis e a responsividade do projeto.

```css
:root {
    --first-background-color: hsl(263, 55%, 52%);
    --second-background-color: hsl(217, 19%, 35%);
    --third-background-color: hsl(219, 29%, 14%);
    --dark-opaque-color: hsl(219, 29%, 14%,.7);
    --white-color: hsl(0, 0%, 100%);
    --white-opaque-color: hsl(0, 0%, 100%, .5);
    --container-background-color: hsl(210, 46%, 95%);
    --commentary-color: hsl(0, 0%, 81%);
}
```

A organização da estrutura HTML de cada janela de usuário foi realizada da mesma forma, alterando somente as classes de cada ```div```, para que assim as cores de fundo específicas de cada usuário e que o ```grid-area``` fosse definido.

```html
      <div class="window daniel">
        <div class="profile">
          <img src="assets/images/image-daniel.jpg" alt="personal user avatar" class="avatar">
          <div>
            <h2 class="name">Daniel Clifford</h2>
            <p class="verified-user">Verified Graduate</p>
          </div>
        </div>
        <p class="avaliation">
          I received a job offer mid-course, and the subjects I learned were current, if not more so,
          in the company I joined. I honestly feel I got every penny’s worth.
        </p>
        <p class="commentary">
          “ I was an EMT for many years before I joined the bootcamp. I’ve been looking to make a
          transition and have heard some people who had an amazing experience here. I signed up
          for the free intro course and found it incredibly fun! I enrolled shortly thereafter.
          The next 12 weeks was the best - and most grueling - time of my life. Since completing
          the course, I’ve successfully switched careers, working as a Software Engineer at a VR startup. ”
        </p>
      </div>
```

### Desenvolvimento contínuo

Conhecimentos em CSS e HTML bem consolidados. O foco é avançar cada vez mais o conhecimento para a área de JavaScript e ReactJS, para cada vez mais melhorar a estilização e aumentar as possibilidades de interação no projeto.

### Recursos úteis

- [Responsive Viewer](https://chromewebstore.google.com/detail/responsive-viewer/inmopeiepgfljkpkidclfgbgbmfcennb) - Essa extensão do navegador nos ajuda a visualizar o projeto através das telas dos diversos dispositivos, assim, melhorar a responsividade. 
- [Auto rename tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag) - Com essa extensão do VSCode é possível alterar, simultaneamente, o valor das tags HTML na sua abertura e fechamento, assim o processo de desenvolvimento do código é acelerado.
- [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) - Extensão do VSCode que transmite automaticamente no navegador as alterações feitas no projeto, dispensando a necessidade de atualização da página.
- [Color HighLight](https://marketplace.visualstudio.com/items?itemName=naumovs.color-highlight) - Faz com que as cores escritas em RGB, RGBA, HSL e outros fiquem coloridas com a cor que as define. Assim facilita visualmente a seleção de cores no CSS.

## Author

- Linkedin - [FelipeSantiagoMorais](https://www.linkedin.com/in/felipe-santiago-873025288/)
- Frontend Mentor - [@SantiagoMorais](https://www.frontendmentor.io/profile/SantiagoMorais)
- GitHub - [SantiagoMorais](https://github.com/SantiagoMorais)
