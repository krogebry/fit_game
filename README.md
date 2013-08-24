fit_game
========

A game for fitness.


Use case
=========
Actor:
  Name: Bryan
  Role: Participant that is coming into the gym for a workout.

Actor:
  Name: Joe
  Role: Trainer.

Story:
  Bryan is coming in for a workout.  Joe is going to help encourage and motivate Bryan as well as guide him through the correct forms for the various stations.

  Bryan enters the gym and swipes his NFC-enabled gym card with Joe's reader.

  Joe's reader ( nexus, whatever ) loads the URL from the NFS tag: http://site.com/checkin/:member_id
  This will check the member in, but also load the profile into Joe's "active queue".

  Joe's active queue should give Joe the ability to quickly swipe through user profiles so he can take notes and rate performance.

  Once the workout is complete, Joe will close the session for Bryan.

  Once the session is closed, the game engine is invoked:
    * Analyze the workout performance.
    * Compare to previous workouts.
    * Assign bonuses and rewards.


