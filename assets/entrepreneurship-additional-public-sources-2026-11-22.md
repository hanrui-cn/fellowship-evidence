# Entrepreneurship：新增公开来源核验与 Above 对照

核验日期：2026-11-22。本文只列本轮新取得、已打开核读且不在 `entrepreneurship-public-sources-2026-11-21.md` 主证据中的来源。结论先行：**有两组值得加入的新证据——2018年政府入库公告、2015年外部开发者实际集成案例；没有找到更强的融资、知名企业客户、收购交割或医疗成效新来源。**

## N1：2018年科技部火炬中心科技型中小企业入库公告

来源：

- [北京市2018年第三批入库科技型中小企业名单公告](http://www.chinatorch.gov.cn/zxqyfw/c101143/201805/dd56d216664f4e19aff4d223490f5429.shtml)，页面显示日期 **2018-05-18**。
- [公告附件PDF](http://www.chinatorch.gov.cn/zxqyfw/c101143/201805/dd56d216664f4e19aff4d223490f5429/files/e24f5bfe6738470190772f7301869b4a.pdf)，第229项。

附件原文：

> 229 北京乐塔克科技有限公司 201811010808005530

**来源性质：**政府官方原始公告及附件；独立于申请人和LearningTech，不是新闻稿或转载。公告页元数据含2021年的页面生成时间，但页面显示的公告日期为2018-05-18；本项采用页面显示的公告日期，不把2021生成时间当作入库日期。

**直接支持：**北京乐塔克在2018年第三批科技型中小企业入库名单中，入库登记编号为 `201811010808005530`。这是2018年的政府公开记录，也可作为政府体系内的正面公开认可。

**证明边界：**它不能只凭一张名单证明2013–2018每年持续经营，也不能证明韩锐当时的CEO任期、收入、融资或收购交割。它的最大价值是为既有“香港早期业务→北京→2018”链条增加一个**独立、有明确日期的2018年政府记录**。应写“列入科技型中小企业入库名单”，不写成竞争性奖项、政府资助或经营审计。

## N2：外部开发者在2015年实际集成RealTimeCat

### N2a：OneMoreFace团队的原始仓库及代码

来源：

- [ShanghaitechGeekPie/OneMoreFace仓库](https://github.com/ShanghaitechGeekPie/OneMoreFace)。
- [仓库元数据API](https://api.github.com/repos/ShanghaitechGeekPie/OneMoreFace)：`created_at` 为 **2015-10-24T07:03:35Z**，`pushed_at` 为2015-10-26。
- [团队README](https://raw.githubusercontent.com/ShanghaitechGeekPie/OneMoreFace/master/README.md)。
- [应用代码 `onemoreface.js`](https://raw.githubusercontent.com/ShanghaitechGeekPie/OneMoreFace/master/OneMoreFace/static/js/onemoreface.js)。
- [页面模板 `live.html`](https://raw.githubusercontent.com/ShanghaitechGeekPie/OneMoreFace/master/OneMoreFace/template/live.html)。

README原文：

> 该系统由计算机视觉库Clmtrackr结合实时猫的Webrtc API服务构建,以Django为服务框架。

代码不是只提到产品名，而是实际加载并调用SDK：

- `live.html` 加载 `js/realtimecat-0.1.min.js`；
- `onemoreface.js` 创建 `new RTCat.Stream(config)` 和 `new RTCat.Session(token)`；
- 随后调用 `session.connect()`、`session.publish(localStream)`、`session.subscribe(...)`，并处理远程流和消息。

**来源性质：**外部开发团队的一手原始技术记录；独立于LearningTech，不是新闻稿或转载。Git日期是开发者元数据，代码头另记2015-10-24/25。

**直接支持：**2015年一个上海科技大学学生团队在其24小时黑客马拉松项目中实际集成RealTimeCat WebRTC API及JavaScript SDK。它比npm下载计数更直接地证明了**外部开发者复用和具体应用集成**。

**证明边界：**代码及README证明集成，不单独证明长期生产部署、付费客户、独立用户数量或服务 uptime；也不是LearningTech获奖的证据。

### N2b：SegmentFault当时报道确认采用及杭州一等奖

来源：[SegmentFault 1024 Hackathon 优秀作品汇总](https://segmentfault.com/a/1190000003920404)，**2015-10-28**，SegmentFault思否。

原文：

> 「OneMoreFace」是本次大赛杭州一等奖，来自 Geek Pie 团队……

团队介绍引文：

> 本项目使用了 clmtrackr 项目和实时猫 WebRTC 大厅服务。

**来源性质：**独立技术社区/赛事方的当时编辑报道；采用性文字是团队自述，但由赛事方在获奖作品汇总中刊出，不是LearningTech新闻稿。

**直接支持：**同一外部团队的OneMoreFace获得杭州一等奖，且获奖作品介绍明确列出RealTimeCat服务。与N2a代码合读，可证明这不是只有下载而无实例的采用记录。

**证明边界：**奖项属于OneMoreFace团队，不属于LearningTech或韩锐；不可写成“RealTimeCat获得黑客马拉松一等奖”。

### N2c：上海科技大学官方独立 corroboration

来源：[热烈祝贺我校学生获得SegmentFault Hackathon杭州站第一名](https://life.shanghaitech.edu.cn/2015/1028/c2675a17965/page.htm)，**2015-10-28**，上海科技大学。

原文要点：Geek Pie团队的OneMoreFace从33个项目中脱颖而出获得第一名；五人团队经现场24小时开发，最终经过demo展示与答辩获奖。

**来源性质：**独立大学官方公告；不是LearningTech材料。**该文不点名RealTimeCat**，因此只用于核实团队、项目、开发过程和获奖，不单独证明SDK采用。

**组合价值：**N2a证明RealTimeCat集成，N2b由赛事方同时记载采用和获奖，N2c由大学独立核实项目及获奖。三者构成一条清楚的外部采用证据链，但不应算作三个互不相关的客户。

### N2d：团队成员本人公开复盘（补充，不重复计为另一客户）

来源：[情感机器人](https://mc.dfrobot.com.cn/article-351334.html)，**2015-11-14**，DF创客社区，作者 `erikxiong`（熊昭平）。

作者以第一人称说明自己参加SegmentFault Hackathon并凭OneMoreFace获杭州站第一名，随后写：

> 该系统由计算机视觉库Clmtrackr结合实时猫的Webrtc API服务构建,以Django为服务框架。

**来源性质：**外部团队成员的一手公开陈述；不是LearningTech新闻稿。与N2a/N2b是同一团队、同一项目，只作直接人证式补充，**不增加独立采用项目数**。

## Above rubric 对照

官方 Above 要求企业活跃超过五年、与IT/digital直接相关并惠及社会；须清楚说明创办人的领导、行业需求及设立过程；成功至少由显著利润、显著融资、知名企业客户或其他企业/慈善/政府机构的正面公开认可之一衡量。

| 维度 | 本轮新增证据的作用 | 结论及保留边界 |
|---|---|---|
| 活跃超过五年 | N1给出2018-05-18政府名单中的北京乐塔克；与既有早期业务、2014产品、2017经营和2018产品/承接记录组合 | **明显加强2018端点的独立性。**不能把N1单独写成五年证明，仍须保留既有香港到北京业务沿革 |
| 创办人领导及设立过程 | 本轮没有比铅笔道创始人采访、2014当时商业材料和既有公司记录更强的领导证据 | 沿用既有Action，不用OneMoreFace或政府名单替代创办人领导证据 |
| IT/digital及行业需求 | N2是2015年真实WebRTC SDK集成，直接对应数字产品和服务 | **R2 strongest addition**：由“下载量”推进到“外部团队实际构建应用” |
| 社会收益 | 本轮未取得新的独立远程医疗、患者结果、学校采用或临床证据 | 沿用既有教学使用规模及铅笔道远程医疗案例；不把OneMoreFace娱乐项目或N1入库名单冒充社会收益 |
| 正面公开认可 | N1是2018政府入库公告；既有2017国家高新技术企业证书仍是R1主证据 | N1可辅助政府公开认可，但应准确写“入库”，不是竞争性奖项 |
| 融资、知名客户、收购 | 本轮未取得可核验的更强新来源 | R3维持既有融资协议、兆尹材料及客户证据；2018精确交割日期仍未由新公开来源独立核实 |

**总体判断：**新增材料主要补强 Above 的**五年经营链条（N1）**和**实际开发者采用（N2）**，并使政府公开认可多一条官方记录。它们没有独立解决RMB 8.5M到账、China General Technology Group/Motorola Solutions付费交付、2018收购交割月份或医疗结果；这些方面不应因本轮检索而扩大表述。

## 建议的精简 Action / R1–R3 证据结构

### Action — Business record

1. **Founding, leadership and operation**：保留现有36氪/铅笔道、2014当时材料及2017–2018产品记录；在该项加入 **N1政府2018入库公告**。一句话证明作用：官方名单在2018-05-18列北京乐塔克及入库编号，为五年经营链提供独立的2018政府端点。
2. **Product commercialisation and exit**：保留现有SDK/私有云/公有云、百家云发布、后续收购报道及承接材料。本轮无需新增项。

### R1 — National recognition

- 以既有 **2017 National High-Tech Enterprise证书GR201711003470** 为主证据，继续配既有全国认定制度说明。
- **N1只在Action出现一次即可**；若页面确需第二条R1，可作交叉引用，不重复建立同一证据卡，不将其包装成奖项。

### R2 — Developer adoption

1. 保留现有npm首发、MIT许可、下载区间及约600家注册开发机构，继续注明下载不等于去重用户或付费客户。
2. 新增一张 **“Independent developer integration, 2015”** 证据卡：主链接用N2a仓库/代码，配N2b SegmentFault报道；N2c大学公告作交叉核验，N2d可不占首层。证明作用：外部学生团队在24小时项目中实际调用RealTimeCat SDK，并凭该应用获杭州一等奖；明确奖项属于该团队。

### R3 — Commercial success

- 保留现有兆尹2017材料、融资协议及知名企业客户证据和教学使用规模。**本轮没有足够强的新公开来源建议加入R3。**

## 未采用来源及检索结论

- 找到一篇署“猎云网／周丽梅、10月21日”的《实时猫：专注于WebRTC技术的实时云视频技术服务商》全文，文中称实时猫与中国联通合作；但本轮实际可打开的仅是[无关游戏聚合域名上的转载页](https://www.68371556.com/41529490cc451078/22c56653ab49a176.html)。原猎云正文或可靠存档未恢复，故**不把该转载页列为成品证据，也不据它新增“中国联通为客户/合作伙伴”**。这与既有来源说明中“猎云正文未取得”的限制一致。
- 公开检索出现实时猫官网、博客、演示站及更多公司目录，但当前官网跳转域名停放页，博客/演示站未能稳定打开正文；已有GitHub、Wayback和npm原始记录更直接，未以搜索摘要补写新事实。
- 未找到可核读的新融资完成公告、General Technology/Motorola/Hitachi/Huawei客户方记录、独立医疗使用调查或确认2018精确收购交割的新公告。转载铅笔道、重复商业计划书目录和串项数据库均未计入新证据。
