# Offseason Setup

List of decrees and bonuses for the end of the season

## Endpoint

`https://blaseball.com/database/offseasonSetup`

## Response

```json
{
    "decrees": [
        {
            "_id": "eat_the_rich",
            "type": 7,
            "title": "Eat the Rich",
            "description": "Redistribute the funds from the Top 1% of Fans at the end of each Season",
            "votes": 0
        },
        {
            "_id": "eat_the_crust",
            "type": 8,
            "title": "Eat the Crust",
            "description": "5 Players from the 2-Time Champion Pies will be reassigned to Random Teams",
            "votes": 0
        },
        {
            "_id": "interviews",
            "type": 9,
            "title": "Interviews",
            "description": "GET TO KNOW THE PLAYERS",
            "votes": 0
        },
        {
            "_id": "late_stage",
            "type": 10,
            "title": "Late Stage",
            "description": "Postseason Bet Payouts increase each round: 2x, 3x, 5x",
            "votes": 0
        },
        {
            "_id": "blaserunning",
            "type": 11,
            "title": "Blaserunning",
            "description": "Stolen Bases are worth 0.1 Runs",
            "votes": 0
        }
    ],
    "bonuses": [
        {
            "_id": "anticapitalism",
            "type": 31,
            "value": 1,
            "title": "Anticapitalism, brought to you by Friends at the Table",
            "description": "Your team will become fully anticapitalist.",
            "votes": 0
        },
        {
            "_id": "division_baserunning_cut",
            "type": 44,
            "value": 0.1,
            "title": "Rigour Mortis",
            "description": "Stiff Limbs. -10% team baserunning to your team's division opponents.",
            "votes": 0
        },
        {
            "_id": "team_improve_baserunning",
            "type": 2,
            "value": 0.15,
            "title": "Evil Wind Sprints",
            "description": "The Wind can be Evil. Run. +15% Team Baserunning",
            "votes": 0
        },
        {
            "_id": "max_random_player",
            "type": 22,
            "value": 1,
            "title": "Bloodlust",
            "description": "URRRRRRGGHHHHHH. Maxes the stats of a random player on your team.",
            "votes": 0
        },
        {
            "_id": "steal_best_player",
            "type": 25,
            "value": 1,
            "title": "Highway Robbery",
            "description": "The best player in the league joins your team.",
            "votes": 0
        },
        {
            "_id": "steal_best_player_subleague",
            "type": 34,
            "value": 1,
            "title": "Headhunter",
            "description": "The best hitter in your team's subleague (Good or Evil) joins your team.",
            "votes": 0
        },
        {
            "_id": "steal_best_player_division",
            "type": 35,
            "value": 1,
            "title": "Vulture",
            "description": "The best player in your team's division joins your team.",
            "votes": 0
        },
        {
            "_id": "variable_team_hitting",
            "type": 37,
            "value": 0.2,
            "title": "Pretty Plz?",
            "description": "Feed your hitters coffee grounds. Team hitting changes from -5% to +15%",
            "votes": 0
        },
        {
            "_id": "reroll_worst_players_3",
            "type": 10,
            "value": 3,
            "title": "Team-Building Exercise",
            "description": "Re-rolls your team's three worst players",
            "votes": 0
        },
        {
            "_id": "summoning_circle",
            "type": 12,
            "value": 3,
            "title": "Summoning Circle",
            "description": "Re-rolls your team's 3 worst hitters",
            "votes": 0
        },
        {
            "_id": "exploratory_surgeries",
            "type": 11,
            "value": 3,
            "title": "Exploratory Surgeries",
            "description": "Re-rolls your team's worst 3 pitchers",
            "votes": 0
        },
        {
            "_id": "team_improve_overall",
            "type": 4,
            "value": 0.08,
            "title": "Performance Enhancing Demons",
            "description": "Mggoka match ng strike fm'latghor. Fm'latgh. +8% Team Overall",
            "votes": 0
        },
        {
            "_id": "team_improve_pitching",
            "type": 1,
            "value": 0.1,
            "title": "Pseudo-Thumbs",
            "description": "Pseudo-Thumbs burst from the skin on the opposite of your pitchers' hands. +10% Team Pitching",
            "votes": 0
        },
        {
            "_id": "team_improve_defense",
            "type": 3,
            "value": 0.15,
            "title": "The Rack",
            "description": "[cartilage and bone snapping]  +15% Team Defense",
            "votes": 0
        },
        {
            "_id": "send_worst_hitter",
            "type": 30,
            "value": 1,
            "title": "Exile",
            "description": "Send your team's worst hitter to a random other team. Receive a random player back.",
            "votes": 0
        },
        {
            "_id": "send_worst_pitcher",
            "type": 29,
            "value": 1,
            "title": "Go Away",
            "description": "Send your team's worst pitcher to a random team. Receive a random player back.",
            "votes": 0
        }
    ],
    "decreesToPass": 2
}
```

## Field Descriptions

**`decrees`**: List of decrees.

**`decrees.type`**: Integer id of the decree.

**`decrees.title`**: The title displayed in the election page.

**`decrees.description`**: What will happen if this decree is enacted.

**`decrees.votes`**: How many votes this decree has (always 0 because setup?).

**`bonuses`**: List of bonuses

**`bonuses.type`**: Integer id of the bonus.

**`bonuses.value`**: Unknown

**`bonuses.title`**: The title displayed in the election page.

**`bonuses.description`**: What will happen from this bonus.

**`bonuses.votes`**: Always zero?

**`decreesToPass`**: How many decrees will take effect