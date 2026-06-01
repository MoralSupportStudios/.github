# Org Settings Setup Guide

A checklist for hardening and organizing the **Moral Support Studios** GitHub
org. These are dashboard settings that can't be set from a repo — links and
click-paths are provided so you can knock them out quickly.

> Org settings live at: `https://github.com/organizations/MoralSupportStudios/settings`

## 1. Security (do these first)

- [ ] **Require two-factor auth for everyone.**
  Settings → *Authentication security* → check **Require two-factor
  authentication for everyone in the organization**.
  ⚠️ Members without 2FA are removed when you enable this — make sure your own
  account has 2FA on first.
- [ ] **Enable private vulnerability reporting org-wide.**
  Settings → *Code security* → enable **Private vulnerability reporting** for
  new and existing repos. (Pairs with the `SECURITY.md` already in this repo.)
- [ ] **Enable Dependabot alerts & secret scanning** for all repos.
  Settings → *Code security* → turn on **Dependabot alerts** and **Secret
  scanning** (free on public repos).

## 2. Member permissions

- [ ] **Set base permissions to "Read"** (not Write).
  Settings → *Member privileges* → **Base permissions: Read**. Grant Write/Admin
  per-repo or per-team instead of org-wide.
- [ ] **Restrict repo creation** to owners (or owners + specific teams) while the
  org is small. Settings → *Member privileges* → *Repository creation*.
- [ ] **Restrict who can delete/transfer repos** to owners.

## 3. Teams

Create teams so you can @-mention groups and manage access in bulk:
`https://github.com/orgs/MoralSupportStudios/teams`

- [ ] **`@core`** — you (and any future collaborators); Write/Admin on game repos.
- [ ] **`@playtesters`** — trusted testers; Triage access (can label/assign issues
  but not push).
- [ ] *(later)* **`@contributors`** — outside contributors who've earned write to
  specific repos.

## 4. Branch protection (per repo, e.g. Space-Game)

Repo → Settings → *Branches* → add a rule for the default branch:

- [ ] **Require a pull request before merging.**
- [ ] **Require status checks to pass** (once you have CI).
- [ ] **Require branches to be up to date before merging.**
- [ ] Optionally **block force-pushes** to the default branch.

> Even solo, PR-only merging gives you a clean history and a place for CI to run.

## 5. Community

- [ ] **Enable Discussions** on Space-Game for non-bug community chat
  (questions, "looking for crew", show-and-tell). Repo → Settings → *Features* →
  **Discussions**.
- [ ] **Verify the org's community profile** is green: each repo should show
  README, CODE_OF_CONDUCT, CONTRIBUTING, etc. — the org defaults in this `.github`
  repo cover repos that don't define their own.

## 6. Profile

- [ ] Add an **org logo/avatar** and a short bio + the itch.io URL on the org
  profile page. Settings → *Profile*.
