<template>
  <div class="container">
    <NuxtPage />
  </div>
</template>

<style lang="scss">
@import '@compromis/blobby/scss/blobby';

body {
  font-weight: 500;
}

.card-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 3.5rem;
  margin-top: 2rem;

  .card {
    position: relative;
    min-height: 21rem;
    display: flex;
    border-radius: 1.5rem !important;

    .card-content {
      display: flex;
      flex-direction: column;
      height: 100%;
      flex-grow: 1;
    }

    &.card-padded {
      padding: 2.25rem;
    }

    h2 {
      font-weight: 700;
      width: fit-content;
      letter-spacing: -.02em;
      padding-bottom: 1rem;
      margin-bottom: auto;
      font-size: 2.25rem;
    }

    p {
      max-width: 50ch;
    }

    &.even {
      text-align: right;
      padding-left: 200px;

      h2,
      p {
        margin-left: auto;
      }
    }

    &.odd {
      padding-right: 200px;
    }
  }

  .card p:last-child {
    margin-bottom: 0;
  }

  .icon {
    position: absolute;
    top: 55%;

    img {
      width: 200px;
      transform: translateY(-50%);
    }

    &.calculator {
      right: -2rem;
    }

    &.piggy {
      left: -4rem;

      img {
        width: 240px;
      }
    }

    &.heart {
      right: -2rem;

      img {
        transform: translateY(-50%) scaleX(-1);
      }
    }

    &.crayons {
      left: -3rem;
      top: 70%;

      img {
        width: 150px;
      }
    }

    &.train {
      top: auto;
      right: -5rem;
      bottom: -6rem;

      img {
        width: 340px;
        transform: none;
      }
    }
  }
}

.container {
  padding: 2rem;
  max-width: 1000px;
}

.header {
  .compromis-logo {
    margin-bottom: 3rem;

    svg {
      width: 200px;
    }
  }

  .site-title {
    font-weight: 500;
    padding-bottom: 1rem;
    line-height: 1;
    margin-bottom: 1.5rem;
  }

  .language-link {
    margin-left: auto;
  }
}

.sign {
  margin-top: 5rem;
  text-align: center;
}

.button-primary {
  display: inline-flex;
  background: $gradient-primary;
  color: $white;
  margin-bottom: 2rem;
  padding: .75em 2em;
  border-radius: 2rem;
  font-size: $text-xl;
  transition: .2s ease;
  align-items: center;

  img {
    height: 1em;
    margin-right: .5em;
  }

  &:hover {
    color: $white;
    text-decoration: none;
    box-shadow: $shadow-raised;
    transform: translateY(-.2em);
  }
}

.from-purple {
  --gradient-start: #5c439a;
}

.to-blue {
  --gradient-end: #50b2e4;
}

.from-magenta {
  --gradient-start: #db2b60;
}

.to-plum {
  --gradient-end: #90298b;
}

@include media-breakpoint-down(md) {
  .container {
    padding: 1rem;
  }

  .header {
    .site-title {
      font-size: 3.75rem !important;
    }
  }

  .card-grid {
    margin-top: 3rem;
    gap: 6rem;

    .card {
      &.card-padded {
        padding: 120px 1.5rem 1.5rem;
      }

      &.odd {
        padding-right: 1.5rem;
      }

      &.even {
        padding-left: 1.5rem;
        text-align: left;

        h2 {
          margin-left: 0;
        }
      }

      .icon {
        top: -2.5rem;
        left: 50%;
        right: auto;
        bottom: auto;
        transform: translate(-50%, 0) !important;

        img {
          transform: none;
          width: auto;
          height: 150px;
        }
      }
    }
  }

  .form {
    height: 2900px;
  }
}
</style>
