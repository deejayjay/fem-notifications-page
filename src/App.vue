<script>
export default {
  name: 'App',
  data() {
    return {
      areAllMessagesRead: false,
      noOfNotifications: 3
    }
  },
  methods: {
    markAllAsReadHandler() {
      this.areAllMessagesRead = true;
      this.noOfNotifications = 0;
    }
  }
}
</script>

<template>
  <main class="main">
    <div class="title-bar">
      <div class="title-bar__left">
        <h1 class="title">Notifications</h1>
        <span class="title__notifications">{{ noOfNotifications }}</span>
      </div>
      <button type="button"
              class="btn-read"
              :disabled="areAllMessagesRead"
              @click="markAllAsReadHandler">Mark all as read</button>
    </div>
    <!-- List of notifications -->
    <ul class="notifications-list">
      <li class="notifications-list-item">
        <article class="notification"
                 :class="{ 'notification--unread': !areAllMessagesRead }">
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
              <a href="#"
                 class="notification__author">Mark Webber</a> reacted to your recent post
              <a href="#"
                 class="notification__post">My first tournament today!</a>
              <span class="notification__indicator"
                    v-if="!areAllMessagesRead"></span>
            </h2>
            <p class="notification__time">1m ago</p>
          </section>
        </article>
      </li>
      <li class="notifications-list-item">
        <article class="notification"
                 :class="{ 'notification--unread': !areAllMessagesRead }">
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
              <a href="#"
                 class="notification__author">Angela Gray</a> followed you
              <span class="notification__indicator"
                    v-if="!areAllMessagesRead"></span>
            </h2>
            <p class="notification__time">5m ago</p>
          </section>
        </article>
      </li>
      <li class="notifications-list-item">
        <article class="notification"
                 :class="{ 'notification--unread': !areAllMessagesRead }">
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
              <a href="#"
                 class="notification__author">Jacob Thompson</a> has joined your group
              <a href="#"
                 class="notification__group">Chess Club</a>
              <span class="notification__indicator"
                    v-if="!areAllMessagesRead"></span>
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
              <a href="#"
                 class="notification__author">Rizky Hasanuddin</a> sent you a private message
            </h2>
            <p class="notification__time">5 days ago</p>
            <a class="notification__private-message"
               href="#">
              Hello, thanks for setting up the Chess Club. I've been a member for a few weeks now and
              I'm already having lots of fun and improving my game.
            </a>
          </section>
        </article>
      </li>
      <li class="notifications-list-item">
        <article class="notification notification--profile-pic">
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
              <a href="#"
                 class="notification__author">Kimberly Smith</a> commented on your picture
            </h2>
            <p class="notification__time">1 week ago</p>
          </section>
          <picture>
            <source srcset="./assets/images/image-chess.webp"
                    media="(min-width: 1024px)"
                    width="45"
                    height="45">
            <img src="./assets/images/image-chess.webp"
                 alt="My profile picture"
                 class="notification__profile-picture"
                 width="39"
                 height="39">
          </picture>
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
              <a href="#"
                 class="notification__author">Nathan Peterson</a> reacted to your recent post
              <a href="#"
                 class="notification__post ml--3">5 end-game strategies to increase your win rate</a>
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
              <a href="#"
                 class="notification__author">Anna Kim</a> left the group
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
  background-color: var(--color-white);
  border-radius: 0;
  transition: border-radius 0.25s;
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
  font-size: clamp(2rem, 2.5vw, 2.4rem);
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
  font-size: clamp(1.4rem, 2vw, 1.6rem);
  color: var(--color-dark-grayish-blue);
  transition: color 0.25s;
}

.btn-read:disabled {
  color: var(--color-grayish-blue);
}

.btn-read:hover:not(:disabled) {
  cursor: pointer;
  color: var(--color-primary-blue);
}

.btn-read:focus-visible {
  outline-color: var(--color-dark-grayish-blue);
}

.notification {
  font-size: clamp(1.4rem, 2vw, 1.6rem);
  display: grid;
  grid-template-columns: 39px 1fr;
  gap: 1.3rem;
  margin-bottom: 1rem;
  padding: 1.6rem;
  border-radius: 8px;
  background-color: var(--color-white);
  box-shadow: 0 0 2px transparent;
  transition: background-color 0.3s, box-shadow 0.3s;
}

.notification--profile-pic {
  grid-template-columns: 39px 1fr 39px;
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
  translate: 0 -25%;
}

.notification__author {
  font-weight: 800;
  color: var(--color-very-dark-blue);
  margin-right: 0.6rem;
  text-decoration: none;
  transition: color 0.25s;
}

.notification__author:hover {
  color: var(--color-primary-blue);
  cursor: pointer;
}

.notification__post,
.notification__group {
  font-weight: 800;
  margin-left: 0.6rem;
  text-decoration: none;
}

.notification__post {
  color: var(--color-dark-grayish-blue);
  transition: color 0.25s;
}

.notification__post:hover {
  cursor: pointer;
  color: var(--color-primary-blue);
}

.notification__group {
  color: var(--color-primary-blue);
}

.ml--3 {
  margin-left: 0.3rem;
}

.notification__time {
  margin-top: 0.4rem;
  color: var(--color-grayish-blue);
}

.notification__avatar {
  width: 39px;
  height: 39px;
}

.notification__profile-picture {
  border-radius: 7px;
}

.notification__private-message {
  display: block;
  border: 1px solid var(--color-light-grayish-blue-2);
  border-radius: 5px;
  padding: 1.6rem;
  margin-top: 1.2rem;
  text-decoration: none;
  color: var(--color-dark-grayish-blue);
  transition: background-color 0.25s;
}

.notification__private-message:hover {
  cursor: pointer;
  background-color: var(--color-light-grayish-blue-1);
}

@media only screen and (width >=1024px) {
  .main {
    border-radius: 15px;
    max-width: 73rem;
    padding: 3.3rem 3rem 0;
  }

  .notification {
    grid-template-columns: 45px 1fr;
    margin-bottom: 0.8rem;
  }

  .notification--profile-pic {
    grid-template-columns: 45px 1fr 45px;
  }

  .notification__avatar {
    width: 45px;
    height: 45px;
  }
}
</style>
