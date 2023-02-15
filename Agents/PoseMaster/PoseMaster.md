## PoseMaster WalkCycle Legs Example


https://user-images.githubusercontent.com/44372160/219148209-e9e14cc1-722b-4244-947d-d2ef806b2f1d.mp4



```
# SETTING PARSELTONGUE CONTEXT
jargon studio animation

# SETTING-UP SCENE
import character princess from princess in princess as princess
import object lights from princess in lights as studio lights
import object camera from zoom camera in camera as camera

# STARTING POSE (walk base)
posemaster princess
princess left thigh turn right side 10deg mirror, flip
princess save pose lr as walk base

# CONTACT POSE
princess load pose walk base
princess left thigh turn down side 20deg mirror, flip
princess hip arh root 180, 0.75, 0.0, translate
princess left toes lock to left calf, right leg tail to right calf 
princess left toes disc arh root  0, 0.0, -0.3, right leg  0, -0.05, 0.25
princess release left toes, right leg
princess save pose tr as walk contact

# STEP-DOWN POSE
princess load pose walk base
princess left thigh turn down side 20deg mirror, flip
princess hip arh root 180, 0.72, 0.0, translate
princess left toes lock to left calf, right leg tail to right calf 
princess left toes disc arh root  0, 0.0, 0.35, right leg  0, -0.05, 0.2
princess release left toes, right leg
princess save pose tr as walk down

# PASS POSE
princess load pose walk base
princess hip arh root 180, 0.76, 0.0, translate
princess left thigh turn up 20deg
princess left toes lock to left calf, right leg to right calf 
princess left toes disc arh root  -90, 0.09, 0, right leg  0, 0, 0
princess release left toes, right leg
princess save pose tr as walk pass

# LIFT-UP POSE
princess load pose walk base
princess hip arh root 180, 0.78, 0.0, translate
princess left thigh turn up 30deg
princess left toes lock to left calf, left leg to left calf 
princess left toes disc arh root  0, 0, -0.15, right leg  0, -0.1, 0.25
princess right thigh turn down 20deg
princess left leg turn up 20deg
princess release left toes, left leg
princess save pose tr as walk up

# WRITING LEFT LEG TO TIMELINE THEN MIRRORING SAME TO RIGHT LEG

princess load pose walk base
princess advance frame by absolute 1
princess load pose tr walk contact
princess write pose

princess advance frame by absolute 3
princess load pose tr walk down
princess write pose

princess advance frame by absolute 8
princess load pose tr walk pass
princess write pose

princess advance frame by absolute 12
princess load pose tr walk up
princess write pose

princess advance frame by absolute 16
princess copy pelvis yz from frame 1, mirror 1, -1, mirror 1, -1
princess write pose

princess advance frame by relative 2
princess copy pelvis yz from frame 3, mirror 1, -1, mirror 1, -1
princess write pose

princess advance frame by relative 7
princess copy pelvis yz from frame 8, mirror 1, -1, mirror 1, -1
princess write pose

princess advance frame by relative 11
princess copy pelvis yz from frame 12, mirror 1, -1, mirror 1, -1
princess write pose

princess advance frame by relative 15
princess copy pelvis yz from frame 16, mirror 1, -1, mirror 1, -1
princess write pose

# STASHING FOR REUSABILITY, REPITION & MIXING ACTIONS (NLA:Non-Linear Animation)

princess stash action repeat 8x as legs walk
```
## PoseMaster Advanced Clenching Fingers Example


```
princess turned her left thigh to right by 10 degrees mirrored
left upperarm right 80% mirror opposite, right lowerarm up 20 mirror 100%,
left index 01 down 400% ,mirror, flip 02 up 90deg mirror
```