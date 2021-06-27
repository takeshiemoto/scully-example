---
title: 'My initial post'
description: '初めての投稿です'
published: true
slug: my-initial-post
---

# Scully でブログを作成する手順

## 新しい記事を投稿する手順

### Markdown を生成する

```bash
ng generate @scullyio/init:post --name="Angular tutorial"
```

- angular-tutorial.md が生成される

```markdown
---
title: 'Angular tutorial'
description: 'blog description'
published: false
slugs:
  - ___UNPUBLISHED___kao8mvda_pmldPr7aN7owPpStZiuDXFZ1ILfpcv5Z
---
```

- `published: false`の場合は匿名モードランダムな URL になる
- ブログ公開前のプレビューなどに利用する

### 作成した記事を確認する

```bash
npm run scully
npm run scully:serve
```

## 記事を公開する

- `published: true`に変更し、`slug`を削除する

```bash
npm run scully
npm run scully:serve
```

`http://localhost:1668/blog/angular-tutorial`

> publish: true で slug を設定すると任意の URL に変更できます
