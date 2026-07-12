# Data Dictionary

## Analysis Table: `All Data`

| Field | Description |
|---|---|
| Match ID | Unique identifier for each match |
| Date | Match date |
| Season | Football season, such as 2024/2025 |
| Time | Match kickoff time |
| Comp | Competition name |
| Round | Competition round or league matchweek |
| Venue | Home, Away, or Neutral |
| Result | Win, Draw, or Lose |
| GF | Goals scored by FC Barcelona |
| GA | Goals conceded by FC Barcelona |
| Opponent | Opposing team |
| Poss | FC Barcelona possession percentage |
| Attendance | Recorded match attendance |
| Captain | FC Barcelona captain for the match |
| Formation | FC Barcelona starting formation |
| Opp Formation | Opponent starting formation |

## Fact Table: `Fact_Matches`

| Field Group | Fields |
|---|---|
| Identifiers | Match ID, Date_key, Season_key, Comp_key, Venue_key, Opponent_key, Captain_key, Formation_key |
| Descriptive attributes | Round, Result, Opp Formation |
| Measures | GF, GA, Poss, Attendance |

## Dimension Tables

| Table | Key | Main Attribute |
|---|---|---|
| Dim_Date | Date_key | Date, time, month name, quarter |
| Dim_Season | Season_key | Season |
| Dim_Comp | Comp_key | Competition |
| Dim_Venue | Venue_key | Venue |
| Dim_Opponent | Opponent_key | Opponent |
| Dim_Captain | Captain_key | Captain |
| Dim_Formation | Formation_key | Formation |
