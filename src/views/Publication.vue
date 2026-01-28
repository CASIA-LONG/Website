<template>
  <div class="publication">
    <div class="container">
      <h1>Publications</h1>
      <div class="publication-list">
        <ol>
          <li>Xuemin Hu, Pan Chen, Yijun Wen, Bo Tang, <strong>Long Chen</strong>. Long-and Short-Term Constraint-Driven Safe Reinforcement Learning for Autonomous Driving. 2026.</li>
          <li>Xiaotong Zhang, Yuanjing Wang, Siyu Teng, Luxi Li, <strong>Long Chen</strong>. Alternating Partition Prioritized Planning for Scalable Multi-Robot Coordination in Congested Environments. 2025.</li>
          <li><strong>Long Chen</strong>, Ye Zhao, Ziyuan Wang, Aoming Zhan, Jinyu Gao, Bing Li, Yumei Zhou, Shushan Qiao. A Brain-Inspired Intelligent Vision Sensor With Spiking Processing-in-Sensor Architecture for Spike Feature Encoding. 2025.</li>
          <li>Xianda Guo, Chenming Zhang, Youmin Zhang, Wenzhao Zheng, Dujun Nie, Matteo Poggi, <strong>Long Chen</strong>. Lightstereo: Channel Boost is All You Need for Efficient 2D Cost Aggregation. 2025.</li>
          <li>Yuchen Li, Luxi Li, Zhenshan Bing, Libo Sun, Alois Christian Knoll, Fei-Yue Wang, <strong>Long Chen</strong>. A Visual Benchmark for Autonomous Driving in Open-Pit Mines. 2025.</li>
          <li>Xianda Guo, Wenjie Yuan, Yunpeng Zhang, Tian Yang, Chenming Zhang, Zheng Zhu, Qin Zou, <strong>Long Chen</strong>. Adjacent-view Transformers for Supervised Surround-view Depth Estimation. 2025.</li>
          <li>Dujun Nie, Xianda Guo, Yiqun Duan, Ruijun Zhang, <strong>Long Chen</strong>. WMNav: Integrating Vision-Language Models into World Models for Object Goal Navigation. 2025.</li>
          <li>Jinyu Gao, Ye Zhao, Ziyuan Wang, <strong>Long Chen</strong>, Aoming Zhan, Qihang Jiang, Feng Zhang, Yong Chen, Shushan Qiao. A General-Purpose Computing Core With Cooperative Motion Detection and Feature Extraction for Always-On PWM Image Sensors. 2025.</li>
          <li>Yunfeng Ai, Xinqing Li, Ruiqi Song, Chenglin Cui, Bin Tian, <strong>Long Chen</strong>, Fei-Yue Wang. PMScenes: A Parallel Mine Dataset for Autonomous Driving in Surface Mines. 2025.</li>
          <li>Siyu Teng, Yutong Wang, Xingxia Wang, Juanjuan Li, Yuchen Li, Xiaotong Zhang, Lingxi Li, Long Chen, Fei-Yue Wang. The ParallelWorkforce: A Framework for Synergistic Collaboration in Digital, Robotic, and Biological Workers of Industry 5.0. 2025.</li>
          <li>Yuchen Li, Luxi Li, Siyu Teng, Zhenshan Bing, Alois Christian Knoll, Zhe Xuanyuan, <strong>Long Chen</strong>. Online Triangular Constraint Calibration for LiDAR and Cameras in Open-Pit Mines. 2025.</li>
          <li>Xuan Yuwen, Jicheng Chen, Bin Liu, Xin Wan, Kai Wen, <strong>Long Chen</strong>, Hui Zhang. Vision-Based Road Segmentation With Active Gaze Control for Autonomous Vehicles. 2025.</li>
          <li>Wenxuan Li, Qin Zou, Chi Chen, Bo Du, <strong>Long Chen</strong>, Jian Zhou, Hongkai Yu. Co-Fix3D: Enhancing 3D Object Detection With Collaborative Refinement. 2025.</li>
          <li><strong>Long Chen</strong>, Peng Deng, Lingxi Li, Xuemin Hu. Mixed Motivation Driven Social Multi-Agent Reinforcement Learning for Autonomous Driving. 2025.</li>
          <li>Yuchen Li, <strong>Long Chen</strong>, Lingxi Li, Xuemin Hu. MiningEye: A Textual Explanation Method for Autonomous Driving and Intelligent Transportation in Open-pit Mines. 2025.</li>
        </ol>
      </div>
    </div>
  </div>
</template>

<script setup>
// Publication page logic
</script>

<style scoped>
/* Publication Page Styles */
.publication {
  padding: 4rem 0;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 1.5rem;
}

.publication h1 {
  font-size: 2.5rem;
  margin-bottom: 3rem;
  text-align: center;
  color: #1a237e;
  position: relative;
}

.publication h1::after {
  content: '';
  display: block;
  width: 80px;
  height: 3px;
  background-color: #2196f3;
  margin: 1rem auto 0;
}

.publication-list {
  margin-top: 2rem;
}

.publication-list ol {
  padding-left: 2rem;
  list-style-position: outside;
}

.publication-list li {
  margin-bottom: 2rem;
  line-height: 1.7;
  color: #333;
  padding: 1.5rem;
  background-color: #f9f9f9;
  border-radius: 8px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
  transition: all 0.3s ease;
  border-left: 4px solid #2196f3;
}

.publication-list li:hover {
  transform: translateX(5px);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  background-color: #f5f5f5;
}

.publication-list strong {
  font-weight: 600;
  color: #1a237e;
}

/* Responsive Design */
@media (max-width: 768px) {
  .publication {
    padding: 3rem 0;
  }
  
  .publication h1 {
    font-size: 2rem;
  }
  
  .publication-list li {
    padding: 1.2rem;
    margin-bottom: 1.5rem;
  }
}

@media (max-width: 480px) {
  .publication h1 {
    font-size: 1.8rem;
  }
  
  .publication-list ol {
    padding-left: 1.5rem;
  }
  
  .publication-list li {
    padding: 1rem;
  }
}
</style>