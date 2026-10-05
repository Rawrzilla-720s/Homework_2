# Homework 2 — My Movie Review (TMNT 2007)

CSC 4370 Web Programming · Suryaprakash Murugavvel · Section 002

A recreation of a Rotten Tomatoes style review page using HTML5 and an external
stylesheet. No tables, no inline styles, no presentational markup.

**Live:** https://codd.cs.gsu.edu/~smurugavvel1/web/hw2/index.html

## Layout Lab

| System | Where | Why |
| --- | --- | --- |
| CSS Grid | `#content` — `grid-template-columns: 1fr 250px` | The main column and sidebar are a two-dimensional page region relationship, and the counter bar spans both tracks with `grid-column: 1 / -1`. |
| Flexbox | `#reviews`, `.quote`, `.critic`, `#validators` | One-dimensional alignment of a repeated component. Handles the icon-beside-text rows and column wrapping with no spacer elements. |
| Media queries | 700px and 480px | Grid collapses to a single column; type and the score scale down; validator links unpin so they never cover content on a phone. |

## Measured results

At a 480px viewport:

| Element | Computed width |
| --- | --- |
| `#content` | 452px |
| `#main` | 452px |
| `#overview` | 432px |

No horizontal scrolling at 700px or 480px.

## Validation

Both files pass the W3C validators with zero errors.

## Files

```
index.html     page markup
styles.css     all styling
images/        the nine supplied assets
```
