<script setup>
const { data: news } = await useAsyncData('news', () => {
  return queryContent('news').sort({ date: -1 }).limit(2).find()
})
</script>

<template>
  <section>
    <SectionHeading heading="News" />
    <div class="news-archive-container">
      <NewsArchiveTile v-for="(article, index) in news" :key="index" :article="article" />
      <div class="more-link">
        <NuxtLink to="/news">
          More
        </NuxtLink>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@import "assets/scss/variables.scss";
@import "assets/scss/mixins.scss";

.news-archive-container {
        @include gap;

        display: grid;
        grid-template-columns: 1fr;
        justify-content: space-between;

        @include onScreen('tablet-portrait-up') {
            grid-template-columns: 5fr 5fr 2fr;
            flex-direction: row;
        }
    }

    .more-link {
        @include fontStyle('largeBodyText');

        background: $grey;
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;

        a {
            @include padding-v(1.5em);
            @include padding-h(5ch);

            @include onScreen('tablet-portrait-up') {
                @include padding-h(2ch);
            }
        }
    }
</style>
