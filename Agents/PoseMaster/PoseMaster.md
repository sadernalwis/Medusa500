## PoseMaster Example

```
jargon studio animation

posemaster princess
princess left thigh turn right side 10deg mirror, flip
princess save pose lr as walk base

princess load pose walk base
princess left thigh turn down side 20deg mirror, flip
princess hip arh root 180, 0.75, 0.0, translate
princess left toes lock to left calf, right leg tail to right calf 
princess left toes disc arh root  0, 0.0, -0.3, right leg  0, -0.05, 0.25
princess release left toes, right leg
princess save pose tr as walk contact

princess load pose walk base
princess left thigh turn down side 20deg mirror, flip
princess hip arh root 180, 0.72, 0.0, translate
princess left toes lock to left calf, right leg tail to right calf 
princess left toes disc arh root  0, 0.0, 0.35, right leg  0, -0.05, 0.2
princess release left toes, right leg
princess save pose tr as walk down

princess load pose walk base
princess hip arh root 180, 0.76, 0.0, translate
princess left thigh turn up 20deg
princess left toes lock to left calf, right leg to right calf 
princess left toes disc arh root  -90, 0.09, 0, right leg  0, 0, 0
princess release left toes, right leg
princess save pose tr as walk pass

princess load pose walk base
princess hip arh root 180, 0.78, 0.0, translate
princess left thigh turn up 30deg
princess left toes lock to left calf, left leg to left calf 
princess left toes disc arh root  0, 0, -0.15, right leg  0, -0.1, 0.25
princess right thigh turn down 20deg
princess left leg turn up 20deg
princess release left toes, left leg
princess save pose tr as walk up

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

princess stash action repeat 8x as legs walk
```
#### Comments Owl #[...]#
