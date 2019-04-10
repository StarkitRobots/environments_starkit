# Kick Tuning

kicks are in
env/<name of the robot>kick_<classic|lateral|small>.json

(kick.json is not used any more)

## Work flow:

1) deploy and run
2) ssh into the robot and go in folder env/<name-of-the-robot>
3) rhio
    - go into moves/kick
    - put live to 1
    (in order to reload the json file at each kick)
4) modify the kick classic|lateral|small>.json
5) kickGen in rhio
6) test the kick:
    > kick on rhio

then go to 4)

Same for standup.

## remark

you can add a file for form
kick_<classic|lateral|small>_left.json
only left (the right is the default one)

## in rhio
- when tune parameters, use the 'diff' command to see your changes
- when you are happy, use the 'save' command, and the values are stored in
the env/rhio folder at the good place.
be carrefull the values are stored in the robot.
