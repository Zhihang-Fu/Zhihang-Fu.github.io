# Zhihang Fu's Homepage

Personal academic homepage of **Zhihang Fu (付志航)** — Advanced Algorithm Expert at Token Foundry, Alibaba Group. Post-training Qwen for real-world impact.

**🌐 Live site: [zhihang-fu.github.io](https://zhihang-fu.github.io)**

## About This Site

- 🔆 **Research** — LLM post-training: Planning & Tool-Use, reasoning scaffolding, hallucination reduction
- 📚 **Publications** — ICLR / NeurIPS / ICML / ACL and more ([Google Scholar](https://scholar.google.com/citations?user=e_e3Ur0AAAAJ&hl=en))
- 🎖️ **Hiring** — Interns and full-time researchers in LLM research & applications ([details](https://zhihang-fu.github.io/internship/))

## Local Development

Both setups below use **China mirrors by default** (Aliyun apt & RubyGems) for fast, reliable builds in mainland China.

### Option A: Docker (recommended)

The repo ships two Dockerfiles:

- `Dockerfile.local` — **use this one locally**: Aliyun apt source + Aliyun RubyGems mirror
- `Dockerfile` — upstream version with official sources (slow in CN)

```bash
# Build once (a few minutes for the first build)
docker build -f Dockerfile.local -t zhihang-homepage .

# Serve with live reload
docker run --rm -v $(pwd):/usr/src/app -p 4000:4000 zhihang-homepage
```

Visit <http://localhost:4000>. Editing any file triggers an automatic rebuild — except `_config.yml`, which requires restarting the container.

### Option B: Native Ruby

```bash
# 1. (Optional, faster in CN) Switch apt to the Aliyun mirror — Ubuntu 22.04:
sudo sed -i.bak 's|archive.ubuntu.com|mirrors.aliyun.com|g; s|security.ubuntu.com|mirrors.aliyun.com|g' /etc/apt/sources.list
#    On Ubuntu 24.04, edit /etc/apt/sources.list.d/ubuntu.sources instead.

# 2. Install Ruby and build tools
sudo apt update && sudo apt install -y ruby-full build-essential nodejs zlib1g-dev

# 3. Switch RubyGems to the Aliyun mirror
gem sources --remove https://rubygems.org/ --add https://mirrors.aliyun.com/rubygems/
gem install bundler
bundle config mirror.https://rubygems.org https://mirrors.aliyun.com/rubygems/

# 4. Install dependencies and serve
bundle install
bundle exec jekyll serve -l -H localhost
```

If `bundle install` complains about the Ruby version, install a newer Ruby via [rbenv](https://github.com/rbenv/rbenv) or [RVM](https://rvm.io) and retry.

## Project Structure

| Path | What lives there |
| --- | --- |
| `_pages/about.md` | Homepage content (Hero, News, Services) |
| `_pages/publications.html` | Publications page |
| `_publications/` | One markdown file per paper |
| `_pages/Internship.html` | Hiring / internship page |
| `_sass/` | Theme styles (SCSS); design tokens in `_variables.scss` |
| `_includes/` | Reusable components (sidebar, masthead, footer…) |
| `_data/navigation.yml` | Top navigation links |
| `_config.yml` | Site-wide settings & author profile |
| `images/` | Avatar, paper teasers, favicons |

Note: `assets/css/main.css` is a build artifact of `assets/css/main.scss` — it is git-ignored on purpose. Never commit it; Jekyll regenerates it on every build.

## Credits

Built with [Jekyll](https://jekyllrb.com), based on [Academic Pages](https://github.com/academicpages/academicpages.github.io) (forked from the [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) theme, © Michael Rose, MIT License). See [LICENSE](LICENSE).
