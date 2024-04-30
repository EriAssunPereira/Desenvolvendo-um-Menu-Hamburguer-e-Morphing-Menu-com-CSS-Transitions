# Desenvolvendo-um-Menu-Hamburguer-e-Morphing-Menu-com-CSS-Transitions

Vou explicar e dar um exemplo prático de como desenvolver um Menu Hambúrguer e Morphing Menu com transições CSS, tudo organizado em módulos.

**Descrição do Projeto:**
Este projeto é focado em ensinar os conceitos fundamentais de animações no CSS. Você aprenderá sobre:

- **Transições CSS (CSS Transitions):** Utilizando pseudo-elementos (`::before`, `::after`) e pseudo-classes (`:hover`, `:focus`, etc.), você poderá criar efeitos visuais interativos que respondem a ações do usuário.
  
- **Animações CSS (@keyframes):** Você irá explorar como criar animações mais complexas que mudam de estilo ao longo do tempo.

Ao final do projeto, você terá construído um portfólio interativo usando apenas HTML e CSS, consolidando o conhecimento adquirido nas aulas.

**Exemplo Prático:**

Vamos criar um Menu Hambúrguer que, ao clicar, transforma-se em um "X" (Morphing Effect) e revela um menu de navegação.

```css
/* Estrutura básica do menu hambúrguer */
.hamburger-menu {
  display: block;
  position: relative;
  width: 30px;
  height: 2px;
  background: #333;
  transition: all 0.3s ease-in-out;
}

.hamburger-menu::before,
.hamburger-menu::after {
  content: '';
  position: absolute;
  width: 100%;
  height: 2px;
  background: #333;
  transition: all 0.3s ease-in-out;
}

.hamburger-menu::before { top: -10px; }
.hamburger-menu::after { top: 10px; }

/* Estado do menu quando ativo */
.menu-ativo .hamburger-menu {
  transform: rotate(45deg);
}

.menu-ativo .hamburger-menu::before {
  top: 0;
  transform: rotate(0);
  opacity: 0;
}

.menu-ativo .hamburger-menu::after {
  top: 0;
  transform: rotate(90deg);
}
```

```html
<!-- HTML para o menu hambúrguer -->
<div class="menu-ativo">
  <div class="hamburger-menu"></div>
</div>
```

**Módulos:**
Para modularizar, você pode separar o CSS do menu hambúrguer em um arquivo chamado `hamburger-menu.css` e incluí-lo no seu HTML usando a tag `<link>`. Isso ajuda a manter o código organizado e facilita a manutenção.

Espero que este exemplo te ajude a entender melhor como criar animações e transições com CSS. 

Vou te explicar melhor e dar mais um exemplo prático de como desenvolver um Menu Hambúrguer e Morphing Menu com transições CSS, tudo organizado em módulos.

**Descrição do Projeto:**
Este projeto é focado em ensinar os conceitos fundamentais de animações no CSS. Você aprenderá sobre:

- **Transições CSS (CSS Transitions):** Utilizando pseudo-elementos (`::before`, `::after`) e pseudo-classes (`:hover`, `:focus`, etc.), você poderá criar efeitos visuais interativos que respondem a ações do usuário.
  
- **Animações CSS (@keyframes):** Você irá explorar como criar animações mais complexas que mudam de estilo ao longo do tempo.

Ao final do projeto, você terá construído um portfólio interativo usando apenas HTML e CSS, consolidando o conhecimento adquirido nas aulas.

**Exemplo Prático:**

Vamos criar um Menu Hambúrguer que, ao clicar, transforma-se em um "X" (Morphing Effect) e revela um menu de navegação.

```css
/* Estrutura básica do menu hambúrguer */
.hamburger-menu {
  display: block;
  position: relative;
  width: 30px;
  height: 2px;
  background: #333;
  transition: all 0.3s ease-in-out;
}

.hamburger-menu::before,
.hamburger-menu::after {
  content: '';
  position: absolute;
  width: 100%;
  height: 2px;
  background: #333;
  transition: all 0.3s ease-in-out;
}

.hamburger-menu::before { top: -10px; }
.hamburger-menu::after { top: 10px; }

/* Estado do menu quando ativo */
.menu-ativo .hamburger-menu {
  transform: rotate(45deg);
}

.menu-ativo .hamburger-menu::before {
  top: 0;
  transform: rotate(0);
  opacity: 0;
}

.menu-ativo .hamburger-menu::after {
  top: 0;
  transform: rotate(90deg);
}
```

```html
<!-- HTML para o menu hambúrguer -->
<div class="menu-ativo">
  <div class="hamburger-menu"></div>
</div>
```

**Módulos:**
Para modularizar, você pode separar o CSS do menu hambúrguer em um arquivo chamado `hamburger-menu.css` e incluí-lo no seu HTML usando a tag `<link>`. Isso ajuda a manter o código organizado e facilita a manutenção.

Espero que este exemplo te ajude a entender melhor como criar animações e transições com CSS.
