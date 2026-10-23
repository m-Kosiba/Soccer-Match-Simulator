SOCCER MATCH SIMULATOR

BEGIN

    IMPORT random module

    CLASS Team

        CONSTRUCTOR
            Store team name
            Set score to 0
            Set total shots to 0
            Set shots on target to 0
        END CONSTRUCTOR

        METHOD take_shot
            Increase total shots by 1
            Randomly determine if shot is on target

            IF shot is on target THEN
                Increase shots on target by 1
                Randomly determine if a goal is scored

                IF a goal is scored THEN
                    Increase team score by 1
                END IF
            ELSE
                Set goal to false
            END IF

            Return goal and shot outcome
        END METHOD

        METHOD display_stats
            Display team name
            Display goals
            Display total shots
            Display shots on target
        END METHOD

    END CLASS

    CLASS SoccerMatch

        CONSTRUCTOR
            Store home team
            Store away team
            Set match duration to 90 minutes
        END CONSTRUCTOR

        METHOD simulate_match
            Display match title and team names

            FOR each five-minute interval from 5 to 90

                FOR each team
                    Randomly determine if shooting chance occurs

                    IF shooting chance occurs THEN
                        Call take_shot
                        Display shot outcome
                    END IF
                END FOR

                IF minute equals 45 THEN
                    Display halftime score
                END IF

            END FOR

            Display final score
            Display both teams' statistics
            Determine winner or draw
        END METHOD

        METHOD display_score
            Display both team names and scores
        END METHOD

        METHOD display_winner
            Compare the two team scores

            IF home team has more goals THEN
                Display home team as winner
            ELSE IF away team has more goals THEN
                Display away team as winner
            ELSE
                Display that the match is a draw
            END IF
        END METHOD

    END CLASS

    Create home team named Immaculata
    Create away team named Opponent
    Create SoccerMatch object using both teams
    Run the match simulation

END