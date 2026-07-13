---
permalink: /search/
title: "Search"
excerpt: "Search the CANlab documentation, walkthroughs, and tutorials."
author_profile: false
---
{% include base_path %}

<p>Search across the CANlab documentation, walkthroughs, and tutorials. Type at least two characters; results update as you type.</p>

<div class="search-page">
  <input type="text"
         id="search-input"
         placeholder="Search walkthroughs, tutorials, setup&hellip;"
         aria-label="Search this site"
         autofocus />
  <ul id="results-container"></ul>
</div>

<script src="{{ "/assets/js/simple-jekyll-search.min.js" | relative_url }}"></script>
<script>
  (function () {
    // Merge two full-text indexes: search.json (Jekyll pages, auto-generated)
    // and search-extra.json (published HTML walkthroughs, built by
    // markdown_generator/build_search_extra.py).
    var sources = [
      '{{ "/search.json" | relative_url }}',
      '{{ "/search-extra.json" | relative_url }}'
    ];

    Promise.all(sources.map(function (url) {
      return fetch(url).then(function (r) { return r.ok ? r.json() : []; }).catch(function () { return []; });
    })).then(function (parts) {
      var data = Array.prototype.concat.apply([], parts);

      SimpleJekyllSearch({
        searchInput: document.getElementById('search-input'),
        resultsContainer: document.getElementById('results-container'),
        json: data,
        searchResultTemplate: '<li><a href="{url}"><strong>{title}</strong></a><p>{excerpt}</p></li>',
        noResultsText: '<li class="search-no-results">No results found.</li>',
        limit: 25,
        fuzzy: false
      });

      // Pre-fill from ?q= so the nav search box can deep-link here.
      var params = new URLSearchParams(window.location.search);
      var q = params.get('q');
      if (q) {
        var input = document.getElementById('search-input');
        input.value = q;
        input.dispatchEvent(new Event('input'));
      }
    });
  })();
</script>

<style>
  .search-page #search-input {
    width: 100%;
    padding: 0.6em 0.8em;
    font-size: 1.1em;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;
    margin-bottom: 1.25em;
  }
  .search-page #results-container {
    list-style: none;
    padding: 0;
    margin: 0;
  }
  .search-page #results-container li {
    border-bottom: 1px solid #eee;
    padding: 0.75em 0;
  }
  .search-page #results-container li:last-child { border-bottom: none; }
  .search-page #results-container p {
    margin: 0.25em 0 0;
    color: #555;
    font-size: 0.95em;
  }
  .search-no-results { color: #888; font-style: italic; }
</style>
