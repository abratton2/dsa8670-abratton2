# Pseudocode: Which NFL Stats Drive Win Rate (Last 5 Years)

Descriptive steps for finding which offensive and defensive team statistics best relate to win rate over the last five NFL seasons.

## Step 1: Load the dataset

- Gather team-level season stats for the last five years (for example, points for/against, yards, turnovers, sacks, third-down rate).
- Include each team’s wins and losses (or win percentage) for each season.
- Import the table into the analysis environment.
- Confirm it loaded correctly by checking row count, column names, and a few sample rows (one row per team-season).

## Step 2: Clean the data

- Remove rows with missing win totals or key offensive/defensive metrics.
- Standardize team names so the same franchise is spelled the same way across seasons.
- Create a win-rate column if needed (wins ÷ games played).
- Check for obvious errors (win rates outside 0–1, negative yardage) and fix or drop those rows.
- Keep only the columns needed: season, team, win rate, and the offensive/defensive stats of interest.

## Step 3: Calculate summary statistics

- Compute the average and range of win rate across all team-seasons.
- For each offensive and defensive stat, calculate its correlation with win rate.
- Rank the stats from strongest to weakest association with winning.
- Optionally split offense vs. defense to see which side of the ball shows stronger links overall.

## Step 4: Create a visualization

- Make a bar chart of the top offensive and defensive stats ranked by association with win rate.
- Add a scatter plot for the strongest predictor (x-axis = that stat, y-axis = win rate) with one point per team-season.
- Label axes clearly and title the charts so the comparison is obvious.
- Use color or separate panels to distinguish offensive stats from defensive stats.

## Step 5: Interpret results

- State which offensive and defensive stats showed the strongest relationship with win rate over the last five years.
- Explain the pattern in plain language (for example, “teams that allow fewer points tend to win more”).
- Note limitations: correlation is not causation, rule/scheme changes across seasons, and small sample of seasons.
- Suggest one follow-up (for example, check whether the same stats matter in the playoffs, or control for strength of schedule).

