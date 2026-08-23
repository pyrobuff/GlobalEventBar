# GlobalEventBar

Server-wide cooperative events for Paper, Purpur, Spigot, and Bukkit.

Every player contributes to one shared goal. Progress is shown on a BossBar, scores are stored by UUID, and ranking / participation / completion rewards are paid when the event finishes.

**Developer:** [pyroBuff](https://github.com/pyrobuff)  
**Version:** 1.1.0  
**Requires:** Minecraft 1.21.x / 26.1.x / 26.2, Java 21  
**License:** Proprietary — official JAR is free to use; source code is not published

> This public repository contains documentation and releases only. The plugin source is private.

## Download

Get the official JAR from [Releases](https://github.com/pyrobuff/GlobalEventBar/releases).

Put `GlobalEventBar-1.1.0.jar` in `plugins/`, then **stop and start** the server. Do not use `/reload`.

## Features

- Six gameplay types: mining, mob kills, fishing, farming, woodcutting, block placing
- Custom events count every playable type with existing point values
- Shared server target with a live BossBar
- Player contributions, ranks, and leaderboard GUIs
- Ranking, participation, and completion rewards
- SQLite storage (survives restart)
- Optional schedule and minimum-player requirement
- English and Turkish language files
- Optional Vault, PlaceholderAPI, and ItemsAdder

## Commands

| Command | Description |
| --- | --- |
| `/event` | Player GUI, stats, leaderboard, and rewards |
| `/eventbar start <type>` | Start an event |
| `/eventbar admin` | Admin GUI |
| `/eventbar cancel` | Cancel without paying rewards |
| `/eventbar complete` | Force-complete and pay rewards |
| `/eventbar reload` | Reload configuration |

Aliases: `/globalevent`, `/geb`

## PlaceholderAPI

Identifier: `globalevent`

- `%globalevent_event%`
- `%globalevent_current%`
- `%globalevent_target%`
- `%globalevent_percentage%`
- `%globalevent_player_contribution%`
- `%globalevent_player_rank%`

## Configuration

After first start, edit files in `plugins/GlobalEventBar/`:

- `config.yml` — language, BossBar, schedule, worlds
- `events.yml` — event types, targets, point tables
- `rewards.yml` — ranking, participation, and completion rewards
- `lang/` and `menus/` — English and Turkish text

## Support

Open an [issue](https://github.com/pyrobuff/GlobalEventBar/issues) on this repository.  
In-game: `/eventbar developer`

---

Sunucu geneli kooperatif etkinlikler, ortak BossBar, UUID sıralaması ve yapılandırılabilir ödüller. Paper, Purpur, Spigot ve Bukkit. Kaynak kod yayınlanmaz; resmi JAR ücretsizdir.
