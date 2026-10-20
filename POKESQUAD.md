# PokeSquad Battler's Showdown site

A fork of [Pokémon Showdown's client](https://github.com/smogon/pokemon-showdown-client) (AGPL-3.0, so this fork is public
and open source too; based on its commit `ab4b77b`) for **PokeSquad Battler**
([Mikale4/PokeSquadBattler](https://github.com/Mikale4/PokeSquadBattler)). It connects to PokeSquad's Showdown server
([Mikale4/PokeSquad-Showdown](https://github.com/Mikale4/PokeSquad-Showdown)), whose **[Gen 9] PokeSquad** format plays the
game's own battles.

- `play.pokemonshowdown.com/pokesquad.html`: the home page. Its settings point at PokeSquad's server
  (`pokesquad-showdown.onrender.com`; `?~~host:port` tries another) and say it has no login server (`noguestsecurity`).
- No login server: **Choose name** sends the name straight to the server (`client-main.ts`), and on connecting the name you
  chose last time comes back by itself (`panel-mainmenu.tsx`).
- `.github/workflows/pokesquad-pages.yml`: builds the client and publishes it on GitHub Pages.

Sprites, sounds and the Pokédex data still load from Pokémon Showdown's own site.
