# NeuroProject

Once upon a time I was chatting with some friends and we wondered if, given two numbers, human brain takes longer to decide which one is greater. Does that depend on their difference? Does that depend on if they share the first digit? We conjectured that the more difference they have, the faster the brain can recognize which one is greater, but to find that out we designed this experiement.

This consists of several rounds where a number from 1 to 100 (and other than 50) is shown, and the user has to determine if it's smaller or greater than 50. After all these rounds, we store the time that the user took to decide in each case in a database to analyze them, as well as the numbers theirselves and if the user answered correctly.

Additionally, we also wanted to experiment with directions: The way that the user tells if the number is greater or smaller than 50 is by pressing the keys 'B' or 'Y', which are one right above the other in the standard QWERTY distribution. However, the twist is that, at the beginning of the experiment, we flip a coin to decide if the user will have to press the key 'Y' to express "greater" and 'B' for "smaller" or the other way around. Our second conjecture was that, since people already have set in our minds that "up" is related with "greater" and "down" with smaller (for instance, when we want to change the volume of the TV), the users that use 'Y' for "greater" and 'B' for "smaller" will decide faster or will have less mistakes than the other kind of users.

We used the framework jsPsych to model the experiment, and stored the data in a Supabase table. The files Experiment_es.html and Experiment_en.html contain the experiment in spanish and english respectively.
