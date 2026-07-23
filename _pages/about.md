---
permalink: /
title: "Academic Pages is a ready-to-fork GitHub Pages template for academic personal websites"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>家常菜谱大全</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: "Microsoft Yahei", sans-serif;
        }
        body {
            background-color: #f8f5f0;
            color: #333;
        }
        /* 头部导航 */
        header {
            background: #d63031;
            color: #fff;
            text-align: center;
            padding: 25px 0;
            box-shadow: 0 2px 8px rgba(0,0,0,0.15);
        }
        header h1 {
            font-size: 28px;
            letter-spacing: 2px;
        }
        header p {
            margin-top: 8px;
            opacity: 0.9;
        }

        /* 分类按钮区域 */
        .tab-box {
            width: 90%;
            max-width: 1000px;
            margin: 30px auto;
            display: flex;
            justify-content: center;
            gap: 20px;
        }
        .tab-btn {
            padding: 12px 36px;
            border: none;
            border-radius: 50px;
            font-size: 17px;
            cursor: pointer;
            background: #fff;
            border: 2px solid #d63031;
            color: #d63031;
            transition: all 0.3s ease;
        }
        .tab-btn.active {
            background: #d63031;
            color: white;
        }
        .tab-btn:hover {
            transform: translateY(-2px);
        }

        /* 菜谱容器 */
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto 50px;
        }
        .food-list {
            display: none;
            grid-template-columns: repeat(auto-fill, minmax(340px, 1fr));
            gap: 30px;
        }
        .food-list.show {
            display: grid;
        }

        /* 菜品卡片样式 */
        .food-card {
            background: white;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 3px 12px rgba(0,0,0,0.08);
            transition: 0.3s;
        }
        .food-card:hover {
            transform: translateY(-6px);
            box-shadow: 0 8px 20px rgba(0,0,0,0.12);
        }
        .food-img {
            width: 100%;
            height: 220px;
            object-fit: cover;
        }
        .food-info {
            padding: 18px;
        }
        .food-name {
            font-size: 20px;
            color: #222;
            margin-bottom: 10px;
            font-weight: bold;
        }
        .title-line {
            color: #d63031;
            font-weight: bold;
            margin: 10px 0 4px;
        }
        .food-desc {
            line-height: 1.6;
            font-size: 14.5px;
            color: #555;
        }

        footer {
            text-align: center;
            padding: 20px;
            background: #222;
            color: #aaa;
            font-size: 14px;
        }
    </style>
