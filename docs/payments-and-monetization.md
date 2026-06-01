# Payments & Monetization

Goal: **every payout routes to the Moral Support Studios LLC business bank
account** (the one tied to your EIN). Each platform handles payouts in its own
dashboard, so this is a per-platform connect-the-account task. Use the same
business bank account everywhere for clean bookkeeping.

> None of this can be configured from GitHub — these are settings inside each
> platform, using your logins. Steps are listed so you can do them quickly.

## Where money can come in (current stage)

| Channel | Effort | Obligation | Recommended now? |
| --- | --- | --- | --- |
| **itch.io** "pay what you want" / donations | Low | None | ✅ Yes |
| **Ko-fi** tip jar | Low | None | ✅ Yes |
| **GitHub Sponsors** | Low | Light | Optional (good if devs follow you) |
| **Patreon** | High | Monthly perks expected | ⏳ Wait until there's demand |
| **Steam** sales | High | Full store page | ⏳ When the game is ready |

## Connect each payout to the LLC bank account

### itch.io
1. Account → **Settings → Payouts** (or Get Paid).
2. Connect **PayPal** or **Stripe** under the LLC. Route that PayPal/Stripe to
   the business bank account tied to your EIN.
3. On the Space-Game project page → **Pricing** → set **"$X or donate"** / "pay
   what you want" so people *can* tip without it gating the build.

### Ko-fi
1. Create the page as the **business** (use studio name).
2. **Settings → Payments** → connect **Stripe** (instant) and/or PayPal, both
   pointing at the LLC bank account.
3. Add the Ko-fi link to `FUNDING.yml` and the README (I can do this — just send
   the handle).

### GitHub Sponsors (optional)
1. `https://github.com/sponsors` → join as the **organization**
   (MoralSupportStudios), not your personal account, so it's under the LLC.
2. Complete Stripe Connect with the business bank + EIN tax info.
3. Uncomment `github:` in `.github/FUNDING.yml`.

### Steam (later)
See [steam-launch-prep.md](./steam-launch-prep.md) — Steamworks payout uses the
business bank + W-9 under the EIN.

## Bookkeeping tips

- Keep **all** revenue flowing into the one business account; pay business
  expenses (Steam fee, software, art commissions) from it too — clean records
  for taxes.
- Save platform payout reports monthly (itch, Ko-fi, Steam all export CSVs).
- Talk to an accountant once revenue is real; an LLC's tax treatment varies.
