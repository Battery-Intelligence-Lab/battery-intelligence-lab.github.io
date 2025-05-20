# Battery Intelligence Lab website

## Editing

Use [Markdown](https://daringfireball.net/projects/markdown/) to edit pages and post content.

### Pages

- Home: `index.md`
- Research: `research/index.html`
- People: `people.md`
- Publications: `publications.md`
- Data and code: `data-and-code.md`
- ~~Lab: `lab.md`~~ -> now removed (to deprecated folder)
- Contact: `contact.md`
- Research subpages: `research/{research-area}/index.html`
- Projects: `research/{research-area}/{project-name}.md`

### Posts

- `_posts/{YYYY-MM-DD-post-name}.md`

### Data

- Articles: `_data/articles.yml`
- Data and code:` _data/data-and-code.yml`
- ~~Equipment: `_data/equipment.yml`~~ -> no longer used
- People: `_data/people.yml`
- Sponsors: `_data/sponsors.yml`

### Images

- Article thumbnails:` img/articles/{image-name}.jpg` (ideal size 144px*144px)
- ~~Equipment: `img/equipment/{image-name}.jpg` (ideal size 720px*480px or 480px*720px)~~ -> not used any longer
- Page hero images: `img/hero/{page-name}.jpg` (ideal size 1140px*500px)
- Page hero images (retina): `img/hero/{page-name}@2x.jpg` (ideal size 2280px*1000px)
- People photos: `img/people/{first-name}-{surname}.jpg` (ideal size 720px*480px)
- Sponsor logos: `img/sponsors/{sponsor-name}.png` (ideal height: 96px)

## Building

The site will be auto-built (using [jekyll](https://jekyllrb.com/)) by github pages after each commit.