</head>
<body>
    <header>
        <h1>家常美味菜谱</h1>
        <p>简单易学 | 居家下厨必备食谱</p>
    </header>

    <!-- 分类切换按钮 -->
    <div class="tab-box">
        <button class="tab-btn active" data-type="meat">肉菜专区</button>
        <button class="tab-btn" data-type="veg">素菜专区</button>
    </div>

    <div class="container">
        <!-- 肉菜列表 -->
        <div class="food-list show" id="meat">
            <!-- 红烧肉 -->
            <div class="food-card">
                <img class="food-img" src="https://img0.baidu.com/it/u=1240887212,3823211223&fm=253&fmt=auto&app=138&f=JPEG?w=800&h=500" alt="红烧肉">
                <div class="food-info">
                    <div class="food-name">经典红烧肉</div>
                    <div class="title-line">所需食材：</div>
                    <p class="food-desc">五花肉500g、冰糖、生姜、大葱、八角、生抽、老抽、料酒</p>
                    <div class="title-line">制作步骤：</div>
                    <p class="food-desc">1.五花肉切块冷水下锅焯水去血沫捞出洗净；<br>
                    2.锅中少油炒冰糖至枣红色，倒入肉块翻炒上色；<br>
                    3.加葱姜八角、料酒、生抽老抽翻炒，加开水没过肉块；<br>
                    4.小火慢炖40分钟，大火收汁即可出锅。</p>
                </div>
            </div>

            <!-- 可乐鸡翅 -->
            <div class="food-card">
                <img class="food-img" src="https://img2.baidu.com/it/u=278923210,2844213302&fm=253&fmt=auto&app=138&f=JPEG?w=800&h=500" alt="可乐鸡翅">
                <div class="food-info">
                    <div class="food-name">可乐鸡翅</div>
                    <div class="title-line">所需食材：</div>
                    <p class="food-desc">鸡翅中8个、可乐一罐、姜片、生抽、老抽、食盐</p>
                    <div class="title-line">制作步骤：</div>
                    <p class="food-desc">1.鸡翅两面划刀焯水沥干水分；<br>
                    2.平底锅少油煎至两面金黄，放入姜片爆香；<br>
                    3.倒入可乐、生抽、少许老抽，小火焖煮15分钟；<br>
                    4.开大火收浓汤汁，汤汁裹满鸡翅即可。</p>
                </div>
            </div>

            <!-- 鱼香肉丝 -->
            <div class="food-card">
                <img class="food-img" src="https://img1.baidu.com/it/u=3633022111,1781101123&fm=253&fmt=auto&app=120&f=JPEG?w=800&h=500" alt="鱼香肉丝">
                <div class="food-info">
                    <div class="food-name">鱼香肉丝</div>
                    <div class="title-line">所需食材：</div>
                    <p class="food-desc">猪里脊、木耳、胡萝卜、笋丝、泡椒、糖醋酱汁</p>
                    <div class="title-line">制作步骤：</div>
                    <p class="food-desc">1.肉丝腌制入味，配菜切丝焯水备用；<br>
                    2.泡椒蒜末炒出鱼香味，下入肉丝滑炒断生；<br>
                    3.放入全部配菜翻炒，淋入调好的鱼香芡汁翻炒均匀出锅。</p>
                </div>
            </div>
        </div>

        <!-- 素菜列表 -->
        <div class="food-list" id="veg">
            <!-- 蒜蓉油麦菜 -->
            <div class="food-card">
                <img class="food-img" src="https://img2.baidu.com/it/u=199663522,3299252121&fm=253&fmt=auto&app=138&f=JPEG?w=800&h=500" alt="蒜蓉油麦菜">
                <div class="food-info">
                    <div class="food-name">蒜蓉油麦菜</div>
                    <div class="title-line">所需食材：</div>
                    <p class="food-desc">油麦菜一把、大量大蒜、盐、蚝油、少许白糖</p>
                    <div class="title-line">制作步骤：</div>
                    <p class="food-desc">1.油麦菜洗净沥干，大蒜剁成蒜蓉；<br>
                    2.热油下入一半蒜蓉炸至微黄，放入油麦菜大火快炒；<br>
                    3.菜叶变软后加盐、蚝油、白糖调味；<br>
                    4.出锅前放入剩余生蒜蓉翻炒几秒即可。</p>
                </div>
            </div>

            <!-- 清炒土豆丝 -->
            <div class="food-card">
                <img class="food-img" src="https://img2.baidu.com/it/u=1297821131,3072923222&fm=253&fmt=auto&app=138&f=JPEG?w=800&h=500" alt="清炒土豆丝">
                <div class="food-info">
                    <div class="food-name">酸辣土豆丝</div>
                    <div class="title-line">所需食材：</div>
                    <p class="food-desc">土豆、青椒、干辣椒、米醋、食盐、蒜末</p>
                    <div class="title-line">制作步骤：</div>
                    <p class="food-desc">1.土豆切丝清水浸泡洗去淀粉，口感更脆爽；<br>
                    2.热油爆香干辣椒蒜末，下入土豆丝大火爆炒；<br>
                    3.沿锅边淋入米醋，加青椒丝、食盐翻炒一分钟立刻出锅。</p>
                </div>
            </div>

            <!-- 香菇青菜 -->
            <div class="food-card">
                <img class="food-img" src="https://img0.baidu.com/it/u=3329520080,1542003381&fm=253&fmt=auto&app=138&f=JPEG?w=800&h=500" alt="香菇青菜">
                <div class="food-info">
                    <div class="food-name">香菇扒青菜</div>
                    <div class="title-line">所需食材：</div>
                    <p class="food-desc">上海青、干香菇、生抽、淀粉、白糖、食用油</p>
                    <div class="title-line">制作步骤：</div>
                    <p class="food-desc">1.青菜焯水摆盘，泡发香菇切花刀；<br>
                    2.锅中煎香香菇，加入生抽、清水焖煮2分钟；<br>
                    3.水淀粉勾芡收汁，将香菇连同汤汁浇在青菜上完成。</p>
                </div>
            </div>
        </div>
    </div>

    <footer>
        家常菜谱网站 © 2026 仅供学习使用
    </footer>

    <script>
        // 获取按钮和菜谱盒子
        const btns = document.querySelectorAll('.tab-btn');
        const foodBox = document.querySelectorAll('.food-list');

        // 切换分类逻辑
        btns.forEach(btn => {
            btn.addEventListener('click', () => {
                // 清空所有激活样式
                btns.forEach(b => b.classList.remove('active'));
                foodBox.forEach(box => box.classList.remove('show'));
                // 当前按钮激活
                btn.classList.add('active');
                // 显示对应菜谱
                const type = btn.getAttribute('data-type');
                document.getElementById(type).classList.add('show');
            })
        })
    </script>
</body>
</html>
