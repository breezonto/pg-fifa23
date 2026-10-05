# Schema from Male Players CSV Raw Data

This document describes the schema of the PostgreSQL table `public.male_players` (imported from male_players.csv).

| # | Column | Type | Nullable | Example | Comment | Group |
|---:|---|---|---|---|---| --- |
| 1 | `player_id` | `bigint` | Yes |  | Unique identifier of the player. | Player Identity & Metadata | 
| 2 | `player_url` | `text` | Yes |  | URL associated with the player record. | Player Identity & Metadata | 
| 3 | `fifa_version` | `integer` | Yes |  | FIFA game/version associated with the player data. | FIFA Dataset / Version | 
| 4 | `fifa_update` | `integer` | Yes |  | FIFA data update identifier. | FIFA Dataset / Version | 
| 5 | `fifa_update_date` | `date` | Yes |  | Date on which the FIFA data update was released or recorded. | FIFA Dataset / Version | 
| 6 | `short_name` | `text` | Yes |  | Short/display name of the player. |  Player Identity & Metadata | 
| 7 | `long_name` | `text` | Yes |  | Full name of the player. | Player Identity & Metadata | 
| 8 | `player_positions` | `text` | Yes |  | Playing position or positions assigned to the player. | Position | 
| 9 | `overall` | `integer` | Yes |  | Overall player rating. | Overall Ratings | 
| 10 | `potential` | `integer` | Yes |  | Potential player rating. | Overall Ratings | 
| 11 | `value_eur` | `bigint` | Yes |  | Estimated player market value in euros. | Market & Contract | 
| 12 | `wage_eur` | `bigint` | Yes |  | Player wage value in euros. | Market & Contract | 
| 13 | `age` | `integer` | Yes |  | Age of the player. | Personal Information | 
| 14 | `dob` | `date` | Yes |  | Date of birth of the player. | Personal Information | 
| 15 | `height_cm` | `integer` | Yes |  | Player height in centimetres. | Personal Information | 
| 16 | `weight_kg` | `integer` | Yes |  | Player weight in kilograms. | Personal Information | 
| 17 | `league_id` | `bigint` | Yes |  | Identifier of the player's league. | League & Club | 
| 18 | `league_name` | `text` | Yes |  | Name of the player's league. | League & Club | 
| 19 | `league_level` | `integer` | Yes |  | Competitive level of the player's league. | League & Club | 
| 20 | `club_team_id` | `bigint` | Yes |  | Identifier of the player's club team. | League & Club | 
| 21 | `club_name` | `text` | Yes |  | Name of the player's club. | League & Club | 
| 22 | `club_position` | `text` | Yes |  | Position assigned to the player at the club. | Position | 
| 23 | `club_jersey_number` | `integer` | Yes |  | Jersey number assigned to the player at the club. | League & Club | 
| 24 | `club_loaned_from` | `text` | Yes |  | Club from which the player is loaned, if applicable. | League & Club | 
| 25 | `club_joined_date` | `date` | Yes |  | Date on which the player joined the club. | League & Club | 
| 26 | `club_contract_valid_until_year` | `integer` | Yes |  | Year until which the player's club contract is valid. | Market & Contract | 
| 27 | `nationality_id` | `bigint` | Yes |  | Identifier of the player's nationality. | Nationality & National Team | 
| 28 | `nationality_name` | `text` | Yes |  | Name of the player's nationality. | Nationality & National Team | 
| 29 | `nation_team_id` | `bigint` | Yes |  | Identifier of the player's national team. | Nationality & National Team | 
| 30 | `nation_position` | `text` | Yes |  | Position assigned to the player in the national team. | Position | 
| 31 | `nation_jersey_number` | `integer` | Yes |  | Jersey number assigned to the player in the national team. | Nationality & National Team  | 
| 32 | `preferred_foot` | `text` | Yes |  | Player's preferred foot. | Personal Information | 
| 33 | `weak_foot` | `integer` | Yes |  | Rating of the player's ability with the weaker foot. | General Skills | 
| 34 | `skill_moves` | `integer` | Yes |  | Rating of the player's skill-move ability. | Technical Skills | 
| 35 | `international_reputation` | `integer` | Yes |  | Rating representing the player's international reputation. | Overall Ratings | 
| 36 | `work_rate` | `text` | Yes |  | Player's work-rate classification. | Player Characteristics | 
| 37 | `body_type` | `text` | Yes |  | Player body-type classification. | Personal Information | 
| 38 | `real_face` | `boolean` | Yes |  | Indicates whether the player has a real-face representation. | Player Identity & Metadata | 
| 39 | `release_clause_eur` | `bigint` | Yes |  | Player release-clause value in euros. | Market & Contract | 
| 40 | `player_tags` | `text` | Yes |  | Tags associated with the player. | Player Characteristics | 
| 41 | `player_traits` | `text` | Yes |  | Traits associated with the player. | Player Characteristics | 
| 42 | `pace` | `integer` | Yes |  | Overall pace rating. | General Skills | 
| 43 | `shooting` | `integer` | Yes |  | Overall shooting rating. | General Skills | 
| 44 | `passing` | `integer` | Yes |  | Overall passing rating. | General Skills | 
| 45 | `dribbling` | `integer` | Yes |  | Overall dribbling rating. | General Skills | 
| 46 | `defending` | `integer` | Yes |  | Overall defending rating. | General Skills | 
| 47 | `physic` | `integer` | Yes |  | Overall physical rating. | General Skills | 
| 48 | `attacking_crossing` | `integer` | Yes |  | Rating for crossing ability. | Attacking Attributes | 
| 49 | `attacking_finishing` | `integer` | Yes |  | Rating for finishing ability. | Attacking Attributes | 
| 50 | `attacking_heading_accuracy` | `integer` | Yes |  | Rating for heading accuracy. | Attacking Attributes | 
| 51 | `attacking_short_passing` | `integer` | Yes |  | Rating for short passing. | Attacking Attributes | 
| 52 | `attacking_volleys` | `integer` | Yes |  | Rating for volley ability. | Attacking Attributes | 
| 53 | `skill_dribbling` | `integer` | Yes |  | Rating for dribbling skill. | Technical Skills | 
| 54 | `skill_curve` | `integer` | Yes |  | Rating for curve/shaped-ball ability. | Technical Skills | 
| 55 | `skill_fk_accuracy` | `integer` | Yes |  | Rating for free-kick accuracy. | Technical Skills | 
| 56 | `skill_long_passing` | `integer` | Yes |  | Rating for long passing. | Technical Skills | 
| 57 | `skill_ball_control` | `integer` | Yes |  | Rating for ball-control ability. | Technical Skills | 
| 58 | `movement_acceleration` | `integer` | Yes |  | Rating for acceleration. | Movement Attributes | 
| 59 | `movement_sprint_speed` | `integer` | Yes |  | Rating for sprint speed. | Movement Attributes | 
| 60 | `movement_agility` | `integer` | Yes |  | Rating for agility. | Movement Attributes | 
| 61 | `movement_reactions` | `integer` | Yes |  | Rating for reactions. | Movement Attributes | 
| 62 | `movement_balance` | `integer` | Yes |  | Rating for balance. | Movement Attributes | 
| 63 | `power_shot_power` | `integer` | Yes |  | Rating for shot power. | Power & Physical Attributes | 
| 64 | `power_jumping` | `integer` | Yes |  | Rating for jumping ability. | Power & Physical Attributes | 
| 65 | `power_stamina` | `integer` | Yes |  | Rating for stamina. | Power & Physical Attributes | 
| 66 | `power_strength` | `integer` | Yes |  | Rating for physical strength. | Power & Physical Attributes | 
| 67 | `power_long_shots` | `integer` | Yes |  | Rating for long-shot ability. | Power & Physical Attributes | 
| 68 | `mentality_aggression` | `integer` | Yes |  | Rating for aggression. | Mentality Attributes | 
| 69 | `mentality_interceptions` | `integer` | Yes |  | Rating for interception ability. | Mentality Attributes | 
| 70 | `mentality_positioning` | `integer` | Yes |  | Rating for positioning. | Mentality Attributes | 
| 71 | `mentality_vision` | `integer` | Yes |  | Rating for vision. | Mentality Attributes | 
| 72 | `mentality_penalties` | `integer` | Yes |  | Rating for penalty-taking ability. | Mentality Attributes | 
| 73 | `mentality_composure` | `integer` | Yes |  | Rating for composure. | Mentality Attributes | 
| 74 | `defending_marking_awareness` | `integer` | Yes |  | Rating for defensive marking awareness. | Defensive Attributes | 
| 75 | `defending_standing_tackle` | `integer` | Yes |  | Rating for standing-tackle ability. | Defensive Attributes | 
| 76 | `defending_sliding_tackle` | `integer` | Yes |  | Rating for sliding-tackle ability. | Defensive Attributes | 
| 77 | `goalkeeping_diving` | `integer` | Yes |  | Rating for goalkeeper diving. | Goalkeeping Attributes | 
| 78 | `goalkeeping_handling` | `integer` | Yes |  | Rating for goalkeeper handling. | Goalkeeping Attributes | 
| 79 | `goalkeeping_kicking` | `integer` | Yes |  | Rating for goalkeeper kicking. | Goalkeeping Attributes | 
| 80 | `goalkeeping_positioning` | `integer` | Yes |  | Rating for goalkeeper positioning. | Goalkeeping Attributes | 
| 81 | `goalkeeping_reflexes` | `integer` | Yes |  | Rating for goalkeeper reflexes. | Goalkeeping Attributes | 
| 82 | `goalkeeping_speed` | `integer` | Yes |  | Rating for goalkeeper speed. | Goalkeeping Attributes | 
| 83 | `ls` | `text` | Yes |  | Player rating for the left-striker position. | Position-Specific Ratings | 
| 84 | `st` | `text` | Yes |  | Player rating for the striker position. | Position-Specific Ratings | 
| 85 | `rs` | `text` | Yes |  | Player rating for the right-striker position. | Position-Specific Ratings | 
| 86 | `lw` | `text` | Yes |  | Player rating for the left-wing position. | Position-Specific Ratings | 
| 87 | `lf` | `text` | Yes |  | Player rating for the left-forward position. | Position-Specific Ratings | 
| 88 | `cf` | `text` | Yes |  | Player rating for the centre-forward position. | Position-Specific Ratings | 
| 89 | `rf` | `text` | Yes |  | Player rating for the right-forward position. | Position-Specific Ratings | 
| 90 | `rw` | `text` | Yes |  | Player rating for the right-wing position. | Position-Specific Ratings | 
| 91 | `lam` | `text` | Yes |  | Player rating for the left attacking-midfielder position. | Position-Specific Ratings | 
| 92 | `cam` | `text` | Yes |  | Player rating for the central attacking-midfielder position. | Position-Specific Ratings | 
| 93 | `ram` | `text` | Yes |  | Player rating for the right attacking-midfielder position. | Position-Specific Ratings | 
| 94 | `lm` | `text` | Yes |  | Player rating for the left-midfielder position. | Position-Specific Ratings | 
| 95 | `lcm` | `text` | Yes |  | Player rating for the left central-midfielder position. | Position-Specific Ratings | 
| 96 | `cm` | `text` | Yes |  | Player rating for the central-midfielder position. | Position-Specific Ratings | 
| 97 | `rcm` | `text` | Yes |  | Player rating for the right central-midfielder position. | Position-Specific Ratings | 
| 98 | `rm` | `text` | Yes |  | Player rating for the right-midfielder position. | Position-Specific Ratings | 
| 99 | `lwb` | `text` | Yes |  | Player rating for the left wing-back position. | Position-Specific Ratings | 
| 100 | `ldm` | `text` | Yes |  | Player rating for the left defensive-midfielder position. | Position-Specific Ratings | 
| 101 | `cdm` | `text` | Yes |  | Player rating for the central defensive-midfielder position. | Position-Specific Ratings | 
| 102 | `rdm` | `text` | Yes |  | Player rating for the right defensive-midfielder position. | Position-Specific Ratings | 
| 103 | `rwb` | `text` | Yes |  | Player rating for the right wing-back position. | Position-Specific Ratings | 
| 104 | `lb` | `text` | Yes |  | Player rating for the left-back position. | Position-Specific Ratings | 
| 105 | `lcb` | `text` | Yes |  | Player rating for the left centre-back position. | Position-Specific Ratings | 
| 106 | `cb` | `text` | Yes |  | Player rating for the centre-back position. | Position-Specific Ratings | 
| 107 | `rcb` | `text` | Yes |  | Player rating for the right centre-back position. | Position-Specific Ratings | 
| 108 | `rb` | `text` | Yes |  | Player rating for the right-back position. | Position-Specific Ratings | 
| 109 | `gk` | `text` | Yes |  | Player rating for the goalkeeper position. | Position-Specific Ratings | 
| 110 | `player_face_url` | `text` | Yes |  | URL of the player's face image. | Player Identity & Metadata | 

## Notes

- The schema is reproduced from the PostgreSQL `\d` table description provided.
- The `Comment` column provides a human-readable semantic description based on each attribute name; the original schema does not contain explicit column comments.
- The supplied schema output does not specify constraints, indexes, primary keys, foreign keys, or default values beyond the displayed empty/default fields.
- The displayed PostgreSQL output leaves the `Nullable` and `Default` columns empty for all fields; this document therefore does not infer additional constraints or defaults.
