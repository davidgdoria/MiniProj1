# MiniProj1

O meu currículo, feito como Single Page Application em Vue.js para a Tarefa 2.2 do Mestrado em Engenharia Informática e Tecnologia Web (Universidade Aberta).

Projeto no GitHub: https://github.com/users/davidgdoria/projects/1

## Como abrir

Basta abrir o `index.html` no browser. É preciso ter internet, porque o Vue e o Vue Router vêm da CDN do jsDelivr.

## Como está feito

Está tudo no `index.html`: o HTML, o CSS e o JavaScript. Usei Vue 3 com Vue Router, as duas bibliotecas carregadas por CDN, sem build.

Há quatro páginas, cada uma com a sua rota:

- `#/` — Início
- `#/quem-sou-eu` — Quem Sou Eu?
- `#/o-que-faco` — O que faço?
- `#/hobbies` — Hobbies

O router está em modo hash (`createWebHashHistory`), por isso ao clicar nos links só muda a parte do endereço depois do `#`. O browser não volta a pedir a página ao servidor: o Vue troca apenas o conteúdo do `<main>`. O cabeçalho e o rodapé com as redes sociais são comuns a todas as páginas.

A janela modal é usada no botão "Contactar" da página inicial e em cada carta da página Hobbies. Fecha no ×, com a tecla Esc ou com um clique fora da janela.

Os hobbies estão desenhados como cartas de TCG (um dos hobbies), só com CSS.

Os textos do currículo estão todos no objeto `perfil`, no início do script.

## Wireframes

Estão em `docs/wireframes.pdf`, e cada um também em PNG e SVG na pasta `docs/wireframes/`.

## Créditos

- [Vue.js](https://vuejs.org/) e [Vue Router](https://router.vuejs.org/)
- Ícones: [Font Awesome Free](https://fontawesome.com/license/free) (licença CC BY 4.0)
- Tipos de letra: [IBM Plex Sans e IBM Plex Mono](https://fonts.google.com/specimen/IBM+Plex+Sans) (SIL Open Font License), pelo Google Fonts

## Recursos consultados

- [Developing a Single Page App with FastAPI and Vue.js](https://testdriven.io/blog/developing-a-single-page-app-with-fastapi-and-vuejs/)
- [Introduction to Vue.js with a Single Page Application (SPA) in Visual Studio](https://www.red-gate.com/simple-talk/development/javascript/introduction-to-vue-js-with-a-single-page-application-spa-in-visual-studio/)
- [What is a Single Page Application?](https://www.seguetech.com/what-is-a-single-page-application/)
- [MDN — O seu primeiro website](https://developer.mozilla.org/pt-BR/docs/Learn_web_development/Getting_started/Your_first_website)
