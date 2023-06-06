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
    <!-- List of notifications -->
    <ul class="notifications-list">
      <li class="notifications-list-item">
        <article class="notification notification--unread">
          <picture>
            <source srcset="./assets/images/avatar-mark-webber.webp"
                    media="(min-width: 1024px)"
                    width="45"
                    height="45">
            <img src="./assets/images/avatar-mark-webber.webp"
                 alt="Avatar of Mark Webber"
                 class="notification__avatar"
                 width="39"
                 height="39">
          </picture>
          <section class="notification__content">
            <h2 class="notification__title">
              <span class="notification__author">Mark Webber</span> reacted to your recent post
              <strong class="notification__post">My first tournament today!</strong>
              <span class="notification__indicator"></span>
            </h2>
            <p class="notification__time">1m ago</p>
          </section>
        </article>
      </li>
      <li class="notifications-list-item">
        <article class="notification notification--unread">
          <picture>
            <source srcset="./assets/images/avatar-angela-gray.webp"
                    media="(min-width: 1024px)"
                    width="45"
                    height="45">
            <img src="./assets/images/avatar-angela-gray.webp"
                 alt="Avatar of Angela Gray"
                 class="notification__avatar"
                 width="39"
                 height="39">
          </picture>
          <section class="notification__content">
            <h2 class="notification__title">
              <span class="notification__author">Angela Gray</span> followed you
              <span class="notification__indicator"></span>
            </h2>
            <p class="notification__time">5m ago</p>
          </section>
        </article>
      </li>
      <li class="notifications-list-item">
        <article class="notification notification--unread">
          <picture>
            <source srcset="./assets/images/avatar-jacob-thompson.webp"
                    media="(min-width: 1024px)"
                    width="45"
                    height="45">
            <img src="./assets/images/avatar-jacob-thompson.webp"
                 alt="Avatar of Jacob Thompson"
                 class="notification__avatar"
                 width="39"
                 height="39">
          </picture>
          <section class="notification__content">
            <h2 class="notification__title">
              <span class="notification__author">Jacob Thompson</span> has joined your group
              <a href="#"
                 class="notification__group">Chess Club</a>
              <span class="notification__indicator"></span>
            </h2>
            <p class="notification__time">1 day ago</p>
          </section>
        </article>
      </li>
      <li class="notifications-list-item">
        <article class="notification">
          <picture>
            <source srcset="./assets/images/avatar-rizky-hasanuddin.webp"
                    media="(min-width: 1024px)"
                    width="45"
                    height="45">
            <img src="./assets/images/avatar-rizky-hasanuddin.webp"
                 alt="Avatar of Rizky Hasanuddin"
                 class="notification__avatar"
                 width="39"
                 height="39">
          </picture>
          <section class="notification__content">
            <h2 class="notification__title">
              <span class="notification__author">Rizky Hasanuddin</span> sent you a private message
            </h2>
            <p class="notification__time">5 days ago</p>
            <p class="notification__private-message">
              Hello, thanks for setting up the Chess Club. I've been a member for a few weeks now and
              I'm already having lots of fun and improving my game.
            </p>
          </section>
        </article>
      </li>
      <li class="notifications-list-item">
        <article class="notification">
          <picture>
            <source srcset="./assets/images/avatar-kimberly-smith.webp"
                    media="(min-width: 1024px)"
                    width="45"
                    height="45">
            <img src="./assets/images/avatar-kimberly-smith.webp"
                 alt="Avatar of Kimberly Smith"
                 class="notification__avatar"
                 width="39"
                 height="39">
          </picture>
          <section class="notification__content">
            <h2 class="notification__title">
              <span class="notification__author">Kimberly Smith</span> commented on your picture
            </h2>
            <p class="notification__time">1 week ago</p>
          </section>
        </article>
      </li>
      <li class="notifications-list-item">
        <article class="notification">
          <picture>
            <source srcset="./assets/images/avatar-nathan-peterson.webp"
                    media="(min-width: 1024px)"
                    width="45"
                    height="45">
            <img src="./assets/images/avatar-nathan-peterson.webp"
                 alt="Avatar of Nathan Peterson"
                 class="notification__avatar"
                 width="39"
                 height="39">
          </picture>
          <section class="notification__content">
            <h2 class="notification__title">
              <span class="notification__author">Nathan Peterson</span> reacted to your recent post
              <strong class="notification__post ml--3">5 end-game strategies to increase your win rate</strong>
            </h2>
            <p class="notification__time">2 weeks ago</p>
          </section>
        </article>
      </li>
      <li class="notifications-list-item">
        <article class="notification">
          <picture>
            <source srcset="./assets/images/avatar-anna-kim.webp"
                    media="(min-width: 1024px)"
                    width="45"
                    height="45">
            <img src="./assets/images/avatar-anna-kim.webp"
                 alt="Avatar of Anna Kim"
                 class="notification__avatar"
                 width="39"
                 height="39">
          </picture>
          <section class="notification__content">
            <h2 class="notification__title">
              <span class="notification__author">Anna Kim</span> left the group
              <a href="#"
                 class="notification__group">Chess Club</a>
            </h2>
            <p class="notification__time">2 weeks ago</p>
          </section>
        </article>
      </li>
    </ul>
    <!-- End of list of notifications -->
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
  color: var(--color-dark-grayish-blue);
}

.btn-read:focus-visible {
  outline-color: var(--color-dark-grayish-blue);
}

.notification {
  font-size: 1.4rem;
  display: grid;
  grid-template-columns: 39px 1fr;
  gap: 1.3rem;
  margin-bottom: 1rem;
  padding: 1.6rem;
  border-radius: 8px;
}

.notifications-list-item:last-of-type .notification {
  margin-bottom: 0;
}

.notification--unread {
  background-color: var(--color-very-light-grayish-blue);
  box-shadow: 0 0 2px rgba(0, 0, 0, 0.1);
}

.notification__content {
  line-height: 1.275;
  color: var(--color-dark-grayish-blue);
}

.notification__indicator {
  width: 8px;
  height: 8px;
  border-radius: 50%;
  background-color: var(--color-primary-red);
  display: inline-block;
  margin-left: 6px;
}

.notification__author {
  font-weight: 800;
  color: var(--color-very-dark-blue);
  margin-right: 0.6rem;
}

.notification__post,
.notification__group {
  font-weight: 800;
  margin-left: 0.6rem;
}

.ml--3 {
  margin-left: 0.3rem;
}

.notification__group {
  text-decoration: none;
  color: var(--color-primary-blue);
}

.notification__time {
  margin-top: 0.4rem;
  color: var(--color-grayish-blue);
}

.notification__avatar {
  width: 39px;
  height: 39px;
}

.notification__private-message {
  border: 1px solid var(--color-light-grayish-blue-2);
  border-radius: 5px;
  padding: 1.6rem;
  margin-top: 1.2rem;
}

@media only screen and (width >=1024px) {
  .notification {
    grid-template-columns: 45px 1fr;
  }

  .notification__avatar {
    width: 45px;
    height: 45px;
  }
}
</style>
