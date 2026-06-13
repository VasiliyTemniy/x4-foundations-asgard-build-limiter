# Asgard Build Limiter

*The art of ATF shipbuilding is fading. Replacement Asgards take time — or never
come.*

This mod puts a configurable construction delay on Terran AI Asgard building.
When the Protectorate takes up an Asgard order, the work takes time — and you
will hear about it: a logbook rumour reports that Terran engineers are trying
to revive an ancient ATF battleship design. Set the delay high enough, and the
lost art stays lost.

## Why

In vanilla, losing an Asgard costs the Terran Protectorate about one minute of
paperwork: the job system orders a replacement the moment the wreck cools, for
less metallic microlattice than a Syn. For a ship lore says nobody remembers how
to build — and that no other faction can answer — that is neither balanced nor
believable.

## Game version compatibility

- 9.00 release - **supported**
- 9.00 betas and release candidates - **supported**
- 8.00 release - **supported**

## Dependencies

- **Cradle of Humanity DLC** — the mod limits Terran Asgard production; without
  the DLC there is nothing to limit.
- **SirNukes Mod Support APIs** ([link](https://www.nexusmods.com/x4foundations/mods/503)) —
  provides the Extension Options menu used for configuration.

Both are hard dependencies. The mod will not load without them.

## What it does

- Intercepts the Terran job system's Asgard build orders and holds them until
  the configured cooldown since the last Asgard build has elapsed.
- Touches nothing else: escorts, Syns, destroyers and the rest of the Terran
  war machine build normally. Fleets simply wait for their flagship.
- Your own shipyards are unaffected — this limits the AI faction only.

The held build occupies no shipyard slot, no resources and no build queue; the
job just retries later, exactly as it would if a shipyard were unavailable.

## Configuration

Extension Options -> Asgard Build Limiter:

| Setting | Default | Meaning |
| --- | --- | --- |
| Enabled | on | Turn the limiter off to restore vanilla behaviour. |
| Cooldown | 120 min | In-game minutes between AI Asgard builds. |

Guide: 60-120 minutes makes Asgards a rare, punishing loss instead of a
disposable asset. Crank the slider to maximum and the Terrans will effectively
never field a new one — the art is lost for good.

## Compatibility

- Patches two spots in vanilla `md/job_helper.xml`; no other vanilla files
  touched. Safe to add to or remove from an existing save.

Pairs well with an Asgard main battery rebalance like
**Asgard Spinal Lance Re-Balanced**
([link](https://www.nexusmods.com/x4foundations/mods/869)), if you believe a
single ship out-gunning the rest of the galaxy fifty-fold was a typo.

## Credits

- Built on **SirNukes Mod Support APIs**.
- By VasiliyTemniy.

## Source

https://github.com/VasiliyTemniy/x4-foundations-asgard-build-limiter
