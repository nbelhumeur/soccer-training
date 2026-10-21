# Soccer Training – Youth Coach Practice Planner

A simple static practice builder for youth soccer coaches (U8 and U10).
Build a 60–90 minute session focused on **fundamentals and lots of touches**
from a visual activity library, with a live timeline and skill-focus summary.

## Use it

Open `index.html` in a browser. No build step and no dependencies.

1. Browse the **training library**; search by activity or skill, filter by session phase, or select skill chips. Multiple skill filters match activities covering all selected skills.
2. **Add** trainings to your practice. Adjust each one's minutes and reorder with the arrows.
3. Watch the plan panel update live:
   - **Total time** against the 60–90 minute target range
   - **Timeline** of the practice, colored by each training's primary skill
   - **Core focus** tags for the top skills; expand **Skill breakdown** for all coverage bars (primary skill counts full time, secondary skills count half)
4. **Copy link** to share the exact plan (stored in the URL), or **Print** a field-ready plan with diagrams and coaching points. The plan is also saved in your browser.

Trainings work for both U8 and U10; use the suggested progressions to make them harder.

## Adding trainings

Trainings live in the `LIB` object in `index.html`. Each has a default duration, ordered skills (first is primary), setup, steps, coaching points, and a small diagram spec.

## Publishing on GitHub Pages

This site needs no build step. Publish directly from the repository:

1. Commit and push `index.html`, `styles.css`, `.nojekyll`, and this README to `main`.
2. Open [Settings → Pages](https://github.com/nbelhumeur/soccer-training/settings/pages).
3. Set **Source** to **Deploy from a branch**, select **main** and **/ (root)**, then **Save**.
4. Wait for the **pages build and deployment** run to complete in the Actions tab.

The expected address is <https://nbelhumeur.github.io/soccer-training/>.
Once Pages is enabled, future pushes to `main` automatically update the site.
The `.nojekyll` file tells Pages to serve the static files without Jekyll processing.
Pages sites are public by default, even when the source repository is private.

## Notes

- Touch counts are rough estimates for planning, not measurements.
- Totals count active training only; allow additional time for water, setup, and transitions.
- The session structure reflects commonly used youth guidance (Play-Practice-Play,
  small-sided games, U8 4v4 / U10 7v7); it has not been checked against specific
  federation documents yet. Verify against your club or state association.

## Roadmap

- More activities, and a way to swap activities in a plan
- Season themes (dribbling, passing, 1v1 defending, shooting)
