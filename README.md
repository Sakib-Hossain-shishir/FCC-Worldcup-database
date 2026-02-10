# World Cup Database (PostgreSQL)

A relational **World Cup database** built using **PostgreSQL** and **SQL**.  
This project stores match and team data and answers common football statistics questions through structured SQL queries.

The focus is on **correct database design**, **clean joins**, and **accurate querying** — not shortcuts.

---

## Database Schema

### `teams`
| Column | Type | Description |
|------|------|------------|
| team_id | SERIAL | Primary key |
| name | VARCHAR | Team name |

### `games`
| Column | Type | Description |
|------|------|------------|
| game_id | SERIAL | Primary key |
| year | INT | World Cup year |
| round | VARCHAR | Tournament round |
| winner_id | INT | Winning team (FK → teams.team_id) |
| opponent_id | INT | Opponent team (FK → teams.team_id) |
| winner_goals | INT | Goals scored by winner |
| opponent_goals | INT | Goals scored by opponent |

---
