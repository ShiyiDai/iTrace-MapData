# iTrace 地图数据

本仓库用于准备 iTrace 的地图数据分发材料，当前保持私有。数据包保存于草稿 Release，未作为公开下载服务提供。

## 当前状态

当前包包含 App 使用的完整行政边界、地区目录、来源说明和显示瓦片。它是融合数据，不是仅含 OSM 的数据集。天地图对于离线分发和 ODbL 相容共享的授权仍待确认；不能将整个包视为已经取得 ODbL 授权。

本仓库不包含用户照片、个人足迹、账号凭据或 App 业务源码。内部来源记录中的授权状态按原样保留，不代表新的法律结论。

## 数据包与核验

草稿版本：`review-2026-09-15`。附件 `map-database-review.zip` 是机器可读本地审阅包。版本、来源、文件清单和 SHA-256 见 [版本记录](versions/2026-09-15-review.json)。下载后可使用 `shasum -a 256 map-database-review.zip` 核对压缩包哈希。未来 App 数据更新时必须同步生成新包，不能拿旧包对应新版本。

## 来源与许可

- 部分地图数据 © OpenStreetMap contributors，依据 [ODbL 1.0](https://opendatacommons.org/licenses/odbl/1-0/) 提供；[离线许可全文](licenses/ODbL-1.0.txt)。
- 天地图公众版基础地理信息数据：引自天地图，https://www.tianditu.gov.cn/ 。融合与分发条件待确认。
- 台湾县市界线：内政部国土测绘中心，2020，縣市界線（TWD97經緯度），COUNTY_MOI_1090820；依据[政府资料开放授权条款第1版](https://data.gov.tw/license)提供，遵守条款即可使用。
- 香港区界：香港政府民政事务总署、DATA.GOV.HK；适用 [DATA.GOV.HK 使用条款](https://data.gov.hk/en/terms-and-conditions)。

以上按来源说明权利，不对第三方内容作统一授权承诺。当前不设置覆盖整个仓库的开源许可证。

## 转公开前

1. 确认天地图等新增内容允许离线分发及按 ODbL 相容条件共享。
2. 复核完整数据库、许可声明和当前 App 的对应关系。
3. 确认面向公众的署名方式、地图审核及既有发布要求。
4. 经仓库所有者确认后再修改可见性、发布 Release，并将实际数据下载入口接入 App。

私有仓库和草稿 Release 不等于已经履行对公众提供衍生数据库的义务。不会自动切换为公开。
