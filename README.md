# Awesome PM Skills

A curated set of AI agent skills for product managers who care about taste, judgment, and shipping docs that don't sound like AI wrote them.

## Skills in this repo

### 1. [`grill-prd`](./skills/grill-prd/) — by [Vinod Iyengar](https://www.linkedin.com/in/vinodiyengar)

Relentless product interview before you write a PRD, one-pager, or launch memo. Batched themed questions, fuzzy-language challenges, then a sharp TL;DR memo plus a full PRD only after you say you're ready.

Install / invoke: copy `skills/grill-prd` into your agent skills folder, then run `/grill-prd`.

Interview discipline adapted from Matt Pocock's grilling pattern ([mattpocock/skills](https://github.com/mattpocock/skills)).

### 2. [`human-review`](./skills/human-review/) — by [Peter Yang](https://github.com/petergyang)

Visual review for HTML and Markdown: edit like a Google Doc, leave comments, send batched feedback to your agent. Great for PRDs, landing pages, and product copy.

Upstream (use this for install): [petergyang/human-review](https://github.com/petergyang/human-review)

```bash
npx -y human-review setup --global
```
Then: `/human-review your-file.md`

This repo keeps a short pointer skill so PMs can discover it next to grill-prd. The full tool lives in Peter's repo.

## Why these two

Most PM skills help you fill a template.

These two are daily practices for judgment:

1. **Grill first**  force the decision tree before the document exists.
2. 2. **Review like a human** — edit and comment on the artifact itself instead of describing edits in chat.
  
   3. ## Credits
  
   4. - **Matt Pocock** — [`/grill-me`](https://github.com/mattpocock/skills) and the grilling interview pattern that `grill-prd` builds on.
      - - **Peter Yang** — [`/human-review`](https://github.com/petergyang/human-review) for visual, human-in-the-loop document review.
        - - **Vinod Iyengar** — `grill-prd` and this curated collection.
         
          - Related cousins worth knowing (not vendored here):
         
          - - [artificialguybr/grill-me-product](https://github.com/artificialguybr/grill-me-product) — founder/idea grill (market, CAC/LTV, positioning)
            - - [unsoldgroup/flesh-out-product-skill](https://github.com/unsoldgroup/flesh-out-product-skill) — grill → domain model → tickets
             
              - ## License
             
              - MIT for original content in this repo (`grill-prd`, README curation).
             
              - `human-review` remains owned by Peter Yang under its upstream MIT license — install from [petergyang/human-review](https://github.com/petergyang/human-review).
              - 
