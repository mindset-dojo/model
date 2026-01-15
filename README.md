## 🥋 The Dojo

The Dojo is an open-source reference architecture for making transformation practices, lived experience, and stewardship visible during complex change.

The architecture reflects the emerging Circle~Dojo organizational change pattern, which is being developed with the intent of submission to [Pattern Languages of Programs, People & Practices](https://plopcon.org/) and will be linked or included here when complete.

If you’d like a gentle way to explore, fork this repository, publish it with GitHub Pages, and create a simple practitioner card and first Story.

### Quickstart: run your fork on GitHub Pages

1. **Fork** this repository.
2. In your fork, open **Settings → Pages** and set **Source** to the `main` branch and the `/` (root) directory.
3. Wait for the Pages build to finish, then visit `https://<username>.github.io/dojo` to confirm it is live.
4. Prefer an in-browser workspace? Use **GitHub Codespaces** from the repository header to edit without installing anything locally.

#### Troubleshooting

| Symptom | Fix |
| --- | --- |
| Build fails with CNAME error | Remove or update `CNAME` if you do not use a custom domain. |
| Custom domain not resolving | Allow DNS to propagate; keep `CNAME` aligned with your domain. |
| Jekyll/front matter error | Ensure front matter blocks start/end with `---` and use valid YAML keys. |

### Become a practitioner: card + first Story

Share who you are and what you are practicing by shipping both a practitioner card and a first Story.

1. Add your practitioner card under `_practitioners/` with your slug, e.g., `_practitioners/alex-doe.md`:

   ```yaml
   ---
   layout: threshold
   sections_key: practitioner
   name: Alex Doe
   description: Short bio sentence.
   title: "What you repeat, you become"
   title_mark: Repeat
   icon: fa-solid fa-infinity
   active: true
   join_date: 2025-01-01
   progression_level: -8
   progression_level_date: 2025-06-01
   about: |
     ### Summary

     A short paragraph on who you are and what you are practicing.

     ### Connect

     - [Email](mailto:alex@example.com)
     - [LinkedIn](https://linkedin.com/in/alexdoe)
   ---

   ```

   - Mirror any additional optional fields you see in existing practitioner cards to stay consistent.
2. Create your first Story under `_stories/<year>/<your-slug>/`, e.g., `_stories/2025/alex-doe/2025-06-15-beginner-mind.md`:

   ```yaml
   ---
   layout: story
   title: Your Story Title
   title_mark: Optional short marker
   published_date: 2025-06-15
   refactored_date: 2025-06-15
   practitioners:
     - alex-doe
   practices:
     - threshold
   excerpt: |
     One or two sentences that invite the reader in.
   ---

   ```

   - Keep the tone reflective, practice-oriented, and Markdown-first.
3. Commit and push; GitHub Pages will render your practitioner card and publish your Story on the next build.

### Preview in Codespaces

Run the site directly in your Codespace:

```bash
bundle install
bundle exec jekyll serve --host 0.0.0.0 --port 4000 --livereload
```

- Forward port 4000 in the Ports tab and open it in the browser to view the site.

### Local preview (optional)

If you prefer to preview locally:

```bash
bundle install
bundle exec jekyll serve
```

- Requires Ruby and Bundler. If you use `rbenv` or `asdf`, align with the version pinned in `Gemfile.lock`.
- Preview is served at <http://localhost:4000>.

### Project anatomy

- `_practitioners/` practitioner cards
- `_stories/` Story articles by year/practitioner
- `_practices/` practice entries
- `_areas/` domain areas (e.g., DevOps, Platform)
- `_layouts/` page templates and `_includes/` shared components
- `_data/` structured site data
- `mission.md` front matter for the home (mission) landing page

### Community norms

- Small, focused pull requests make review easy.
- Be direct, respectful, and mission-aligned: reflective, practice-ready, and action-oriented.
- See [LICENSE](LICENSE.md) for reuse expectations.
