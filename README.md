# Yiya
一个无字典分词程序，名字来源于汉语“咿呀学语”。

- 输出频率最高的100个词，不含字本身信息

```java
String text = "xxx";
Yiya.topn(text, 100).forEach(System.out::println);
```

- 输出频率最高的100个词

```java
String text = "xxx";
Yiya.words(text, 100).forEach(System.out::println);
```

- 输出所有词

```java
String text = "xxx";
Yiya.words(text).forEach(System.out::println);
```

例如《三国演义》前100个词为

> 玄德
  孔明
  却说
  丞相
  云长
  荆州
  夏侯
  吕布
  诸葛
  商议
  孙权
  魏延
  赵云
  左右
  刘备
  司马懿
  姜维
  次日
  东吴
  袁绍
  周瑜
  陛下
  都督
  黄忠
  张郃
  先锋
  孟获
  邓艾
  诸葛亮
  后人有诗
  张辽
  成都
  徐晃
  喊声
  百姓
  祁山
  鲁肃
  接应
  董卓
  分付
  许褚
  粮草
  文武
  皇叔
  追赶
  夏侯惇
  洛阳
  兄弟
  星夜
  挺枪
  孙乾
  西川
  准备
  袁术
  刘璋
  司马昭
  甘宁
  英雄
  夏侯渊
  孟达
  乘势
  吕蒙
  朝廷
  陆逊
  首级
  襄阳
  李傕
  埋伏
  坚守
  箭射
  庞统
  心腹
  樊城
  郭淮
  廖化
  李典
  汉室
  连夜
  本部
  胜负
  声大震
  子敬
  冀州
  细作
  交锋
  拜谢
  西凉
  从其言
  饮酒
  如之奈何
  太史
  程普
  设宴
  搦战
  礼毕
  许昌
  两个
  厮杀
  慌忙
  性命

《水浒传》前100个词

> 李逵
  武松
  林冲
  哥哥
  吴用
  太尉
  智深
  梁山
  戴宗
  梁山泊
  兄弟
  卢俊义
  燕青
  先锋
  花荣
  晁盖
  王庆
  石秀
  甚么
  杨志
  柴进
  鲁智深
  呼延灼
  秦明
  和尚
  史进
  公孙胜
  张顺
  兄长
  有诗为证
  关胜
  性命
  朱仝
  阮小
  商议
  庄客
  杨雄
  东京
  随即
  许多
  小喽啰
  背后
  洒家
  收拾
  朴刀
  高太尉
  慌忙
  英雄
  朝廷
  分付
  雷横
  徐宁
  枢密
  安排
  西门庆
  刘唐
  解珍
  解宝
  方腊
  寻思
  员外
  琼英
  乔道清
  孙立
  左右
  高俅
  童贯
  董平
  索超
  梁中书
  师父
  包裹
  忠义
  必然
  吴学究
  传令
  押司
  施恩
  黄信
  方才
  城池
  解珍解宝
  朱贵
  百姓
  黑旋风
  宿太尉
  迎接
  衣服
  田虎
  言语
  济州
  虞候
  恁地
  招安
  燕顺
  其余
  提辖
  毕竟
  消息
  备细

《红楼梦》前100个词

> 凤姐
  姑娘
  奶奶
  自己
  东西
  告诉
  姨妈
  所以
  薛姨妈
  探春
  紫鹃
  妹妹
  鸳鸯
  湘云
  李纨
  答应
  媳妇
  晴雯
  尤氏
  姥姥
  刘姥姥
  薛蟠
  到底
  香菱
  明白
  已经
  哥哥
  麝月
  越发
  意思
  喜欢
  周瑞
  小厮
  果然
  主意
  瞧瞧
  跟前
  惜春
  丫鬟
  况且
  悄悄
  雨村
  吩咐
  女孩
  兄弟
  衣裳
  言语
  金桂
  多少
  芳官
  雪雁
  糊涂
  奴才
  伏侍
  迎春
  许多
  嬷嬷
  林之孝
  预备
  赵姨娘
  姊妹
  收拾
  年纪
  父亲
  倘或
  祖宗
  光景
  婶娘
  亲戚
  原故
  愿意
  伺候
  秦钟
  焙茗
  秋纹
  少不得
  薛蝌
  商议
  容易
  高兴
  岫烟
  细细
  林妹妹
  听了这话
  潇湘
  湘莲
  老祖宗
  怡红院
  可怜
  横竖
  交给
  叔叔
  料理
  热闹
  司棋
  慢慢
  工夫
  士隐
  索性
  荣府

《西游记》前100个词

> 八戒
  师父
  和尚
  菩萨
  怎么
  什么
  悟空
  徒弟
  呆子
  闻言
  兄弟
  宝贝
  取经
  铁棒
  东土
  果然
  性命
  公主
  神通
  玉帝
  变作
  哥哥
  土地
  欢喜
  贫僧
  太宗
  陛下
  爷爷
  金箍
  多少
  兵器
  模样
  袈裟
  变化
  手段
  娘娘
  衣服
  吩咐
  师徒们
  仔细
  左右
  金箍棒
  所以
  奈何
  观音
  安排
  钉钯
  叩头
  关文
  五百
  毫毛
  递与
  汝等
  筋斗
  许多
  战兢兢
  齐天大圣
  孩儿
  扯住
  毕竟
  忍不住
  小的们
  收拾
  佛祖
  皇帝
  玄奘
  葫芦
  壁厢
  未曾
  造化
  揭谛
  求经
  毕竟不知
  罗刹
  受用
  诗曰
  可怜
  御弟
  磕头
  摇身一变
  雷音
  花果山
  文武
  合掌
  咒语
  厉声
  哪吒
  木叉
  耳朵
  须臾
  保护
  直至
  马匹
  东土大唐
  列位
  为证
  传旨
  好歹
  悟净
  昨日

还有我喜欢的《隋唐演义》

> 叔宝
  炀帝
  玄宗
  雄信
  萧后
  陛下
  禄山
  伯当
  什么
  润甫
  宇文
  建德
  娘娘
  懋功
  许多
  自己
  老爷
  线娘
  杨妃
  秦琼
  贾润甫
  李密
  吩咐
  左右
  力士
  玄邃
  梅妃
  李靖
  尉迟
  怎么
  朋友
  国忠
  员外
  安禄山
  咬金
  单雄信
  肃宗
  世充
  收拾
  敬德
  朝廷
  高力士
  总管
  潞州
  建威
  刺史
  单二哥
  国桢
  程知节
  英雄
  百姓
  贵妃
  母亲
  紫烟
  豪杰
  木兰
  李玄邃
  内侍
  化及
  公谨
  樊建威
  罗士信
  万岁
  王世充
  安祖
  宇文述
  单全
  徐懋功
  齐国远
  欢喜
  如珪
  冶儿
  杨义臣
  光景
  杨国忠
  赵王
  刚才
  饮酒
  怀玉
  窦建德
  内监
  瓦岗
  果然
  嗣昌
  点头
  李如珪
  袁紫烟
  晋王
  杨素
  秦大哥
  婉儿
  尚未
  家眷
  恰好
  富贵
  幽州
  恐怕
  张果
  词曰
  薛冶儿
