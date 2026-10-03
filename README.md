<div align="center">

<h1>Yakyak</h1>

<h3>Sandbox for testing game balance changes</h3>

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![WebGL](https://img.shields.io/badge/WebGL-990000?style=for-the-badge&logo=webgl&logoColor=white)](https://www.khronos.org/webgl/)
[![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)](https://sqlite.org)

<hr>

<h2>About</h2>

<p>Yakyak is a place to try balance changes without touching a real game.<br>
Import a set of stats and formulas, tweak them, run a bunch of simulated matches,<br>
and see what actually changes. Useful when you want to know<br>
whether a damage tweak breaks something before committing to it.</p>

<p>It ships with templates for common genres, but the underlying model is generic<br>
enough that you can set up your own systems from scratch.</p>

<hr>

<h2>Mechanics</h2>

<table align="center">
<tr>
<td align="center" width="33%">

<h3>Combat</h3>

Damage<br>
Cooldowns<br>
Crit / dodge

</td>
<td align="center" width="33%">

<h3>Resources</h3>

Mana / energy<br>
Generation<br>
Cost curves

</td>
<td align="center" width="33%">

<h3>Progression</h3>

Level scaling<br>
Skill trees<br>
Item stats

</td>
</tr>
</table>

<hr>

<h2>Templates</h2>

<table align="center">
<tr>
<td align="center" width="33%">

<h3>MOBA</h3>

Heroes, abilities, items<br>
Map objectives

</td>
<td align="center" width="33%">

<h3>Card Games</h3>

Deck building<br>
Mana curves

</td>
<td align="center" width="33%">

<h3>RTS</h3>

Unit stats<br>
Build orders

</td>
</tr>
<tr>
<td align="center" width="33%">

<h3>RPG</h3>

Character stats<br>
Loot tables

</td>
<td align="center" width="33%">

<h3>Fighting</h3>

Frame data<br>
Damage scaling

</td>
<td align="center" width="33%">

<h3>Battle Royale</h3>

Weapon stats<br>
Zone damage

</td>
</tr>
</table>

<hr>

<h2>Pipeline</h2>

<p><code>Import → Modify → Simulate → Analyze → Export</code></p>

<p>Data comes in as JSON, you edit it by hand or through the UI,<br>
the engine runs Monte Carlo simulations over many matches,<br>
and the results come out as charts and a summary report.<br>
Win rates, matchup breakdowns, and outlier cases are all surfaced<br>
so you can see what changed and by how much.</p>

<hr>

<h2>Stack</h2>

```javascript
const stack = {
  frontend: ["React", "WebGL", "D3.js"],
  backend: ["Python", "FastAPI", "NumPy"],
  database: ["SQLite", "Redis"],
  analysis: ["Pandas", "SciPy", "Monte Carlo"]
};
```

<hr>

<h2>Setup</h2>

```bash
git clone https://github.com/gimzdev/yakyak.git
cd yakyak

npm install
pip install -r requirements.txt

cp .env.example .env
npm run dev
python backend/server.py
```

<hr>

<h2>Requirements</h2>

[![Node.js](https://img.shields.io/badge/Node.js_18+-339933?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org)
[![Python](https://img.shields.io/badge/Python_3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![RAM](https://img.shields.io/badge/RAM_4GB+-FF6B6B?style=for-the-badge&logo=memory&logoColor=white)](#requirements)

<hr>

[![Docs](https://img.shields.io/badge/Docs-3776AB?style=for-the-badge&logo=gitbook&logoColor=white)](https://docs.yakyak.dev)

</div>
