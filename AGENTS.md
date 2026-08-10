# AGENTS.md — Website editing rules

Shared instructions for AI assistants (Claude Code, Codex, and any reviewer)
working on this academic research website. Claude Code also loads these rules via
`CLAUDE.md`, which imports this file, so both tools follow one source of truth.

---

## Website editing rules
- Purpose: academic research website with credible applied relevance.
- Audience: academic hiring committees, research collaborators, policy and industry readers.
- Never invent publications, affiliations, awards, job titles, data, results, or collaborators.
- Preserve factual distinctions: published, accepted, under review, working paper, and work in progress.
- Use concise scholarly English.
- Voice: write on-page site copy (bio, research, project descriptions) in the first person
  ("I am a doctoral candidate…"). Exceptions kept in third person: the SEO meta description
  in `config/_default/params.yaml` and the repo `README.md`.
- Do not edit deployment, build, or configuration files unless explicitly asked.
- Before substantial edits, identify the files to change and briefly explain the proposed changes.
- Keep the homepage focused on three themes (for now):
  1. Economics of decarbonization technologies (e.g. green hydrogen etc).
  2. Carbon accounting and investment incentives
  3. Carbon removal portfolios

---

## Proposed additions (review and trim — not yet ratified by the owner)

### Facts and source of truth
- The canonical record of facts is the LaTeX CV at `../CV PH 2026.tex`. It wins on any
  conflict over publications, affiliations, titles, dates, and contact details. The
  cover letter and research/teaching statements are secondary inputs.
- Map publication status from the CV's own sections and labels:
  - *Peer-Reviewed Articles* → "published" (with year/venue) or "forthcoming/accepted"
    when the CV says so. Do not call a forthcoming paper "published."
  - *Working Papers* → "working paper"; clearly separate "work in progress" where noted.
- Do not reorder author lists. Author order (often alphabetical in economics/accounting)
  is meaningful — reproduce the CV order exactly.
- Preserve authorship markers (e.g. the `*` denoting lead/equal contribution in the CV).
- If a fact is missing, ambiguous, or you are tempted to "round up," ask — do not fill the gap.

### Content hygiene
- This is a cloned template. Remove all demo/placeholder content before anything is public:
  the sample DeepMind biography, the `pandas`/`pytorch`/`scikit` demo projects, the sample
  blog posts, the "Build your own academic website" CTA card, and HugoBlox promo copy.
- Never leave template lorem-ipsum or placeholder text on a live page.

### Tone and style
- Factual scholarly English. Avoid marketing language, superlatives, and hype — the
  template's default copy is promotional; strip that voice.
- Pick one English variety (British or American) and keep it consistent site-wide.
- Keep date and number formats consistent across pages.

### Privacy
- The site is public and indexed by search engines and AI crawlers. Treat every committed
  file as world-readable.
- Default to the institutional email and institutional address. Do not publish a private
  phone number or home address unless explicitly asked.

### Process and scope
- "Configuration / build / deployment files" you must not touch without being asked include:
  `config/`, `hugoblox.yaml`, `netlify.toml`, `go.mod`, `package.json`, `pnpm-lock.yaml`,
  and everything under `.github/`.
- Do not run `git push`, trigger a deploy, or change the deploy host without explicit instruction.
  Deployment is automated (push to `main` → `.github/workflows/deploy.yml`).
- Only use images/assets the owner has the rights to use; provide descriptive alt text.

---

## Working with this repo (orientation)
- Stack: Hugo Extended + HugoBlox "Academic CV" template. Page content lives as Markdown
  under `content/`; site behaviour and theming under `config/_default/`.
- Homepage is composed of "blocks" in `content/_index.md`. The author/bio profile is the
  folder referenced by `username:` there (`content/authors/me/`).
- Local preview: `pnpm install`, then `hugo server` (or `pnpm dev`). Pinned Hugo version is
  in `hugoblox.yaml` (`0.162.0`).
- Deployment: automated GitHub Pages build on push to `main`. Host is set in `hugoblox.yaml`.

## Review workflow (Claude drafts → Codex/second-pass reviews)
A reviewer pass (Codex, or a fresh Claude read) should check, in priority order:
1. Factual accuracy against `../CV PH 2026.tex`.
2. Correct publication-status labels (published vs forthcoming vs working paper vs WIP).
3. No template placeholder/demo content remains.
4. Tone is scholarly and non-promotional; English variety is consistent.
