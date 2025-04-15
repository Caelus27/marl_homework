### 1.安装openAI的Multiagent-particle-envs，
### 2.下载克隆maddpg开源项目文件openai/maddpggithub.com到mpe的同一目录下
### /multiagent-particle-envs  $-->$ $ pip install e.
### /maddpg  $-->$ $ pip install e.

### 实例

simple_push:
介绍：此环境有 1 个良好代理、1 个对手和 1 个地标。优秀的经纪人根据到地标的距离获得奖励。
如果对手靠近地标，并且代理远离地标（距离差），则对手将获得奖励。因此，对手必须学会 将 
Good Agent 推离 Landmark。

训练指令：
python train.py --scenario simple_push --num-episodes 1000 --exp-name exp1 --save-dir "C:\Users\86178\Desktop\using things\multiagent-particle-envs\maddpg\experiments\model_push\exp1"

展示指令：
python train.py --scenario simple_push  --load-dir "C:\Users\86178\Desktop\using things\multiagent-particle-envs\maddpg\experiments\model_push\exp1" --display 

simple_tag:
介绍：猎人-猎物模型

python train.py --scenario simple_tag --num-episodes 1000 --exp-name tag_exp1 --save-dir "C:\Users\86178\Desktop\using things\multiagent-particle-envs\maddpg\experiments\model_tag\exp1"
python train.py --scenario simple_tag  --load-dir "C:\Users\86178\Desktop\using things\multiagent-particle-envs\maddpg\experiments\model_tag\exp1" --display