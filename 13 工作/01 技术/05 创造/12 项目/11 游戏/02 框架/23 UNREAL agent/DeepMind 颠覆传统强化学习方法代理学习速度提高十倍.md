
# DeepMind 颠覆传统强化学习方法代理学习速度提高十倍


DeepMind 最近的论文《非监督辅助任务中的强化学习》（”[REINFORCEMENT LEARNING WITH UNSUPERVISED AUXILIARY TASKS](https://arxiv.org/pdf/1611.05397.pdf)”）介绍了一种极大提高代理学习速度和最终成效的方法。研究人员通过**让代理在训练中执行两个附加任务，来对标准的深度强化学习方法进行增强”**

Deepmind 表示：“我们的目标是开拓 AI 领域的最前沿，开发出能通过学习解决任何难题，而无须人类教它怎么做的程序。我们的强化学习代理（agent）已经在围棋和雅利达 2600 （Atari 2600, 1970年代的游戏主机）的游戏中有了重大突破。然而，这些游戏需要很多数据和很长的时间来学习。所以我们一直在寻找提高通用学习算法的途径。”

DeepMind 代理在迷宫游戏中执行搜索任务的演示如下图：

**![DeepMind 黑科技！颠覆传统强化学习方法，代理学习速度提高十倍（附视频）](https://static.leiphone.com/uploads/new/article/740_740/201611/582eb2ea7a786.gif)**

**第一个任务涉及，让代理学习怎样控制屏幕上的像素（通过移动看到不同的东西）。这强调了对迷宫游戏中“行动影响你所看到的东西”这一原则的学习，而不是仅仅做出预测。**这类似于婴儿学习控制他们手臂的过程：试图移动双手，观察做出的动作，然后进行调整。通过学习怎么移动来改变屏幕显示的东西，DeepMind 代理学会了对玩这个游戏很有用的视觉输入，并且拿到更高的得分。

**在第二个任务中，代理被训练，怎样从简短的历史背景中预测一系列即将获得的奖励。**为了更好地处理这个情况。当奖励很少时，开发人员向代理按照同等的比例，展示过去获得奖励和没有获得奖励的历史。更高频率地学习奖励的历史之后，这个代理能更快速地发现会带来预期奖励的视觉信号。

这两个附加任务的组合，还有 DeepMind 之前的 A3C 研究成就了他们的全新**“非监督强化和附加学习代理”**（UNREAL agent，UNsupervised REinforcement and Auxiliary Learning agent，下文简称 UNREAL 代理) 。DeepMind 在 57 个雅利达游戏，和一个 叫“迷宫”的 13 层 3D 环境中测试了这个代理。在所有的游戏中，基于原始图像输出， UNREAL 代理被用同样的方式训练。目的是让它做出使游戏得分和奖励最大化的行动。





为获得游戏奖励而需要作出的行动很复杂，从捡起 3D 地图中的苹果到玩“外星入侵”（Space Invaders）。UNREAL 算法经常学着玩这些游戏，学着学着就达到、甚至超越人类的水平。部分结果和可视化展示呈现在下面的视频：


在“迷宫”游戏中，使用两项附加任务（控制屏幕上像素和预测奖励何时发生）的效果出奇的好。**UNREAL  代理能够以超出 DeepMind 现役最好的 A3C 代理十倍的速度学习，并且有远远更好得表现** （游戏得分和奖励）**。Deepmind 的代理平均在每个迷宫层中达到人类专家水平的 87% ，并在一部分迷宫层中有超人类的水平。在雅利达游戏中，这个代理平均达到人类水的九倍。**Deepmind 表示，他们希望这项研究能让他们继续提高代理的水平，让它完成更的复杂任务。

附：有兴趣的技术宅们请点此查看 DeepMind 论文原文 “[REINFORCEMENT LEARNING WITH UNSUPERVISED AUXILIARY TASKS](https://arxiv.org/pdf/1611.05397.pdf)”。



# 相关

- [DeepMind 黑科技！颠覆传统强化学习方法，代理学习速度提高十倍（附视频）](https://www.leiphone.com/news/201611/TYsrMIlxkaROJ9q0.html)
