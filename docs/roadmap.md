# Studio Roadmap & Setup Backlog

A living list of studio/infra todos, ordered so we don't polish the storefront
before the game is worth showing. **The game comes first** — everything below
the dev work is in service of it, not a substitute for it.

> Status: prototype. Bones are in place; the priority is making the core loop
> *fun*, then UI, then assets/music.

## 🎮 The game (always priority #1)

- [ ] **Make the core loop fun.** Nothing below matters until a playtest is
      genuinely fun. Keep iterating on the moment-to-moment co-op experience.
- [ ] **UI** — flagged as the most pressing need after core dev. Biggest
      "feels like a real game" multiplier for the least money; tractable solo or
      with cheap asset packs.
- [ ] **Art assets** — can lean on asset packs / freelancers; don't need final
      art to keep playtests fun.
- [ ] **Music & SFX** — same; placeholder/licensed audio is fine early.

## 🌱 Community (low effort, compounds in the background)

- [ ] **Discord server** — start small whenever; it grows for free. Wire-up
      ready on our side (badge, SUPPORT link, release auto-announcer) — just
      need the invite URL + webhook.
- [ ] **itch devlog** — keep posting build updates; cheap visibility.
- [ ] **Email list** — capture interested players for launch day (third-party
      embed; GitHub Pages can't host a form backend).

## 🌐 Website — GitHub Pages *(parked: build once the game is presentable)*

A single static landing page is the right scope. Gated on having decent UI/art
+ a trailer-worthy clip so it makes a good first impression.

- **Decision made:** custom domain **moralsupportstudios.com** (already owned for
  email). Point it at GitHub Pages with free HTTPS when we build.
- **Decision deferred:** build tooling (hand-written HTML vs. a static-site
  generator) — choose at build time.
- **Repo:** not created yet. Likely a `moralsupportstudios.github.io` org site
  repo when the time comes.
- Planned content: hero + gameplay clip, "Play on itch" + "Join Discord" CTAs,
  "Wishlist on Steam" (when live), about/studio, support/contact.

## 🛒 Storefront — Steam *(parked: needs art + trailer)*

- [ ] See [steam-launch-prep.md](./steam-launch-prep.md). Do **after** the
      website exists so wishlist traffic has a polished home. Wishlists are the
      key pre-launch metric — but only worth driving once there's a trailer.

## ✅ Already set up (org infra)

- Org-wide community health files (CONTRIBUTING, CODE_OF_CONDUCT, SECURITY,
  SUPPORT) + default issue/PR templates.
- [Org settings guide](./org-settings-guide.md), [payments &
  monetization](./payments-and-monetization.md), [Steam
  prep](./steam-launch-prep.md).
- Discord release-announcer workflow template (needs a webhook secret to
  activate).
