<template>
  <div class="logo">
    <h1><span>ChienLe</span></h1>
    <h2 class="yellow">PTN</h2>
    <h3>
      Web Development
    </h3>
    <h3 class="secondh3">Tools</h3>
    <h4>
      Collection of useful programs and scripts
    </h4>
    <h4 class="secondh4">
      to interact with laravel.
    </h4>
  </div>
</template>

<style lang="scss" scope>
.logo {
  padding-top: 1.5rem;
  height: 23rem;
  h1 {
    text-align: center;
    font-size: 10rem;
    text-transform: uppercase;
    font-weight: 900;
    letter-spacing: -0.9rem;
    position: relative;
  }
  h2 {
    text-align: center;
    position: relative;
    top: -9rem;
    left: 15.3rem;
    z-index: -1;
    font-size: 10rem;
    opacity: 1;
  }
  h3 {
    text-align: center;
    left: 15.5rem;
    top: -11rem;
    font-size: 2.5rem;
    text-transform: uppercase;
    font-weight: 600;
    line-height: 1;
    position: relative;
    overflow: hidden;
  }
  .secondh3 {
    left: 19.7rem;
    top: -12rem;
  }
  h4 {
    text-align: center;
    left: 15.5rem;
    top: -12.4rem;
    font-size: 0.8rem;
    font-weight: 500;
    position: relative;
    overflow: hidden;
    line-height: 1;
  }
  .secondh4 {
    left: 18.2rem;
  }
}
@media screen and (max-width: 800px) {
  .logo {
    height: 21rem;
    h1 {
      font-size: 8rem;
      letter-spacing: -0.7rem;
    }
    h2 {
      font-size: 8rem;
      letter-spacing: -0.5rem;
      top: -7.5rem;
      left: 11.3rem;
    }
    h3 {
      left: 11.5rem;
      top: -9.5rem;
      font-size: 1.5rem;
    }
    .secondh3 {
      left: 14rem;
      top: -10rem;
    }
    h4 {
      left: 8rem;
      top: -10rem;
      font-size: 0.8rem;
    }
    .secondh4 {
      left: 10.8rem;
    }
  }
}
@media screen and (max-width: 640px) {
  .logo {
    height: 16rem;
    h1 {
      font-size: 6rem;
      letter-spacing: -0.6rem;
    }
    h2 {
      font-size: 6rem;
      letter-spacing: -0.3rem;
      top: -5.6rem;
      left: 8.55rem;
    }
    h3 {
      left: 9rem;
      top: -7.2rem;
      font-size: 1.3rem;
    }
    .secondh3 {
      left: 11.2rem;
      top: -7.8rem;
    }
    h4 {
      left: 5rem;
      top: -8rem;
      font-size: 0.8rem;
    }
    .secondh4 {
      left: 7.7rem;
    }
  }
}
@media screen and (max-width: 470px) {
  .logo {
    height: 15rem;
    h1 {
      font-size: 5rem;
      letter-spacing: -0.5rem;
    }
    h2 {
      font-size: 5rem;
      letter-spacing: -0.25rem;
      top: -5rem;
      left: 7.1rem;
    }
    h3 {
      left: 7.2rem;
      top: -6.5rem;
      font-size: 1.1rem;
    }
    .secondh3 {
      left: 9rem;
      top: -6.9rem;
    }
    h4 {
      left: 2.5rem;
      top: -6.8rem;
      font-size: 0.8rem;
    }
    .secondh4 {
      left: 5.2rem;
    }
  }
}
@media screen and (max-width: 400px) {
  .logo {
    height: 13rem;
    h1 {
      font-size: 4rem;
      letter-spacing: -0.35rem;
    }
    h2 {
      font-size: 4rem;
      letter-spacing: -0.25rem;
      top: -4rem;
      left: 5.65rem;
    }
    h3 {
      left: 5.8rem;
      top: -5.3rem;
      font-size: 1.1rem;
    }
    .secondh3 {
      left: 7.6rem;
      top: -5.7rem;
    }
    h4 {
      left: 1.2rem;
      top: -5.5rem;
      font-size: 0.8rem;
    }
    .secondh4 {
      left: 3.9rem;
    }
  }
}
</style>

<script>
import { gsap } from "gsap";
export default {
  name: "Logo",
  activate() {
    gsap.from(".logo h1", {
      duration: 1.5,
      delay: 1,
      y: "100%",
      ease: "expo.inOut",
    });

    gsap.from(".logo h3", {
      duration: 1.5,
      delay: 1.2,
      y: "400%",
      ease: "expo.inOut",
    });

    gsap.from(".logo h4", {
      duration: 1.5,
      delay: 1.3,
      y: "600%",
      ease: "expo.inOut",
    });

    gsap.from(".logo h2", {
      duration: 1.5,
      delay: 1.5,
      opacity: 0,
      x: "-10000",
      ease: "expo.inOut",
    });
  },
};
</script>
