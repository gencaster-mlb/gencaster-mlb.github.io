<template>
  <footer>
    <span />
    <p>2022 – 2023</p>
    <NuxtLink href="/imprint">
      Imprint
    </NuxtLink>
  </footer>
</template>

<style lang="scss" scoped>
footer {
        width: 100%;
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        margin-top: 5rem;
        margin-bottom: 2rem;

        span {
            display: block;
        }

        p {
            margin-bottom: 0;
            text-align: center;
        }

        a {
            text-align: end;
        }
    }
</style>
