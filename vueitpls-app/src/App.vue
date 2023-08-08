<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <navbar>
    <div class="navbar">
      <p class="name">Зоомаркет</p>
      <div class="profile">
        <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAH4AAAB+CAMAAADV/VW6AAAAMFBMVEXk5ueutLeqsLPZ3N3n6eq0ubzd4OHS1dfFycvW2dq/xMbg4+S4vcDN0dO8wcPKztCju/PcAAACs0lEQVRoge2a226DMAyGc3ACJIG8/9sOKKvYBoldbJCm/BeVql58PuVkV6mmpqampqampqampqa9YNZDZBX9MOY8dtar242IeXJmk3ZhUDcaAHaaoXsZ3d9lAFj3k71ZcIsBoPoj+BqBTpwP/tD1zYAgTR9O2Ss/CdPPXX/JCca/Tp/5cnRbhc+Si7/D4E0vE38I9dCvfCuCRyR+k4T7gIVrk/n5mKp/i52OrLvN/ZHdfUtwnn/xQyDQtRmY8ZEQ+1mBOfqk2LNHH3oSXWverQcSjW46Vjwx9dwbv6fRtZ5Y8aijdi/ea0f5jnUkXjxt3f03PJXOi3+49MgLL7HiqduO5t12Ht50Hz5yqCuP+7oTac7zbvlz9CcKnTn1xHu2dpEZrxTFe/5nHox49w2/8wrweIk3LnSPPjHRxW+EGlzIc4d7zX8Lt/gEmzuY9AtU/ZtfX31esrMJ+Un6Ev8C27go3dWFmM4SINVS+2VApw8b6kk48G++yr/b2kZPw33zDFBDcPo10Vg+XfY3j3NA+S730xT6cbib/Rqh7XUneBmh9WFK6+XfpbREwEb5cRqoaMfJLQn/UXvrV5f6wcuNk+Zs5+RMYdudf5tNUAImANigS+jdGgwdcxrA58Ot5jQKwfIZAJZ0yX/JdTw5WCamdPqyCY/XDYD4GXw1wF3ciM8nptgIXDmBT842kgEXBiukHv4Z/8MrSHFYTNInFVAZFlP0QQIoL8o6n/rygGsV/0e0PhtkXvrs/1OR3/j44RKtkYLlo2/hxC4Wlo98dwO1gYrlox6f7GX3Fqr8vRQdFX5a/5CoOl2i6r9Vr35R5+utD/LUhKTa4UPu2xNVG/HI0mtjBr5D/kTF4uM+Z/+qGH3qxIguU8RLO1/+R1UUx+vSX3qsEVep9qIVly8Ev6mpqalJVF+YqB54PMBL1AAAAABJRU5ErkJggg==" alt="avatar">
        
      </div>
    </div>
  </navbar>
  <body>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </body>

  <RouterView />
</template>

<style scoped>
body {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
