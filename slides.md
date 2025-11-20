---
marp: true
title: Product Documentation
paginate: true
theme: custom
---
marp: true
theme: default
paginate: true
title: Product Documentation
author: 24f1000182@ds.study.iitm.ac.in
description: "Version-controlled product documentation slides (Marp)."
style: |
  /* Custom theme specification */
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&display=swap');

  section {
    font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    line-height: 1.35;
  }

  h1 {
    color: #0b57d0;
    font-weight: 800;
  }

  h2 { color: #0b57d0; }

  /* Footer / page number styling */
  footer.marppage {
    position: absolute;
    right: 1rem;
    bottom: 0.6rem;
    color: #666;
    font-size: 0.85rem;
  }

  /* Lightweight note style to demonstrate custom classes */
  .note {
    font-size: 0.9rem;
    color: #444;
    opacity: 0.95;
  }

---

<!-- _class: lead -->

# Product Documentation

**Author:** 24f1000182@ds.study.iitm.ac.in

Brief: Maintained in Git, exportable via Marp CLI to PDF/HTML/image formats.

---

# Introduction

This deck documents the product for engineers and stakeholders. It is:

- Version controllable (Markdown)
- Themeable (custom CSS)
- Renderable to PDF/HTML with Marp

---

<!--
backgroundImage: url('https://images.unsplash.com/photo-1504384308090-c894fdcc538d?auto=format&fit=crop&w=1600&q=80')
backgroundSize: cover
backgroundPosition: center
backgroundRepeat: no-repeat
-->

# Product Vision

<div class="note">A short description overlayed on a background image to demonstrate slide-level background directives.</div>

---

# Key Features

- API Enhancements
- Improved Performance (lower latency)
- Cross-platform Support

---

# Mathematical Equations

### Algorithmic Complexity Examples

Recurrence for merge sort:

$$
T(n) = 2T\left(\frac{n}{2}\right) + n
$$

By the Master Theorem:

$$
T(n) = O(n\log n)
$$

Binary search complexity (iterative): $O(\log n)$

---

# Code Snippet: Binary Search

```js
function binarySearch(arr, target) {
  let left = 0, right = arr.length - 1;

  while (left <= right) {
    const mid = Math.floor((left + right) / 2);
    if (arr[mid] === target) return mid;
    if (arr[mid] < target) left = mid + 1;
    else right = mid - 1;
  }
  return -1;
}
```

---

# Maintainability

- Keep slides in `slides.md` under the repo root
- Use branches and PRs to update docs
- Render locally with Marp CLI for proofs and PDFs

---

# Raw GitHub URL

You can retrieve the raw Markdown via:

`https://raw.githubusercontent.com/24f1000182/marp-presentation/main/slides.md`

---

# Thank You

Questions? Reach me at **24f1000182@ds.study.iitm.ac.in**

<!-- footer placeholder to show page numbers when Marp `paginate:true` is used -->
<!-- footer.marppage: -->
