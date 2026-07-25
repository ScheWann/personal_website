---
layout: page
permalink: /publications/
title: Publications
# description: publications in reversed chronological order.
nav: true
nav_order: 1
---

<!-- _pages/publications.md -->

<style>
  /* The year heading was a full-width right-aligned block, so it ate a whole
     row and pushed the first paper of its group down. It stays in the flow
     here -- that keeps the separating rule spanning the full width -- but a
     negative bottom margin equal to its own line box pulls the list back up,
     so the year and the group's first paper share a top edge.

     `line-height: 1` makes the heading exactly 1em tall, which is what makes
     `margin-bottom: -1em` cancel it precisely. */
  .publications h2.bibliography {
    line-height: 1;
    margin-top: 2rem;
    margin-bottom: -1em;
    padding-top: 1.25rem;
  }

  .publications ol.bibliography {
    margin-top: 0;
    margin-bottom: 0;
  }

  /* First group starts the page: no rule and no gap above it. */
  .publications h2.bibliography:first-child {
    margin-top: 0;
    padding-top: 0;
    border-top: 0;
  }
</style>

<div class="publications">

{% bibliography %}

</div>
