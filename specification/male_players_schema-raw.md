# `public.male_players` Schema

This document describes the schema of the PostgreSQL table `public.male_players`.

| # | Column | Type | Nullable | Example | Comment |
|---:|---|---|---|---|---|
| 1 | `player_id` | `bigint` | Yes |  | Unique identifier of the player. |
| 2 | `player_url` | `text` | Yes |  | URL associated with the player record. |
| 3 | `fifa_version` | `integer` | Yes |  | FIFA game/version associated with the player data. |
| 4 | `fifa_update` | `integer` | Yes |  | FIFA data update identifier. |
| 5 | `fifa_update_date` | `date` | Yes |  | Date on which the FIFA data update was released or recorded. |
| 6 | `short_name` | `text` | Yes |  | Short/display name of the player. |
| 7 | `long_name` | `text` | Yes |  | Full name of the player. |
| 8 | `player_positions` | `text` | Yes |  | Playing position or positions assigned to the player. |
| 9 | `overall` | `integer` | Yes |  | Overall player rating. |
| 10 | `potential` | `integer` | Yes |  | Potential player rating. |
| 11 | `value_eur` | `bigint` | Yes |  | Estimated player market value in euros. |
| 12 | `wage_eur` | `bigint` | Yes |  | Player wage value in euros. |
| 13 | `age` | `integer` | Yes |  | Age of the player. |
| 14 | `dob` | `date` | Yes |  | Date of birth of the player. |
| 15 | `height_cm` | `integer` | Yes |  | Player height in centimetres. |
| 16 | `weight_kg` | `integer` | Yes |  | Player weight in kilograms. |
| 17 | `league_id` | `bigint` | Yes |  | Identifier of the player's league. |
| 18 | `league_name` | `text` | Yes |  | Name of the player's league. |
| 19 | `league_level` | `integer` | Yes |  | Competitive level of the player's league. |
| 20 | `club_team_id` | `bigint` | Yes |  | Identifier of the player's club team. |
| 21 | `club_name` | `text` | Yes |  | Name of the player's club. |
| 22 | `club_position` | `text` | Yes |  | Position assigned to the player at the club. |
| 23 | `club_jersey_number` | `integer` | Yes |  | Jersey number assigned to the player at the club. |
| 24 | `club_loaned_from` | `text` | Yes |  | Club from which the player is loaned, if applicable. |
| 25 | `club_joined_date` | `date` | Yes |  | Date on which the player joined the club. |
| 26 | `club_contract_valid_until_year` | `integer` | Yes |  | Year until which the player's club contract is valid. |
| 27 | `nationality_id` | `bigint` | Yes |  | Identifier of the player's nationality. |
| 28 | `nationality_name` | `text` | Yes |  | Name of the player's nationality. |
| 29 | `nation_team_id` | `bigint` | Yes |  | Identifier of the player's national team. |
| 30 | `nation_position` | `text` | Yes |  | Position assigned to the player in the national team. |
| 31 | `nation_jersey_number` | `integer` | Yes |  | Jersey number assigned to the player in the national team. |
| 32 | `preferred_foot` | `text` | Yes |  | Player's preferred foot. |
| 33 | `weak_foot` | `integer` | Yes |  | Rating of the player's ability with the weaker foot. |
| 34 | `skill_moves` | `integer` | Yes |  | Rating of the player's skill-move ability. |
| 35 | `international_reputation` | `integer` | Yes |  | Rating representing the player's international reputation. |
| 36 | `work_rate` | `text` | Yes |  | Player's work-rate classification. |
| 37 | `body_type` | `text` | Yes |  | Player body-type classification. |
| 38 | `real_face` | `boolean` | Yes |  | Indicates whether the player has a real-face representation. |
| 39 | `release_clause_eur` | `bigint` | Yes |  | Player release-clause value in euros. |
| 40 | `player_tags` | `text` | Yes |  | Tags associated with the player. |
| 41 | `player_traits` | `text` | Yes |  | Traits associated with the player. |
| 42 | `pace` | `integer` | Yes |  | Overall pace rating. |
| 43 | `shooting` | `integer` | Yes |  | Overall shooting rating. |
| 44 | `passing` | `integer` | Yes |  | Overall passing rating. |
| 45 | `dribbling` | `integer` | Yes |  | Overall dribbling rating. |
| 46 | `defending` | `integer` | Yes |  | Overall defending rating. |
| 47 | `physic` | `integer` | Yes |  | Overall physical rating. |
| 48 | `attacking_crossing` | `integer` | Yes |  | Rating for crossing ability. |
| 49 | `attacking_finishing` | `integer` | Yes |  | Rating for finishing ability. |
| 50 | `attacking_heading_accuracy` | `integer` | Yes |  | Rating for heading accuracy. |
| 51 | `attacking_short_passing` | `integer` | Yes |  | Rating for short passing. |
| 52 | `attacking_volleys` | `integer` | Yes |  | Rating for volley ability. |
| 53 | `skill_dribbling` | `integer` | Yes |  | Rating for dribbling skill. |
| 54 | `skill_curve` | `integer` | Yes |  | Rating for curve/shaped-ball ability. |
| 55 | `skill_fk_accuracy` | `integer` | Yes |  | Rating for free-kick accuracy. |
| 56 | `skill_long_passing` | `integer` | Yes |  | Rating for long passing. |
| 57 | `skill_ball_control` | `integer` | Yes |  | Rating for ball-control ability. |
| 58 | `movement_acceleration` | `integer` | Yes |  | Rating for acceleration. |
| 59 | `movement_sprint_speed` | `integer` | Yes |  | Rating for sprint speed. |
| 60 | `movement_agility` | `integer` | Yes |  | Rating for agility. |
| 61 | `movement_reactions` | `integer` | Yes |  | Rating for reactions. |
| 62 | `movement_balance` | `integer` | Yes |  | Rating for balance. |
| 63 | `power_shot_power` | `integer` | Yes |  | Rating for shot power. |
| 64 | `power_jumping` | `integer` | Yes |  | Rating for jumping ability. |
| 65 | `power_stamina` | `integer` | Yes |  | Rating for stamina. |
| 66 | `power_strength` | `integer` | Yes |  | Rating for physical strength. |
| 67 | `power_long_shots` | `integer` | Yes |  | Rating for long-shot ability. |
| 68 | `mentality_aggression` | `integer` | Yes |  | Rating for aggression. |
| 69 | `mentality_interceptions` | `integer` | Yes |  | Rating for interception ability. |
| 70 | `mentality_positioning` | `integer` | Yes |  | Rating for positioning. |
| 71 | `mentality_vision` | `integer` | Yes |  | Rating for vision. |
| 72 | `mentality_penalties` | `integer` | Yes |  | Rating for penalty-taking ability. |
| 73 | `mentality_composure` | `integer` | Yes |  | Rating for composure. |
| 74 | `defending_marking_awareness` | `integer` | Yes |  | Rating for defensive marking awareness. |
| 75 | `defending_standing_tackle` | `integer` | Yes |  | Rating for standing-tackle ability. |
| 76 | `defending_sliding_tackle` | `integer` | Yes |  | Rating for sliding-tackle ability. |
| 77 | `goalkeeping_diving` | `integer` | Yes |  | Rating for goalkeeper diving. |
| 78 | `goalkeeping_handling` | `integer` | Yes |  | Rating for goalkeeper handling. |
| 79 | `goalkeeping_kicking` | `integer` | Yes |  | Rating for goalkeeper kicking. |
| 80 | `goalkeeping_positioning` | `integer` | Yes |  | Rating for goalkeeper positioning. |
| 81 | `goalkeeping_reflexes` | `integer` | Yes |  | Rating for goalkeeper reflexes. |
| 82 | `goalkeeping_speed` | `integer` | Yes |  | Rating for goalkeeper speed. |
| 83 | `ls` | `text` | Yes |  | Player rating for the left-striker position. |
| 84 | `st` | `text` | Yes |  | Player rating for the striker position. |
| 85 | `rs` | `text` | Yes |  | Player rating for the right-striker position. |
| 86 | `lw` | `text` | Yes |  | Player rating for the left-wing position. |
| 87 | `lf` | `text` | Yes |  | Player rating for the left-forward position. |
| 88 | `cf` | `text` | Yes |  | Player rating for the centre-forward position. |
| 89 | `rf` | `text` | Yes |  | Player rating for the right-forward position. |
| 90 | `rw` | `text` | Yes |  | Player rating for the right-wing position. |
| 91 | `lam` | `text` | Yes |  | Player rating for the left attacking-midfielder position. |
| 92 | `cam` | `text` | Yes |  | Player rating for the central attacking-midfielder position. |
| 93 | `ram` | `text` | Yes |  | Player rating for the right attacking-midfielder position. |
| 94 | `lm` | `text` | Yes |  | Player rating for the left-midfielder position. |
| 95 | `lcm` | `text` | Yes |  | Player rating for the left central-midfielder position. |
| 96 | `cm` | `text` | Yes |  | Player rating for the central-midfielder position. |
| 97 | `rcm` | `text` | Yes |  | Player rating for the right central-midfielder position. |
| 98 | `rm` | `text` | Yes |  | Player rating for the right-midfielder position. |
| 99 | `lwb` | `text` | Yes |  | Player rating for the left wing-back position. |
| 100 | `ldm` | `text` | Yes |  | Player rating for the left defensive-midfielder position. |
| 101 | `cdm` | `text` | Yes |  | Player rating for the central defensive-midfielder position. |
| 102 | `rdm` | `text` | Yes |  | Player rating for the right defensive-midfielder position. |
| 103 | `rwb` | `text` | Yes |  | Player rating for the right wing-back position. |
| 104 | `lb` | `text` | Yes |  | Player rating for the left-back position. |
| 105 | `lcb` | `text` | Yes |  | Player rating for the left centre-back position. |
| 106 | `cb` | `text` | Yes |  | Player rating for the centre-back position. |
| 107 | `rcb` | `text` | Yes |  | Player rating for the right centre-back position. |
| 108 | `rb` | `text` | Yes |  | Player rating for the right-back position. |
| 109 | `gk` | `text` | Yes |  | Player rating for the goalkeeper position. |
| 110 | `player_face_url` | `text` | Yes |  | URL of the player's face image. |

## Notes

- The schema is reproduced from the PostgreSQL `\d` table description provided.
- The `Comment` column provides a human-readable semantic description based on each attribute name; the original schema does not contain explicit column comments.
- The supplied schema output does not specify constraints, indexes, primary keys, foreign keys, or default values beyond the displayed empty/default fields.
- The displayed PostgreSQL output leaves the `Nullable` and `Default` columns empty for all fields; this document therefore does not infer additional constraints or defaults.
