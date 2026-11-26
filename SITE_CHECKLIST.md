# Website checklist

## A. Get it live (about 10 minutes)
- [ ] Repo is named exactly `saksham132.github.io` (or your current GitHub username + `.github.io`) so the site lives at the root URL
- [ ] Fix the deploy workflow: delete `.github/workflows/jekyll-gh-pages.yml` (the old one is broken) and set Settings → Pages → Source to "Deploy from a branch" → `main` / root
- [ ] Commit and push; watch Settings → Pages (or the Actions tab) for the first build and any red errors
- [ ] Open the live URL on your laptop and your phone

## B. Check the facts on every page
**About**
- [ ] "Started in the lab in April 2025 and joined the program that September" reads right to you
- [ ] Photo: happy with it as the public headshot?
- [ ] Add anything you want here: a "Now" line, research one-liner, or what you're looking for

**Research**
- [ ] Cell Reports citation: author order and PMID 41004338 against PubMed (I got them from a Fred Hutch news page, not PubMed)
- [ ] Advisor names and dates: Shendure (Apr 2025 –), Setty (Sep – Dec 2025), Berger (2022; 2023 – 2025), Zafar (2021 – 2022)
- [ ] Research intro paragraph describes your work the way you would; I only know your PhD work in general terms
- [ ] Shendure Lab entry: add 1 or 2 lines on the RNA / aptamer side if you want it public
- [ ] Unpublished work: confirm you're comfortable with what the Shendure Lab entry reveals (insertion library, FACS enrichment)
- [ ] CV link points to the OLD pdf: replace it (see C)

**Non-research**
- [ ] Add your role and a sentence for Sunday Science and the GS Retreat
- [ ] Add other outreach programs (your notes mention outreach for underrepresented communities, but the CV only lists these)

**Off the Bench**
- [ ] Is "Off the Bench" the title you want? (change in `_config.yml` nav and the page title in `off-the-bench.md`)
- [ ] Add your first photo and first song to see the layout with real content

**Footer / all pages**
- [ ] Email is saksham.gupta.y19@gmail.com: keep, or switch to a UW / HHMI address
- [ ] Add Google Scholar and ORCID links in `_config.yml` if you have them

## C. Things I noticed that still need fixing
- [ ] **Privacy:** both CV PDFs include your phone number. A public CV on the site should drop the phone number (and maybe the city)
- [ ] **Old files still public:** `assets/self_pic.jpg` (4 MB, camera metadata inside) and the old `assets/GuptaSaksham_CV_GS.pdf` are in the repo; delete or replace them once the new files are in
- [ ] **CV content** (your list of changes pending). From my read of it: stray "ˇ" before the Cancer GeVo talk; no PMID on the paper; skills list has no prime editing, FACS or NGS pipeline / HPC work; "Developmental Biology" in research interests vs. genome editing and RNA biology on the site; GS Retreat and Sunday Science entries have no detail
- [ ] **Not tested with real Jekyll:** I couldn't install it, so the first GitHub build is the real test (my browser preview used a stand-in renderer)
- [ ] **Fonts:** Avenir only shows on Apple devices; Windows and Android get Nunito Sans (similar)
- [ ] Phone nav wraps to two lines; fine, but shorten "Off the Bench" if it bothers you
- [ ] `assets/files` is a stray 1-byte file from the old site; safe to delete

## D. Nice to have later
- [ ] A short Projects / tools page (pipelines, protocols on GitHub)
- [ ] Custom domain
- [ ] Weekly routine: paper summary, photo, song (templates in `_templates/`)
