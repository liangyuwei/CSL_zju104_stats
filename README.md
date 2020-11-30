# 中国手语示教数据统计
By: 浙江大学 104机器人实验室
Author: Yuwei Liang

---

## 目录
- [简介](#intro)
- 手语示教数据统计记录
    - [2020年11月27日，星期五](#2020-11-27)
        - [数据手套标定数据](#calib-2020-11-27)
        - [手语词句统计表](#data-2020-11-27)
            - YuMi机器人自我介绍
            - 办理业务
            - 问路1(去西湖)
            - 问路2(去火车东站)
            - 医院挂号
            - 零散单词

---

## <span id="intro">简介</span>
中国手语 - Chinese Sign Language (CSL)     

本仓库记录每次采集手语示教数据的统计结果。示教数据包含手臂运动数据（动捕）、手指运动数据（数据手套）和对应的视频，经由ROS message_filter同步，详见[sign_language_robot](https://github.com/liangyuwei/sign_language_robot/arm_hand_capture)仓库。    

---

## <span id="2020-11-27">手语示教数据统计记录 - 2020年11月27日，星期五</span>

### <span id="calib-2020-11-27">数据手套标定数据</span>    
本次手语示教数据采集分上午、下午两次，采集了2次的数据手套标定数据，位于```calib_files-all-day```文件夹下，包括2个txt(左右手)文件与5个bag文件:    
```calib_{l/r}-20201127-{morning/afternoon}```: Wiseglove数据手套SDK提供的标定数据。   
```hand_length.bag```: 可以从左右腕的相对位置，得到单手的近似的长度大小。   
```lr_all_open.bag, lr_all_close.bag```: 在手掌展平的情况下，张开五指或合拢五指。    
```lr_thumb_s14_90.bag```: 拇指绕食指旋转90°，用于标定手套的S14传感器。  
```lr_index_middle_crossover.bag```: 食指、中指交叉，用于类似中国手语里的“是”动作。   

详见Github 仓库```sign_language_robot```中```arm_hand_capture```包的[README](https://github.com/liangyuwei/sign_language_robot/arm_hand_capture/README.md)。   


### <span id="data-2020-11-27">手语词句统计表</span>
数据包含4段场景对话和若干独立单词。我们对场景对话的单个单词和句子都进行了采集。

1. 场景1: YuMi机器人自我介绍
全文: 我是机器人玉米。我会手语表演(打手语)。给予我这个能力的是浙江大学机器人实验室。

2. 场景2: 办理业务


3. 场景3: 问路1(去西湖)


4. 场景4: 问路2(去火车东站)


5. 场景5: 医院挂号


6. 零散单词


---





