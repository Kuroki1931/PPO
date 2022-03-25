# PPO

# 流れ
input-state-箱の位置、箱の速度、ポールの角度、角速度  
→
(4, 256)-relu-(256, 2)-softmax-Categorical
→
actionを得る
→
env.step(action)で次のstepへ。
T_horizon回学習を進めて、trajectory listを得る。

# 参考
https://github.com/seungeunrho/minimalRL
