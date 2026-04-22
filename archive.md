---
layout: page
title: Archive
subtitle: Historical blog posts
permalink: /archive/
---

<style>
  .archive-wrap {
    --ink: #102038;
    --muted: #4f607a;
    --line: #d9e2ef;
    --panel: #ffffff;
    --hero-a: #f6fbff;
    --hero-b: #eaf5ff;
    --accent: #0d6b9a;
    color: var(--ink);
  }

  .archive-hero {
    margin: 8px 0 20px;
    padding: 22px;
    border: 1px solid var(--line);
    border-radius: 14px;
    background: linear-gradient(136deg, var(--hero-a) 0%, var(--hero-b) 100%);
    box-shadow: 0 12px 24px rgba(16, 34, 56, 0.07);
  }

  .archive-hero h1 {
    margin: 0 0 8px;
    font-size: 1.8rem;
  }

  .archive-hero p {
    margin: 0;
    color: #334967;
    line-height: 1.6;
  }

  .archive-list {
    display: grid;
    gap: 14px;
  }

  .archive-item {
    border: 1px solid #dde6f2;
    border-radius: 12px;
    background: var(--panel);
    padding: 15px;
    box-shadow: 0 10px 20px rgba(16, 34, 56, 0.05);
  }

  .archive-item h3 {
    margin: 0 0 6px;
    font-size: 1.1rem;
  }

  .archive-meta {
    display: inline-block;
    margin-bottom: 8px;
    padding: 4px 9px;
    border-radius: 999px;
    border: 1px solid #c8d9ea;
    color: var(--accent);
    background: #f5faff;
    font-size: 0.83rem;
    font-weight: 700;
  }

  .archive-item p {
    margin: 0;
    color: var(--muted);
    line-height: 1.58;
  }

  .archive-note {
    margin-top: 18px;
    border-left: 4px solid var(--accent);
    background: #f7fbff;
    padding: 12px 14px;
    color: #2f4768;
  }
</style>

<div class="archive-wrap">
  <section class="archive-hero">
    <h1>Archived Blog Posts</h1>
    <p>
      These older posts are currently unpublished from the live site to keep Intune.Ninja focused on the new landing-page and CommunityTools experience.
    </p>
  </section>

  <div class="archive-list">
    <article class="archive-item">
      <h3>Get-IntuneManagementExtensionDiagnostics released</h3>
      <span class="archive-meta">Published date: 2023-03-13 | Status: Archived (unpublished)</span>
      <p>
        Original release post for the Intune Management Extension diagnostics and timeline analysis tool.
      </p>
    </article>

    <article class="archive-item">
      <h3>Intune Linux Custom Compliance script updated</h3>
      <span class="archive-meta">Published date: 2023-03-15 | Status: Archived (unpublished)</span>
      <p>
        Update post covering Linux custom compliance checks and related implementation guidance.
      </p>
    </article>
  </div>

  <div class="archive-note">
    To republish any post later, edit the post file front matter and remove <strong>published: false</strong>.
  </div>
</div>
