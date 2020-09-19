## happy path 1 (/tmp/tmphuqvs01p/dc84510ddf204f78b48ebeba1697f2e9_conversation_tests.md)
* greet: hello there!
    - utter_greet
* mood_great: amazing   <!-- predicted: greet: amazing -->
    - utter_happy   <!-- predicted: utter_greet -->


## happy path 2 (/tmp/tmphuqvs01p/dc84510ddf204f78b48ebeba1697f2e9_conversation_tests.md)
* greet: hello there!
    - utter_greet
* mood_great: amazing   <!-- predicted: greet: amazing -->
    - utter_happy   <!-- predicted: utter_greet -->
* goodbye: bye-bye!
    - utter_goodbye   <!-- predicted: utter_greet -->


## sad path 1 (/tmp/tmphuqvs01p/dc84510ddf204f78b48ebeba1697f2e9_conversation_tests.md)
* greet: hello
    - utter_greet
* mood_unhappy: not good   <!-- predicted: deny: not good -->
    - utter_cheer_up   <!-- predicted: utter_greet -->
    - utter_did_that_help   <!-- predicted: action_listen -->
* affirm: yes
    - utter_happy   <!-- predicted: utter_greet -->


## sad path 2 (/tmp/tmphuqvs01p/dc84510ddf204f78b48ebeba1697f2e9_conversation_tests.md)
* greet: hello
    - utter_greet
* mood_unhappy: not good   <!-- predicted: deny: not good -->
    - utter_cheer_up   <!-- predicted: utter_greet -->
    - utter_did_that_help   <!-- predicted: action_listen -->
* deny: not really
    - utter_goodbye   <!-- predicted: utter_greet -->


## sad path 3 (/tmp/tmphuqvs01p/dc84510ddf204f78b48ebeba1697f2e9_conversation_tests.md)
* greet: hi
    - utter_greet
* mood_unhappy: very terrible   <!-- predicted: deny: very terrible -->
    - utter_cheer_up   <!-- predicted: utter_greet -->
    - utter_did_that_help   <!-- predicted: action_listen -->
* deny: no
    - utter_goodbye   <!-- predicted: utter_greet -->


## say goodbye (/tmp/tmphuqvs01p/dc84510ddf204f78b48ebeba1697f2e9_conversation_tests.md)
* goodbye: bye-bye!
    - utter_goodbye   <!-- predicted: utter_greet -->


## bot challenge (/tmp/tmphuqvs01p/dc84510ddf204f78b48ebeba1697f2e9_conversation_tests.md)
* bot_challenge: are you a bot?   <!-- predicted: get_a_meeting: are you a bot? -->
    - utter_iamabot   <!-- predicted: utter_greet -->


