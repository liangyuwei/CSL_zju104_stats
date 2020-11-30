# 中国手语示教数据统计
By: 浙江大学 104机器人实验室
Author: Yuwei Liang




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


## <span id="intro">简介</span>
中国手语 - Chinese Sign Language (CSL)     

本仓库记录每次采集手语示教数据的统计结果。    

示教数据包含手臂运动数据（动捕）、手指运动数据（数据手套）和对应的视频，经由ROS message_filter同步，以rosbag的形式保存。详见[sign_language_robot](https://github.com/liangyuwei/sign_language_robot/arm_hand_capture)仓库。    


## <span id="2020-11-27">手语示教数据统计记录 - 2020年11月27日，星期五</span>

#### <span id="calib-2020-11-27">数据手套标定数据</span>    

本次手语示教数据采集分上午、下午两次，采集了2次的数据手套标定数据，位于```calib_files-all-day```文件夹下，包括2个txt(左右手)文件与5个bag文件:    
```calib_{l/r}-20201127-{morning/afternoon}```: Wiseglove数据手套SDK提供的标定数据。   
```hand_length.bag```: 可以从左右腕的相对位置，得到单手的近似的长度大小。   
```lr_all_open.bag, lr_all_close.bag```: 在手掌展平的情况下，张开五指或合拢五指。    
```lr_thumb_s14_90.bag```: 拇指绕食指旋转90°，用于标定手套的S14传感器。  
```lr_index_middle_crossover.bag```: 食指、中指交叉，用于类似中国手语里的“是”动作。   

详见Github 仓库```sign_language_robot```中```arm_hand_capture```包的[README](https://github.com/liangyuwei/sign_language_robot/arm_hand_capture/README.md)。   


#### <span id="data-2020-11-27">手语词句统计表</span>
数据包含4段场景对话和若干独立单词。我们对场景对话的单个单词和句子都进行了采集。     

1. 场景1 - YuMi机器人自我介绍    

  (1) 全文
> 我是机器人玉米。
> 
> 我会手语表演(打手语)。
> 
> 给予我这个能力的是浙江大学机器人实验室。

  (2) 文件夹
```yumi_intro/```     

  (3) 单词
| Bag名(.bag) | 中文含义 |
| :----: | :----: |
| wo | 我 |
| shi | 是 |
| yumi | 玉米 |
| jiqiren | 机器人 |
| hui | 会 |
| dashouyu | 打手语，手语表演 |
| jiyu | 给予 |
| zhege | 这个 |
| nengli | 能力 |
| de | 的 |
| zhejiang | 浙江 |
| daxue | 大学 |
| shiyanshi | 实验室 |

  (4) 句子
| Bag名(.bag) | 中文含义 |
| :----: | :----: |
| yumi1 | 我是机器人玉米。|
| yumi2 | 我会手语表演(打手语)。|
| yumi3 | 给予我这个能力的是浙江大学机器人实验室。|



2. 场景2 - 办理业务   
   

  (1) 全文
> 欢迎光临！您好！ 您要办理什么业务？
> 
> 请出示身份证。
> 
> 请填写有关信息。
> 
> 请稍等，我马上为您办理。
> 
> 请签名，办好了。
> 
> 还有什么需要办理的吗？
> 
> 好的，欢迎再次光临！请慢走，再见！

  (2) 文件夹
```banliyewu/```     

  (3) 单词
| Bag名(.bag) | 中文含义 |
| :----: | :----: |
| huanying | 欢迎 |
| guanglin | 光临 |
| ninhao | 您好 |
| yao | 要，需要 |
| banli | 办理 |
| shenme | 什么 |
| yewu | 业务 |
| qing | 请 |
| chushi | 出示 |
| shenfenzheng | 身份证 |
| tianxie | 填写 |
| youguan | 有关 |
| xinxi | 信息 |
| shaodeng | 稍等 |
| mashang | 马上 |
| wei | 为 |
| qianming | 签名 |
| banhaole | 办好了 |
| haiyou | 还有 |
| ma | 吗 |
| zaici | 再次 |
| manzou | 慢走 |
| zaijian | 再见 |

  (4) 句子
| Bag名(.bag) | 中文含义 |
| :----: | :----: |
| banyewu1 | 欢迎光临！您好！ 您要办理什么业务？|
| banyewu2 | 请出示身份证。 |
| banyewu3 | 请填写有关信息。 |
| banyewu4 | 请稍等，我马上为您办理。 |
| banyewu5 | 请签名，办好了。 |
| banyewu6 | 还有什么需要办理的吗？ |
| banyewu7 | 好的，欢迎再次光临！请慢走，再见！|



3. 场景3 - 问路1(去西湖)

  (1) 全文
> 你好！我去西湖边游玩，怎么走？
> 
> 你好！你可以沿着解放路一直向前走，就可以看到西湖了。
> 
> 也可以在这里乘车，到湖滨站下车，(穿)过马路往前走就到了。
> 
> 祝你玩得开心！再见！ 

  (2) 文件夹
```wenlu_xihu/```     

  (3) 单词
| Bag名(.bag) | 中文含义 |
| :----: | :----: |
| qu | 去，走 |
| xihubian | 西湖边 |
| youwan | 游玩 |
| zenme | 怎么|
| zou | 走 |
| keyi | 可以 |
| yanzhe | 沿着 |
| jiefanglu | 解放路 |
| yizhi | 一直 |
| xiang | 向，往 |
| qian | 前 |
| jiu | 就 |
| kandao | 看到 |
| ye | 也 |
| zai | 在 |
| zheli | 这里 |
| chengche | 乘车 |
| dao | 到 |
| hubin | 湖滨 |
| hubinzhan | 湖滨站 |
| xiache | 下车 |
| chuanguo | (穿)过 |
| malu | 马路 |
| zhu | 祝 |
| kaixin | 开心 |

  (4) 句子
| Bag名(.bag) | 中文含义 |
| :----: | :----: |
| wenlu1 | 你好！我去西湖边游玩，怎么走？ |
| wenlu2 | 你好！你可以沿着解放路一直向前走，就可以看到西湖了。 |
| wenlu3 | 也可以在这里乘车，到湖滨站下车，(穿)过马路往前走就到了。 |
| wenlu4 | 祝你玩得开心！再见！ |



4. 场景4 - 问路2(去火车东站)

  (1) 全文
> 你好！我去火车东站，乘几路公交车？
> 
> 你好！你可以在这里乘B4公交车，或者走到前面乘地铁1号线，都可以到火车东站。    

  (2) 文件夹
```wenlu_huochedongzhan/```     

  (3) 单词
| Bag名(.bag) | 中文含义 |
| :----: | :----: |
| huoche | 火车 |
| dongzhan | 东站 |
| jilu | 几路 |
| gongjiaoche | 公交车 |
| b | B |
| 4 | 4 |
| b4 | B4 |
| huozhe | 或者 |
| ditie | 地铁 |
| 1 | 1 |
| hao | 号 |
| xian | 线 |
| dou | 都 |

  (4) 句子
| Bag名(.bag) | 中文含义 |
| :----: | :----: |
| huochedongzhan1 |  你好！我去火车东站，乘几路公交车？ |
| huochedongzhan2 | 你好！你可以在这里乘B4公交车，或者走到前面乘地铁1号线，都可以到火车东站。 |



5. 场景5 - 医院挂号
   

  (1) 全文
> 你好！你哪里不舒服？
> 
> 你可以挂内科。
> 
> 请在自助机上挂号，也可以到窗口排队挂号。
> 
> 如有问题，可以找志愿者帮忙。    

  (2) 文件夹
```yiyuan/```     

  (3) 单词
| Bag名(.bag) | 中文含义 |
| :----: | :----: |
|  nali | 哪里 |
| bushufu | 不舒服 |
| gua | 挂 |
| neike | 内科 |
| zizhuji | 自助机 |
| 上面的gua(“挂”)搭配地铁1号线的“号” | 挂号 |
| chuangkou | 窗口 |
| paidui | 排队 |
| ru | 如，如果 |
| youwenti | 有问题 |
| zhao | 找 |
| zhiyuanzhe | 志愿者 |
| bangmang | 帮忙 |

  (4) 句子
| Bag名(.bag) | 中文含义 |
| :----: | :----: |
| yiyuan1 | 你好！你哪里不舒服？ |
| yiyuan2 | 你可以挂内科。|
| yiyuan3 | 请在自助机上挂号，也可以到窗口排队挂号。 |
| yiyuan4 | 如有问题，可以找志愿者帮忙。 |



6. 零散单词

  (1) 全文
> 称谓:  人  人民  公民  市民  自己  我们  你们  他们  大家  群众  同志  同事  同学  朋友  
> 
> 职业:  工人  农民  牧民  公务员  教师  教练  记者  作家  画家  医生  护士  学生  律师  解放军
> 
> 职务:  校长(院长)  教授  讲师  学位  学历  研究生  学士  硕士  博士
> 
> 食品:  面包  蛋糕  饼干  点心  罐头  果脯  包子  饺子  馄饨  面条  饼  年糕  油条  粽子  汤圆  
> 
> 水果:  菠萝  西瓜  苹果  梨  香蕉  哈密瓜  草莓  橘子  葡萄  
> 
> 交通 通讯:  交通  道路  桥  立交桥  车站  火车  地铁  汽车  卡车  电车  公共汽车  摩托车  自行车  出租汽车  救护车  船  飞机  通讯  信息  挂号信  手机  微信  
> 
> 医院:  挂号处  外科  内科  放射科  门诊  诊疗室  会诊  心电图  化验  CT  B超  治疗  急救  药  药方  西药  中药     

  (2) 文件夹
```words/```     

  (3) 称谓(```words/chengwei/```)
| Bag名(.bag) | 中文含义 |
| :----: | :----: |
| ren | 人 |
| renmin | 人民 |
| gongmin | 公民 |
| shimin | 市民 |
| ziji | 自己 |
| women | 我们 |
| nimen | 你们 |
| tamen | 他们 |
| dajia | 大家 |
| qunzhong | 群众 |
| tongzhi | 同志 |
| tongshi | 同事 |
| tongxue | 同学 |
| pengyou | 朋友 |

  (4) 职业(```words/zhiye/```)
| Bag名(.bag) | 中文含义 |
| :----: | :----: |
| gongren | 工人 |
| nongmin | 农民 |
| mumin | 牧民 |
| gongwuyuan | 公务员 |
| jiaoshi | 教师 |
| jiaolian | 教练 |
| jizhe | 记者 |
|zuojia | 作家 |
| huajia | 画家 |
| yisheng | 医生 |
| hushi | 护士 |
| xuesheng | 学生 |
| lvshi | 律师 |
| jiefangjun | 解放军 |

  (5) 职务(```words/zhiwu/```)
| Bag名(.bag) | 中文含义 |
| :----: | :----: |
|  xiaozhangyuanzhang | 校长(院长) |
| jiaoshou | 教授 |
| jiangshi | 讲师 |
| xuewei | 学位 |
| xueli | 学历 |
| yanjiusheng | 研究生 |
| xueshi | 学士 |
| shuoshi | 硕士 |
| boshi | 博士 |

  (6) 食品(```words/shipin/```)
| Bag名(.bag) | 中文含义 |
| :----: | :----: |
| mianbao | 面包 |
| dangao | 蛋糕 |
| binggan | 饼干 |
| dianxin | 点心 |
| guantou | 罐头 |
| guofu | 果脯 |
| baozi | 包子 |
| jiaozi | 饺子 |
| huntun | 馄饨 |
| miantiao | 面条 |
| bing | 饼 |
| niangao | 年糕 |
| youtiao | 油条 |
| zongzi | 粽子 |
| tangyuan | 汤圆 |

  (7) 水果(```words/shuiguo/```)
| Bag名(.bag) | 中文含义 |
| :----: | :----: |
| boluo | 菠萝 |
| xigua | 西瓜 |
| pingguo | 苹果 |
| li | 梨 |
| xiangjiao | 香蕉 |
| hamigua | 哈密瓜 |
| caomei | 草莓 |
| juzi | 橘子 |
| putao | 葡萄 |

  (8) 交通 通讯(```words/jiaotongtongxun/```)
| Bag名(.bag) | 中文含义 |
| :----: | :----: |
| jiaotong | 交通 |
| daolu | 道路  |
| qiao | 桥 |
| lijiaoqiao | 立交桥 |
| chezhan | 车站 |
| huoche | 火车 |
| 前面场景对话中已有 | 地铁 |
| qiche | 汽车 |
| kache | 卡车 |
| dianche | 电车 |
| gonggongqiche | 公共汽车 |
| motuoche | 摩托车 |
| zixingche | 自行车 |
| chuzuqiche | 出租汽车 |
| jiuhuche | 救护车 |
| chuan | 船 |
| feiji | 飞机 |
| tongxun | 通讯 |
| xinxi | 信息 |
| guahaoxin | 挂号信 |
| shouji | 手机 |
| weixin | 微信 |

  (9) 医院(```words/yiyuan```)
| Bag名(.bag) | 中文含义 |
| :----: | :----: |
| guahaochu | 挂号处 |
| waike | 外科  |
| neike | 内科 |
| fangsheke | 放射科 |
| menzhen | 门诊 |
| zhenliaoshi | 诊疗室 |
| huizhen | 会诊 |
| xindiantu | 心电图 |
| huayan | 化验 |
| ct | CT |
| bchao | B超 |
| zhiliao | 治疗 |
| jijiu | 急救 |
| yaofang  | 药方 |
| xiyao | 西药 |
| zhongyao | 中药 |

