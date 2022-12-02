# TDengineGUI

本人看到原仓库不在进行维护，所以本地打算将项目维护起来。本人正在对代码进行重构，正在快马加鞭优化中。希望您留下您的Star,您的Star将是我的动力。感谢~

温馨提示：源码正在重构，下载源码版本可能不能正常运行下载请下载release版进行使用[wwtbnbwv1.0.0](https://gitee.com/wwtbnbw6688/tdengine-gui3/releases/download/v1.0.0/WWTBNBW%20Setup%201.0.0.exe)

TDengineGUI是一个基于electron构建的，针对时序数据库TDengine的图形化管理工具。具有跨平台、易于使用、版本适应性强等特点。

QQ群号：628594380

##  重构版本界面预览
![输入图片说明](_img/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20221123134631.png)
![输入图片说明](_img/QQ%E6%88%AA%E5%9B%BE20221120194806.png)
![输入图片说明](_img/%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20221123104032.png)
![输入图片说明](_img/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20221123104010.png)
![输入图片说明](_img/%E8%AF%A6%E7%BB%86%E6%95%B0%E6%8D%AE.png)
![输入图片说明](_img/%E6%95%B0%E6%8D%AE%E8%A1%A8%E6%B7%BB%E5%8A%A0.jpg)
![输入图片说明](_img/%E6%95%B0%E6%8D%AE%E8%A1%A8%E6%B7%BB%E5%8A%A02.jpg)
![输入图片说明](_img/%E5%BA%93%E8%AF%A6%E6%83%85%E9%A1%B5%E9%9D%A2.png)
##  请作者喝一杯咖啡吧【自愿备注下您的昵称或方式.我必将铭记于心】
![image](https://user-images.githubusercontent.com/53170533/205204117-0dfee60b-8e61-4f0a-b7e6-7f21622f339d.png)

##  以下是原版描述-当前版本功能

- 通过TDengine restful接口连接到数据库，使用基本不受服务器版本升级影响
- 数据库添加删除操作，显示数据库属性
- 显示数据库中超级表和表信息，删除超级表与表功能
- 显示超级表和表数据功能，提供分页、时间段检索、字段过滤、排序等功能

## 如何获取

### 下载最新版可执行文件【源码正在重构可能不能正常运行下载release版进行使用】：

[wwtbnbw](https://gitee.com/wwtbnbw6688/tdengine-gui3/releases/download/v1.0.0/WWTBNBW%20Setup%201.0.0.exe)

### 通过源代码运行开发版本【源码正在重构目前不建议这种方式运行】：

- 克隆项目: git clone https://gitee.com/wwtbnbw6688/tdengine-gui3.git
- 安装依赖: npm install
- 启动开发版本: npm run start
- 生成桌面应用（可选）: npm run build （生成在dist文件夹下）

## 使用说明

打开软件后，界面左侧会显示需要管理的数据库服务器列表和服务器中数据库列表，同时显示数据库服务器的版本号。

![输入图片说明](https://images.gitee.com/uploads/images/2021/0225/195233_ae0bed6a_1803713.png "1.png")

可以通过“新建连接”按钮，添加新的服务器进行管理。需要提供数据库服务器的ip地址、restful服务的端口号（默认为6041）、连接服务器的用户名和密码（默认为root:taosdata）

![输入图片说明](https://images.gitee.com/uploads/images/2021/0225/195337_004fcbab_1803713.png "2.png")

可以通过点击数据库后的删除图标，进行删除数据库操作。

![输入图片说明](https://images.gitee.com/uploads/images/2021/0225/195350_4ee1db20_1803713.png "3.png")

可以通过点击添加数据库图标，进行添加数据库操作。可以在添加时选择数据库属性(具体属性含义请参考[tdengine官方文档](https://www.taosdata.com/cn/documentation/taos-sql#management))

![输入图片说明](https://images.gitee.com/uploads/images/2021/0225/195404_7f1d3906_1803713.png "5.png")

可以通过点击服务器连接后的删除图标，进行删除数据库连接操作。

![输入图片说明](https://images.gitee.com/uploads/images/2021/0225/195416_5a61f8b1_1803713.png "6.png")

选择要操作的数据库后，即可进入当前数据库操作界面。可以通过点击“切换”按钮调出数据库导航栏，切换要操作的数据库。当前数据库操作界面中分 超级表、表、控制台、数据库属性四个标签页。每个标签页都针对当前数据库进行显示与操作。

![输入图片说明](https://images.gitee.com/uploads/images/2021/0225/195429_aaa36a97_1803713.png "7.png")

超级表（表）标签页中，左侧为超级表（表）的列表，可以进行删除与检索操作（添加、修改等操作后续版本将提供，当前版本如需增加数据表或者插入数据请使用控制台输入命令完成）。左侧则显示当前数据表的数据。

![输入图片说明](https://images.gitee.com/uploads/images/2021/0225/195442_158e0dec_1803713.png "8.png")

![输入图片说明](https://images.gitee.com/uploads/images/2021/0225/195455_4c28d96d_1803713.png "11.png")

可以对表数据进行时间段选择。

![输入图片说明](https://images.gitee.com/uploads/images/2021/0225/195506_e06709c4_1803713.png "9.png")

可以对表数据进行时间字段过滤、排序、分页等操作。

![输入图片说明](https://images.gitee.com/uploads/images/2021/0225/195519_ec81d271_1803713.png "10.png")


控制台中可以输入sql命令运行，并显示restful接口原始返回结果。控制台中输入的命令默认针对当前数据库进行操作，一般情况下不需要在表名称前附加数据库名称。但也可以通过“数据库名.表名”的方式操作其他数据库中的表。（结果显示方式，以后版本将改进）

![输入图片说明](https://images.gitee.com/uploads/images/2021/0225/195530_5c5e66d8_1803713.png "12.png")

数据库属性显示当前数据库的一些基础属性，后期版本将加入属性修改功能。

![输入图片说明](https://images.gitee.com/uploads/images/2021/0225/195541_ca8b8767_1803713.png "14.png")


后期版本待完成功能:
- [ ] 创建超级表（表）功能
- [ ] 修改超级表（表）的表结构
- [ ] 子表与独立表的显示风格区分
- [ ] 完善数据库属性页（修改数据库属性、用户管理等）
- [ ] 超级表标签管理，以及子表的标签配置
- [ ] 按照字段类型检索数据(高级检索功能)
- [ ] 选择数值类型字段进行柱状图，折线图等图表的方式显示数据趋势
- [ ] 显示数据统计量（求和，平均，方差等）
- [ ] 批量插入测试数据功能
- [ ] 数据备份与数据导出功能
- [ ] 修改连接配置信息功能
- [ ] 连接配置信息导出导入功能
- [ ] 基础属性配置功能（连接超时时间、默认每页大小等）
