A short talk on how to measure/quantify "slow"?
Magical numbers: 0.1s 1s 10s
RAIL performance framework (guidelines):
 - Response: from tap to paint < 100ms
 - Animation: consistency is key, variable fps is worse than lower fps. Visual updates < 16ms (60 fps)
 - Idle: use the opportunity to compute when user is not interacting, but keep it in 50ms chunks to be ready to react. Difficult to achieve because there are no APIs yet.
 - Load: interactive in < 1s.