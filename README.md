# Embodied-AI-Learning

这是一个伟大项目，将记录我的具身智能学习过程。

## 简介

用于记录具身智能的学习。这是我的学习笔记仓库。

## 学习内容

- [ ] 基础概念
- [ ] 算法实现
- [ ] 项目实践
- [ ] 论文阅读

## 学习路线

### 模块一：机器人学基础 (The "Body" Logic)
具身智能的输出端通常是动作（Action）。理解坐标系和运动学是调试机器人的基础。

**核心知识点：**
- 空间描述与变换：熟练掌握旋转矩阵、四元数（Quaternion）、欧拉角，理解空间本质。
- URDF 文件解析：理解 Link（连杆）和 Joint（关节）的嵌套关系。
- 运动学 (Kinematics)：
  - 前向运动学 (FK)：给定关节角，求末端执行器位置。
  - 逆向运动学 (IK)：给定末端执行器位置，求关节角。

**推荐学习资源：**
- 经典教材：《机器人学导论》(Introduction to Robotics) by John Craig
- 必读文档：ROS Wiki 的坐标变换 (tf2) 教程

---

### 模块二：3D 视觉与表征学习 (The "Eyes" of AI)
具身智能需要感知深度和物体的 3D 属性。

**核心知识点：**
- RGB-D 感知：理解深度图（Depth Map）与点云（Point Cloud）转换。
- 视觉表征：
  - CLIP (Contrastive Language-Image Pre-training)：图像与文本的联合表征。
  - ViT (Vision Transformer)：现代具身智能模型的主干。
- 物体分割：SAM (Segment Anything Model)，实现物体分割以辅助抓取。

**必读论文：**
- CLIP: Learning Transferable Visual Models From Natural Language Supervision (Radford et al., 2021)
- ViT: An Image is Worth 16x16 Words (Dosovitskiy et al., 2020)
- VC-1: Visual Cortical Mechanisms for Embodied AI (Majumdar et al., 2023)

---

### 模块三：仿真环境与交互基础 (The "Gym" for AI)
大部分实验需在仿真器中完成。

**核心知识点：**
- 物理引擎基础：碰撞检测、摩擦力模型。
- 主流仿真器：
  - Isaac Gym/Sim：NVIDIA 出品，GPU 加速，适合大规模强化学习。
  - PyBullet / MuJoCo：适合单体机器人精细操作。
- 动作空间 (Action Space)：理解连续与离散动作空间。

**必读论文/文档：**
- Embodied AI: A Survey (Duan et al., 2022)
- Habitat: A Platform for Embodied AI Research (Savva et al., 2019)

## 贡献

欢迎提交问题和建议。
