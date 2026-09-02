# League Standings Site

Two files make this work:

- **index.html** — the whole site: layout, styling, scoring logic, and the
  code that fetches live NFL data from ESPN. This is what you'll edit if you
  want to change how it looks.
- **config.json** — just your league's data: 8 players and the 4 team
  abbreviations each one picked (e.g. `"BUF"`, `"KC"`, `"PHI"`). This is what
  you'll edit whenever picks change.

## Updating who owns which teams

1. Open the live site and click **Edit teams**.
2. Fill in names and pick teams from the dropdowns.
3. Click **Download config.json** — it'll save to your Downloads folder.
4. On GitHub, open `config.json` in your repo, click the pencil (edit) icon,
   delete the contents, and paste in the downloaded file's contents.
5. Commit the change. The live site updates automatically within a minute
   or two.

Team abbreviations to use in config.json: ARI, ATL, BAL, BUF, CAR, CHI, CIN,
CLE, DAL, DEN, DET, GB, HOU, IND, JAX, KC, LAC, LAR, LV, MIA, MIN, NE, NO,
NYG, NYJ, PHI, PIT, SEA, SF, TB, TEN, WSH.

## Changing the design

Everything visual lives in the `<style>` block at the top of `index.html`
(colors are CSS variables under `:root` near the top — start there for a
quick palette change). The scoring rules live in the `PTS` object partway
down the `<script>` block if you ever want to adjust point values.
