<template>
  <section class="welcome" ref="welcome">
    <div class="column">
      <h1>THE ZONE</h1>
      <h3>WELCOME TO THE ZONE -</h3>
      <div class="welcome-text">
        <p>
          All of us are here in this space because we are adopters,
          experimentalists and no doubt early believers; but what do we truly
          believe? At Sol Vibez, we believe in embracing the Web3.0 ethos
          wholeheartedly, and to us that means to be <b>connected</b>, to have
          <b>fun</b> and ultimately to achieve <b>decentralization</b>.
        </p>
        <p>
          Talented, creative and passionate individual(s) that are like-minded
          and are willing to contribute to co-create a collective experience
          together are highly sought after, as it is our belief that there is no
          “ONE” leader and that the growth of the Sol Vibez brand will
          eventually be community driven.
        </p>
        <p>
          It is this foundation and belief that we can achieve decentralization
          via Web3.0 technology that forms the very basis of everything we do at
          Sol Vibez. In order to materialize this goal, our team's primary focus
          will be to facilitate the initial growth of Sol Vibez, engage
          like-minded souls, initialize and fulfil the line-up and establish the
          foundation.
        </p>
        <p>Le's get ready to Vibez.</p>
      </div>
    </div>
    <div class="column image-col">
      <img src="../assets/Welcome-Zone.jpg" alt="An Artist's Welcome" />
    </div>
  </section>
  <section class="line-up">
    <h2>LINE-UP</h2>
    <div><img src="../assets/Line-up.png" alt="Line-Up Graphic" /></div>
    <div class="line-up-grid">
      <div class="column">
        <div class="item">
          <h3>SEEDING</h3>
          <p>
            We respect the hustle and grind, but Sol Vibez aims to cultivate and
            establish partnerships with prominent projects, be it mature or
            upcoming; to allow our community to benefit from this synergy. To
            provide our community a breather from all this fast-moving space.
          </p>
        </div>
        <div class="item">
          <h3>CONNECT IRL</h3>
          <p>
            One of the goals is to proliferate our community’s circle.<br />
            We believe the majority of us are not necessarily here to use the
            digital space as a means to escape, but rather, to connect. Sol
            Vibez aims to be a platform that fundamentally connects people to
            themselves and with one another from their on-chain to their
            off-chain equivalent.
          </p>
          <p>
            We will explore different possible initiatives to allow our
            community to participate in and eventually establish valuable IRL
            connections.
          </p>
        </div>
      </div>
      <div class="column">
        <div class="item">
          <h3>COLLATERAL</h3>
          <p>
            Sol Vibez will plan to launch a strategic collection of collateral
            that not only include garments but also a plethora of accessories.
            More will be revealed in due time, all we can say for now is that
            the collection will be of quality as we care deeply about not only
            the users, but how the brand is being represented.
          </p>
          <p>Let’s all swag out with vibez!</p>
        </div>
        <div class="item">
          <h3>By Sol Vibez for Sol Vibez</h3>
          <p>
            At Sol Vibez we believe in embracing Web3.0 ethos and that there is
            no “ONE” leader. We aim to bootstrap digital identity, governance
            and treasury that can be used by the entire community.
          </p>
          <p>
            Sol Vibez treasury will be set up as a multi-signature wallet. This
            means that spending whatever assets in that wallet will require more
            than one sign-off for the transaction to go through. Signer(s) for
            the multi-signature wallet will be chosen from and by the community.
            This will ensure the long-term growth and prosperity of Sol Vibez to
            be always community driven.
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
          From humble beginnings, an entrepreneur and investor of various
          start-ups. Breathes life into visions and concepts. Believes
          knowledge, connections and friendships are irreplaceable assets.
        </p>
      </div>
      <div class="member">
        <div><img src="../assets/pfp-tnon.png" alt="T.Non's Picture" /></div>
        <h3 class="member-name">T.Non</h3>
        <div class="member-title">Project Manager</div>
        <p class="member-desc">
          Experience in various industries ranging from project management to
          logistic trade; with the ability to adapt, analyze and provide
          solutions. An undeniable jack-of-all-trades.
        </p>
      </div>
      <div class="member">
        <div><img src="../assets/pfp-artist.png" alt="Artist's Picture" /></div>
        <h3 class="member-name">P.BELLUM</h3>
        <div class="member-title">Artist</div>
        <p class="member-desc">
          Background in gaming design and a self-taught illustrator. First foray
          into non-fungible tokens. With an eye for details; elements
          materialzed will be highly relatable with references from various
          cultures.
        </p>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
p:not(:last-child) {
  margin-bottom: 18px;
}

img {
  object-fit: contain;
  max-width: 100%;
  max-height: 100%;
}

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
          margin-bottom: 20px;
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
        font-size: 34px;
      }
      .member-title {
        margin-bottom: 20px;
        font-weight: bold;
        font-size: 20px;
        font-family: 'Minion Condensed', Georgia, 'Times New Roman', Times,
          serif;
      }
    }
  }
}

// ---- Mobile Styles
@media (max-width: 1024px) {
  section {
    padding: 0 var(--side-padding-mobile);
    padding-top: 4vh;
    h3 {
      margin-bottom: 12px;
    }
    p {
      font-size: 18px;
    }

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
          margin-bottom: 0;
          line-height: 48px;
        }
        .member-title {
          margin-bottom: 14px;
          font-size: 18px;
        }
      }
    }
  }
}
</style>
