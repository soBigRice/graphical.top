<template>
  <main class="homepage">
    <section class="glass-panel">
      <p class="domain">Welcome to graphical.top</p>

      <h1 class="word" aria-label="graphical">
        <span style="--i: 0" data-letter="g">g</span>
        <span style="--i: 1" data-letter="r">r</span>
        <span style="--i: 2" data-letter="a">a</span>
        <span style="--i: 3" data-letter="p">p</span>
        <span style="--i: 4" data-letter="h">h</span>
        <span style="--i: 5" data-letter="i">i</span>
        <span style="--i: 6" data-letter="c">c</span>
        <span style="--i: 7" data-letter="a">a</span>
        <span style="--i: 8" data-letter="l">l</span>
      </h1>

      <p class="tagline">
        网站简介：这是一个网站，不过目前我没想好写啥，欢迎各位投稿。
        可以点击
        <a
          href="https://github.com/soBigRice/graphical.top"
          target="_blank"
          rel="noopener noreferrer"
        >
          此处
        </a>
        跳转到代码仓库投稿。
      </p>
    </section>

    <a
      class="author"
      href="https://github.com/sobigrice"
      target="_blank"
      rel="noopener noreferrer"
      aria-label="Visit sobigrice on GitHub"
    >
      <svg viewBox="0 0 16 16" aria-hidden="true">
        <path
          d="M8 0C3.58 0 0 3.58 0 8a8.001 8.001 0 0 0 5.47 7.59c.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.5-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82a7.58 7.58 0 0 1 4 0c1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.001 8.001 0 0 0 16 8c0-4.42-3.58-8-8-8Z"
        />
      </svg>
      <span>Author: sobigrice</span>
    </a>
  </main>
</template>

<style scoped>
.homepage {
  position: relative;
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: clamp(1.25rem, 4vw, 3.5rem);
  overflow: visible;
  isolation: isolate;
}

.glass-panel {
  width: min(72rem, 100%);
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: clamp(1.5rem, 5vw, 3.5rem);
  border-radius: clamp(1.25rem, 3vw, 2.25rem);
  border: 1px solid rgba(255, 255, 255, 0.5);
  background: linear-gradient(
    140deg,
    rgba(255, 255, 255, 0.48),
    rgba(255, 255, 255, 0.2)
  );
  text-align: center;
  backdrop-filter: blur(26px) saturate(140%);
  -webkit-backdrop-filter: blur(26px) saturate(140%);
  box-shadow:
    0 26px 60px rgba(5, 24, 29, 0.2),
    inset 0 1px 0 rgba(255, 255, 255, 0.75);
}

.domain {
  margin: 0;
  font-size: clamp(0.82rem, 1.4vw, 1.06rem);
  letter-spacing: 0.06em;
  text-transform: none;
  color: rgba(29, 41, 50, 0.72);
}

.word {
  margin: clamp(0.8rem, 2vw, 1.2rem) 0 clamp(0.4rem, 1vw, 0.8rem);
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  width: 100%;
  gap: 0.03em;
  font-family: var(--font-display);
  font-size: clamp(3.6rem, 18vw, 12rem);
  line-height: 1.08;
  letter-spacing: -0.025em;
  text-transform: lowercase;
  overflow: visible;
  padding: 0.1em 0.14em 0.26em 0.04em;
  text-shadow: 0 14px 32px rgba(66, 63, 145, 0.26);
}

.word span {
  position: relative;
  display: inline-block;
  padding: 0.04em 0.05em 0.12em 0.01em;
  color: transparent;
  background: linear-gradient(
    to right,
    rgba(236, 229, 255, 0.98),
    rgba(188, 182, 255, 0.9) 45%,
    rgba(119, 179, 255, 0.84)
  );
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-stroke: 1px rgba(231, 227, 255, 0.92);
}

.word span::before {
  content: attr(data-letter);
  position: absolute;
  inset: -0.01em -0.03em -0.06em 0;
  color: transparent;
  background-image: linear-gradient(
    to right,
    #d8b9ff 0%,
    #b59bff 30%,
    #8f8cff 58%,
    #5f96ff 80%,
    #59bcff 100%
  );
  background-size: 200% 100%;
  background-position: calc(var(--i) * 12.5%) 50%;
  -webkit-background-clip: text;
  background-clip: text;
  opacity: 0.88;
  pointer-events: none;
}

.word span::after {
  content: attr(data-letter);
  position: absolute;
  inset: -0.01em -0.03em -0.06em 0;
  color: transparent;
  background: linear-gradient(
    180deg,
    rgba(246, 242, 255, 0.98),
    rgba(146, 181, 255, 0.3)
  );
  -webkit-background-clip: text;
  background-clip: text;
  filter: blur(6px);
  opacity: 0.72;
  pointer-events: none;
}

.word span:nth-child(odd) {
  transform: translateY(-0.04em);
}

.word span:nth-child(even) {
  transform: translateY(0.03em);
}

.tagline {
  margin: 0;
  font-family: var(--font-body);
  font-size: clamp(0.95rem, 1.7vw, 1.25rem);
  letter-spacing: 0.03em;
  color: rgba(23, 34, 42, 0.82);
}

.tagline a {
  color: rgba(24, 85, 122, 0.94);
  text-decoration: underline;
  text-decoration-thickness: 1.5px;
  text-underline-offset: 0.14em;
}

.tagline a:hover {
  color: rgba(11, 63, 95, 0.98);
}

.author {
  position: fixed;
  right: clamp(0.8rem, 2.5vw, 1.4rem);
  bottom: clamp(0.8rem, 2.5vw, 1.4rem);
  z-index: 5;
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.48rem 0.72rem;
  border-radius: 999px;
  border: 1px solid rgba(255, 255, 255, 0.55);
  background: rgba(255, 255, 255, 0.28);
  backdrop-filter: blur(14px) saturate(130%);
  -webkit-backdrop-filter: blur(14px) saturate(130%);
  color: rgba(20, 33, 43, 0.92);
  text-decoration: none;
  font-family: var(--font-body);
  font-size: clamp(0.72rem, 1.05vw, 0.88rem);
  letter-spacing: 0.02em;
  box-shadow: 0 12px 28px rgba(10, 23, 31, 0.2);
  transition:
    transform 0.2s ease,
    box-shadow 0.2s ease,
    background-color 0.2s ease;
}

.author svg {
  width: 1rem;
  height: 1rem;
  fill: currentColor;
}

.author:hover {
  transform: translateY(-1px);
  background: rgba(255, 255, 255, 0.35);
  box-shadow: 0 16px 32px rgba(10, 23, 31, 0.24);
}

.author:focus-visible {
  outline: 2px solid rgba(35, 73, 99, 0.65);
  outline-offset: 2px;
}

@media (max-width: 700px) {
  .glass-panel {
    padding: 1.4rem;
  }

  .word {
    gap: 0;
    line-height: 1.08;
  }

  .author {
    right: 0.7rem;
    bottom: 0.7rem;
    padding: 0.42rem 0.62rem;
  }
}
</style>
