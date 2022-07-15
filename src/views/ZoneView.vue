<template>
  <section class="welcome" ref="welcome">
    <div class="column">
      <h1>The Zone</h1>
      <h3>Welcome to the Zone -</h3>
      <div class="welcome-text">
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae nihil
          quam quas maiores deleniti sunt minus cumque illo perferendis tenetur
          dolore, tempora minima atque modi consequatur! Mollitia corporis
          molestias sunt voluptatem ipsam libero optio aliquid!
        </p>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae nihil
          quam quas maiores deleniti sunt minus cumque illo perferendis tenetur
          dolore, tempora minima atque modi consequatur! Mollitia corporis
          molestias sunt voluptatem ipsam libero optio aliquid!
        </p>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae nihil
          quam quas maiores deleniti sunt minus cumque illo perferendis tenetur
          molestias sunt voluptatem ipsam libero optio aliquid!
        </p>
        <p>Let's get ready to vibez.</p>
      </div>
    </div>
    <div class="column image-col">
      <img src="../assets/Welcome-Zone.jpg" alt="An Artist's Welcome" />
    </div>
  </section>
  <section class="line-up">
    <h2>Line-Up</h2>
    <div><img src="../assets/Line-up.png" alt="Line-Up Graphic" /></div>
    <div class="line-up-grid">
      <div class="column">
        <div class="item">
          <h3>Seeding</h3>
          <p>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Totam ex
            repellendus minus soluta asperiores, aliquid expedita iure qui earum
            tenetur eius sint iste sapiente quibusdam? Ipsa voluptas quidem
            pariatur amet?
          </p>
        </div>
        <div class="item">
          <h3>Connect IRL</h3>
          <p>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Totam ex
            repellendus minus soluta asperiores, aliquid expedita iure qui earum
            tenetur eius sint iste sapiente quibusdam? Ipsa voluptas quidem
            pariatur amet?
          </p>
        </div>
      </div>
      <div class="column">
        <div class="item">
          <h3>Collateral</h3>
          <p>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Totam ex
            repellendus minus soluta asperiores, aliquid expedita iure qui earum
            tenetur eius sint iste sapiente quibusdam? Ipsa voluptas quidem
            pariatur amet?
          </p>
        </div>
        <div class="item">
          <h3>By Sol Vibez for Sol Vibez</h3>
          <p>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Totam ex
            repellendus minus soluta asperiores, aliquid expedita iure qui earum
            tenetur eius sint iste sapiente quibusdam? Ipsa voluptas quidem
            pariatur amet?
          </p>
        </div>
      </div>
    </div>
  </section>
  <section class="team">
    <h2>Team</h2>
    <div class="team-list">
      <div class="member">
        <div><img src="../assets/pfp-satin.png" alt="Satin's Picture" /></div>
        <h3 class="member-name">Satin</h3>
        <div class="member-title">Conceptualist</div>
        <p class="member-desc">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusantium
          rem, neque cum harum dignissimos sed obcaecati voluptates quas odio
          consequatur eveniet aperiam, suscipit, autem consectetur!
        </p>
      </div>
      <div class="member">
        <div><img src="../assets/pfp-tnon.png" alt="T.Non's Picture" /></div>
        <h3 class="member-name">T.Non</h3>
        <div class="member-title">Project Manager</div>
        <p class="member-desc">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusantium
          rem, neque cum harum dignissimos sed obcaecati voluptates quas odio
          consequatur eveniet aperiam, suscipit, autem consectetur!
        </p>
      </div>
      <div class="member">
        <div><img src="../assets/pfp-artist.png" alt="Artist's Picture" /></div>
        <h3 class="member-name">Artist</h3>
        <div class="member-title">Artist</div>
        <p class="member-desc">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusantium
          rem, neque cum harum dignissimos sed obcaecati voluptates quas odio
          consequatur eveniet aperiam, suscipit, autem consectetur!
        </p>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
section {
  padding: 0 var(--side-padding);
  padding-top: 10vh;
  h1 {
    margin-bottom: 10px;
  }
  min-height: 90vh;
  &.welcome {
    display: grid;
    grid-template-columns: 4fr 3fr;
    column-gap: 20px;
    .column {
      height: 100%;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      &.image-col {
        justify-content: flex-end;
      }
    }
    .welcome-text {
      justify-self: flex-end;
      p {
        margin: 18px 0;
      }
    }
  }
  &.line-up {
    img {
      max-width: 98vw;
      margin-left: calc(var(--side-padding) * -1);
    }
    .line-up-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      column-gap: 50px;
      margin: 0 40px;
      .item {
        margin-bottom: 50px;
        h3 {
          margin-bottom: 14px;
        }
      }
    }
  }
  &.team {
    .team-list {
      display: flex;
      flex-direction: row;
      column-gap: 80px;
      text-align: center;
      .member-name {
        margin-top: 12px;
      }
      .member-title {
        margin-bottom: 20px;
        font-size: 16px;
        font-family: Georgia, 'Times New Roman', Times, serif;
      }
    }
  }
}

img {
  object-fit: contain;
  max-width: 100%;
  max-height: 100%;
}
p {
  font-weight: 200;
  font-family: Georgia, 'Times New Roman', Times, serif;
}

// ---- Mobile Styles
@media (max-width: 1024px) {
  section {
    padding: 0 var(--side-padding-mobile);
    padding-top: 4vh;

    &.welcome {
      padding-top: 10vh;
      display: flex;
      flex-direction: column;
      .column {
        order: 1;
        &.image-col {
          order: 0;
          height: 45vh;
        }
      }
    }
    &.line-up {
      img {
        margin-left: calc(var(--side-padding-mobile) * -1);
      }
      .line-up-grid {
        display: flex;
        flex-direction: column;
        margin: 0 5px;
        .item {
          margin-bottom: 24px;
          h3 {
            margin-bottom: 8px;
          }
        }
      }
    }
    &.team {
      .team-list {
        display: flex;
        flex-direction: column;
        row-gap: 20px;
        .member-name {
          margin-top: 8px;
        }
        .member-title {
          margin-bottom: 14px;
        }
      }
    }
  }
}
</style>
