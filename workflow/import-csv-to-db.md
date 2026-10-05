# How to Import CSV File Data to PostgreSQL

## Case Study: male_players.csv

Suppose that your data is inside `~/data/fifa-23-complete-player/male_players.csv` and PostgreSQL is successfully installed. Enter this directory first and then enter the interative terminal of PostgreSQL:

```

cd ~/data/fifa-23-complete-player/ # or any directory including your male_players.csv

# enter the interactive terminal of PostgreSQL
psql -U your_user -d your_databases

```

Then create a table "male_players" and specify its schema:

```sql

CREATE TABLE male_players (
    player_id BIGINT,
    player_url TEXT,
    fifa_version INTEGER,
    fifa_update INTEGER,
    fifa_update_date DATE,
    short_name TEXT,
    long_name TEXT,
    player_positions TEXT,
    overall INTEGER,
    potential INTEGER,
    value_eur BIGINT,
    wage_eur BIGINT,
    age INTEGER,
    dob DATE,
    height_cm INTEGER,
    weight_kg INTEGER,
    league_id BIGINT,
    league_name TEXT,
    league_level INTEGER,
    club_team_id BIGINT,
    club_name TEXT,
    club_position TEXT,
    club_jersey_number INTEGER,
    club_loaned_from TEXT,
    club_joined_date DATE,
    club_contract_valid_until_year INTEGER,
    nationality_id BIGINT,
    nationality_name TEXT,
    nation_team_id BIGINT,
    nation_position TEXT,
    nation_jersey_number INTEGER,
    preferred_foot TEXT,
    weak_foot INTEGER,
    skill_moves INTEGER,
    international_reputation INTEGER,
    work_rate TEXT,
    body_type TEXT,
    real_face BOOLEAN,
    release_clause_eur BIGINT,
    player_tags TEXT,
    player_traits TEXT,
    pace INTEGER,
    shooting INTEGER,
    passing INTEGER,
    dribbling INTEGER,
    defending INTEGER,
    physic INTEGER,
    attacking_crossing INTEGER,
    attacking_finishing INTEGER,
    attacking_heading_accuracy INTEGER,
    attacking_short_passing INTEGER,
    attacking_volleys INTEGER,
    skill_dribbling INTEGER,
    skill_curve INTEGER,
    skill_fk_accuracy INTEGER,
    skill_long_passing INTEGER,
    skill_ball_control INTEGER,
    movement_acceleration INTEGER,
    movement_sprint_speed INTEGER,
    movement_agility INTEGER,
    movement_reactions INTEGER,
    movement_balance INTEGER,
    power_shot_power INTEGER,
    power_jumping INTEGER,
    power_stamina INTEGER,
    power_strength INTEGER,
    power_long_shots INTEGER,
    mentality_aggression INTEGER,
    mentality_interceptions INTEGER,
    mentality_positioning INTEGER,
    mentality_vision INTEGER,
    mentality_penalties INTEGER,
    mentality_composure INTEGER,
    defending_marking_awareness INTEGER,
    defending_standing_tackle INTEGER,
    defending_sliding_tackle INTEGER,
    goalkeeping_diving INTEGER,
    goalkeeping_handling INTEGER,
    goalkeeping_kicking INTEGER,
    goalkeeping_positioning INTEGER,
    goalkeeping_reflexes INTEGER,
    goalkeeping_speed INTEGER,

    ls TEXT,
    st TEXT,
    rs TEXT,
    lw TEXT,
    lf TEXT,
    cf TEXT,
    rf TEXT,
    rw TEXT,
    lam TEXT,
    cam TEXT,
    ram TEXT,
    lm TEXT,
    lcm TEXT,
    cm TEXT,
    rcm TEXT,
    rm TEXT,
    lwb TEXT,
    ldm TEXT,
    cdm TEXT,
    rdm TEXT,
    rwb TEXT,
    lb TEXT,
    lcb TEXT,
    cb TEXT,
    rcb TEXT,
    rb TEXT,
    gk TEXT,

    player_face_url TEXT
);

```

Now you can import your male_players.csv file in the same terminal:

```sql

\copy male_players
FROM './male_players.csv'
-- or you can use absolute path, 
-- i.e. FROM '/home/your-username/data/fifa-23-complete-player/male_players.csv'
WITH (
    FORMAT CSV,
    HEADER TRUE,
    NULL ''
);

```