<!-- Slots nomeados -->

<template>
  <div class="container">
    <header>
      <slot name="header"></slot>
    </header>
    <main>
      <slot></slot>
    </main>
    <footer>
      <slot name="footer"></slot>
    </footer>
  </div>
</template>

<style>
  footer {
    border-top: 1px solid #d898fd;
    color: #5c3366;
    font-size: 0.8em;
  }
</style>