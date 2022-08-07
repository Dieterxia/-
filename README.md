# 视频处理一致性方法
## 传统方法
1. 差距过大帧为前后帧的平均
## 深度学习
1. 利用全局的几何一致性来约束随机两帧训练（离线处理视频，随机两帧，通过估计的光流映射和相机位姿和深度映射到另一帧的一致性来约束深度图的稳定性）
(Luo, Xuan, et al. "Consistent video depth estimation." ACM Transactions on Graphics (ToG) 39.4 (2020): 71-1.
)
2. 使用循环框架，利用时序信息（Lin, Shanchuan, et al. "Robust high-resolution video matting with temporal guidance." 
Proceedings of the IEEE/CVF Winter Conference on Applications of Computer Vision. 2022.
）
3. 利用前馈和反馈的特征传播（离线增强）（Lee, Junyong, et al. 
"Reference-based Video Super-Resolution Using Multi-Camera Video Triplets." 
Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. 2022.
）
4. 第一帧处理后，之后帧处理+tracking（有些SOT（第一帧模板和搜索区域，single object tracking），
VOS（和历史帧特征对比，video object segmentation），MOT(Tracking+Detection，Multiple object Tracking)任务）（）
