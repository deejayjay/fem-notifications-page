<script>

</script>

<template>
  <main class="main">
    <div class="title-bar">
      <div class="title-bar__left">
        <h1 class="title">Notifications</h1>
        <span class="title__notifications">3</span>
      </div>
      <button type="button"
              class="btn-read">Mark all as read</button>
    </div>

    <ul>
      <li>
        <article>
          <h2>Mark Webber reacted to your recent post My first tournament today!</h2>
          <p>1m ago</p>
        </article>
      </li>
      <li>
        <article>
          <h2>Angela Gray followed you</h2>
          <p>5m ago</p>
        </article>
      </li>
      <li>
        <article>
          <h2>Jacob Thompson has joined your group Chess Club</h2>
          <p>1 day ago</p>
        </article>
      </li>
      <li>
        <article>
          <h2>Rizky Hasanuddin sent you a private message</h2>
          <p>5 days ago</p>
          <p>
            Hello, thanks for setting up the Chess Club. I've been a member for a few weeks now and
            I'm already having lots of fun and improving my game.
          </p>
        </article>
      </li>
      <li>
        <article>
          <h2>Kimberly Smith commented on your picture</h2>
          <p>1 week ago</p>
        </article>
      </li>
      <li>
        <article>
          <h2>Nathan Peterson reacted to your recent post 5 end-game strategies to increase your win rate</h2>
          <p>2 weeks ago</p>
        </article>
      </li>
      <li>
        <article>
          <h2>Anna Kim left the group Chess Club</h2>
          <p>2 weeks ago</p>
        </article>
      </li>
    </ul>
  </main>
  <footer class="attribution">
    <p>
      Challenge by <a href="https://www.frontendmentor.io?ref=challenge"
         target="_blank">Frontend Mentor</a>.
      Coded by <a href="https://github.com/deejayjay">DeeJayJay</a>.
    </p>
  </footer>
</template>

<style scoped>
.main {
  padding: 2.4rem 1.6rem;
}

.title-bar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 2.4rem;
}

.title-bar__left {
  display: flex;
  gap: 0.9rem;
  align-items: center;
}

.title {
  font-size: 2rem;
  color: var(--color-very-dark-blue);
}

.title__notifications {
  background-color: var(--color-primary-blue);
  color: var(--color-white);
  width: 32px;
  height: 25px;
  display: grid;
  place-items: center;
  border-radius: 6px;
}

.title,
.title__notifications {
  font-weight: 800;
}

.btn-read {
  border: none;
  border-radius: 6px;
  background-color: transparent;
  outline: 2px solid transparent;
  transition: outline-color 0.3s;
  font-size: 1.4rem;
  font-weight: 500;
  color: var(--color-dark-grayish-blue);
}

.btn-read:focus-visible {
  outline-color: var(--color-dark-grayish-blue);
}
</style>
