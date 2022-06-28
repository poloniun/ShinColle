# 設定檔說明 (1.7.10版)
## desk 類

### I:Radar_Update
深海提督的辦公桌的更新間隔，預設128 ticks更新一次。


## general 類

### B:Always_Show_Team
設為true時，即使不手持ヲ級指揮權杖也會顯示隊伍圈圈標記的特效。

### I:Battle_Cooldown
艦隊創建，解散，宣戰的CD。

### I:Boss_Cooldown
艦娘艦隊生成CD，每次CD到有25%機率會生出一個艦隊。

### I:ChunkLoader_Mode
裝備深海羅盤後可開啟的chunk loader模式：
0 = 關閉此功能
1 = 只載入該艦所在chunk
2 = 載入該艦周圍3x3 chunks

### I:Close_GUI_Distance
船艦跑離多少格後會強制關閉船艦物品欄GUI。

### B:Debug_Mode
DEBUG模式，會顯示一些洗頻訊息，請不要開啟這個。

### S:DropRate_Grudge
怨念掉落率，設為0.5表示每兩隻怪會噴一顆，設為10表示一隻怪就會噴出10顆。

### B:Easy_Mode
簡單模式，大造資源獲得量x10倍，船艦使用物品獲得量約x3~5倍。

### B:Friendly_Fire
設為true時，範圍攻擊可以傷害到隊友玩家跟船艦。

### B:Polymetal_as_Mn
是否將多金屬礦登錄為錳礦，有錳礦的mod可能會用到。

### I:Recycle_Large
拆解大型艦娘回收資源量，注意大型艦娘拆出的是金屬方塊跟彈藥集裝箱。

### I:Recycle_Small
拆解小型艦娘回收資源量，注意小型艦娘拆出的是單顆金屬跟彈藥道具。

### B:Show_Name_Tag
是否在船艦頭上顯示名牌。

### B:Sound_Wakamoto
是否開啟棲艦坐騎的語音。

### I:Spawn_Boss_Number
每次野生艦隊生成時，BOSS艦娘生成數量。

### I:Spawn_Mob_Number
每次野生艦隊生成時，小型艦娘生成數量。

### B:Static_Mode
超深海熱漩是否以static模式繪製 (可無限距離顯示該entity)，如果有裝NEI此選項要關閉。

### I:VolcanoCore_Grudge
深海火山核心中每顆怨念可轉換的燃料值。


## ship setting 類

### I:Ammo_Ship
彈藥基本消耗量，每一行設定一個值，依序為：DD驅逐 CL輕巡 CA重巡 CAV航巡 CLT雷巡 CVL輕母 CV航母 BB戰艦 BBV航戰 SS潛艇 AP運輸。

### I:Attack_Base_Speed
各種攻擊的基本延遲時間，依序為近戰、輕攻擊、重攻擊、輕空軍、重空軍。
實際攻擊延遲計算為：基本時間 / 船艦攻速 + 固定時間

### I:Attack_Fixed_Delay
各種攻擊的固定延遲時間。

### S:Attack_Volume 攻擊音效
### S:Ship_Volume 船艦語音
### S:Timekeeping_Volume 報時語音
音量大小設定。

### I:BaseMorale_Caress
撫摸時心情上升基本值。

### B:Can_Flare
是否開啟照明彈功能。

### B:Can_Searchlight
是否開啟探照燈功能。

### B:Timekeeping
是否開啟報時語音。

### B:Check_Ring
小型野生艦娘生成時是否檢查玩家是否攜帶結婚戒指，預設開啟以避免太早碰到艦娘被秒。

### I:Custom_Sound_Rate
### I:Custom_Sound_Rate2
自訂船艦語音設定，每個船艦需要10個值，依序為：船艦ID、閒置、攻擊、受傷、死亡、結婚、擊退玩家、拾取物品、餵食、報時語音，船艦ID可參考該艦生怪蛋的meta值。
每個值代表該語音出現機率，設為0表示只用通用語音，100表示只使用自訂語音。
語音檔設置說明請參考mod中assets\shincolle下的CustomSoundReadme檔內容。

注意玩家自行新增的語音請寫在I:Custom_Sound_Rate
### I:Custom_Sound_Rate2在版本更新時有可能會被我改回預設值，這邊是放我自訂的語音，
可以把它的各項機率值都改成0來停用它。

### I:EXP_Modifier
升級經驗基本倍率，計算方式為：(等級 + 1) * 基本倍率

### I:Exp_Gain
船艦各個動作可獲得的經驗設定，依序為近戰、輕攻擊、重攻擊、輕空軍、重空軍、移動(每格，限運輸艦)、其他動作(拾取、補給等)

### I:Grudge_Action
船艦各動作消耗的怨念量設定，依序為近戰、輕攻擊、重攻擊、輕空軍、重空軍、移動(每2格)

### I:Grudge_Ship
各艦種怨念基本消耗量設定。

### D:LargeBoss_scale
### D:SmallBoss_scale
### D:LargeMob_scale
### D:SmallMob_scale
大小野生艦娘基本數值設定，實際數值還會依照各艦特性上下變動約20%。

### I:Mob_Spawn
小型野生艦娘生成設定，依序為：每個世界中最大數量，生成率(各玩家分開計算)，每次生成多少群，每群最少隻數，每群最大隻數。

### I:SVS_DmgTaken
玩家互打時的船艦受傷的倍率設定，預設為100即完整100%傷害。

### I:Summon_DmgTaken
玩家互打時召喚類受傷的倍率設定。

### D:ship_scale
船艦六大屬性值倍率設定，依序為血量、傷害、防禦、攻速、跑速、射程。

### D:ship_limit_basic
船艦六大屬性上限值設定，設為-1表示沒有上限。

### D:ship_limit_effect
船艦次要屬性上限值設定，設為-1表示沒有上限。依序為暴擊、二連、三連、降低失誤率、對空值、對潛值、閃避率。

### I:ship_teleport
船艦跟隨或者守衛，離目標太遠時傳送到目標旁邊的參數，值為：傳送發動間隔 (ticks)、判定該傳送的最短距離 (方塊數的平方)


## world gen 類

### I:Polymetal_Gravel
每個chunk中可生成的多金屬礫石群數。

### B:Polymetal_Gravel_Replace
可在那些方塊中生成多金屬礫石，依序為石頭、礫石、沙子、泥土。
某些海底方塊類型不同，可在此調整設定。

### I:Polymetal_Ore
多金屬礫石每個chunk生成群數。


## inter-mod 類

### B:Enable_Forestry
是否啟用Forestry支援，需安裝Forestry mod
預設true會新增一些Forestry的蜜蜂。


# 設定檔說明 (1.10.2版)

設定檔增加為三個: shincolle.cfg (主要) loottable.cfg (自訂寶箱內容) sounds.cfg (自訂音效)

## shincolle.cfg 新增：

### I:Command_ShipNum
使用指令/ship list時每一頁最多可列出的船艦個數

### I:Despawn_Boss
### I:Despawn_Minion
野外boss跟小怪船出生後，隔多少tick會判定為可刪除消失
距離超過100格就會被刪除，設為-1可以永久存在

### D:Tile_VolCore
### D:Tile_LargeShipyard
### D:Tile_SmallShipyard
依序為深海火山核心，超深海熱漩，深海熱泉方塊的設定
值依序為最大燃料存量，燃料消耗速度，每個燃料物品可增加燃料數

每個燃料物品可增加燃料數設定差異:
Tile_VolCore設定的值為"每顆怨念"可提供的燃料值，預設為240
Tile_Small跟LargeShipyard設定的值為每個燃料的燃料值"乘上的倍率"，預設為1.0
各個物品的燃料值則完全跟官方設定的燃料值相同，例如煤炭為1600，岩漿為2萬

### I:Tile_Crane
起重機內建暫存大小設定，依序為液體(mB)，IC2的EU暫存

### D:Attrs_Hostile_LargeBoss
### D:Attrs_Hostile_LargeMob
### D:Attrs_Hostile_SmallBoss
### D:Attrs_Hostile_SmallMob
依序大小等級4,3,2,1的野生艦娘數值設定
值依序為血量，傷害，防禦，攻速，跑速，射程
實際數值還會依照各艦娘特性增減，最多+20%
注意防禦不要設超過83，會導致戰艦變成防禦破百無敵

### D:Attrs_Limit
船艦屬性上限設定，設為-1表示無限制
依序為血量/輕攻擊/重攻擊/空軍輕攻擊/空軍重攻擊/防禦/攻速/移速/射程/爆擊/二連/三連/降失誤率/制空/反潛/閃避/經驗增加/彈藥增加/血量回復增加/擊退抵抗

### I:Attrs_Limit_Modernization
近代化改修等級上限設定，預設為3等

### D:Attrs_Scale
船艦六大屬性值倍率設定，依序為血量、傷害、防禦、攻速、跑速、射程。

### D:Held_Item
船艦顯示手持物品的大小設定，值依序為：放大倍率，X位移，Y位移，Z位移

### I:Death_Time
船艦死亡後屍體燃燒時間，燃燒時間跑完才會產生掉落物
預設為400 = 燃燒20秒

### I:CD_SearchLight
更新探照燈的cd時間，預設為4，表示每4 ticks偵測一次亮度並判斷要不要放探照燈。

### I:Infinite_Pump
船艦可以無限抽水或者岩漿的深度
若船艦腳底下的液體超過設定的深度，則抽液體時可以無限抽不會消滅液體方塊
只有水跟岩漿可以設定，液體的寬度也必須達到3x3大小才能無限抽

### I:Ring_Ability
結婚戒指能力設定，-1表示關閉，0以上則為結婚數量設定
結婚數量達到設定值就會開啟該能力
能力依序為：水中呼吸，水中移動，水中挖掘，水中視野，免疫火焰

其中挖掘跟視野的設定是最大值設定，這兩項能力是只要結婚數大於0就有效果
但是效果強度會根據結婚數變化

### I:Drum_EU
深海起重機的EU傳輸速度設定，值依序為：基本值，附魔加成值
總傳輸速度為：(船艦等級 * 0.1 + 1) * (基本值 * 變壓器裝備數量 + 附魔加成值 * 附魔總個數)

### I:Drum_Liquid
深海起重機的液體傳輸速度設定，值依序為：基本值，附魔加成值
總傳輸速度為：(船艦等級 * 0.1 + 1) * (基本值 * 抽水機裝備數量 + 附魔加成值 * 附魔總個數)

### B:Can_Teleport
船艦離守衛點或者主人太遠是否可以傳送過去。
若船艦經常在傳送後就莫名消失，就需要設為false以關閉該功能。

### I:Consume_Ammo
船艦攻擊時彈藥消耗基礎量，依序為驅逐/輕巡/重巡/航巡/雷巡/航母/戰艦/航戰/潛艇/輸送或特殊艦

### I:Consume_Grudge_Action
船艦各個動作的消耗怨念基礎量，依序為輕攻擊/重攻擊/輕航空攻擊/重航空攻擊/移動

### I:Consume_Grudge_Idle
船艦閒置時怨念消耗基礎量，依序為驅逐/輕巡/重巡/航巡/雷巡/航母/戰艦/航戰/潛艇/輸送或特殊艦

### I:Limit_MobSpawnNumber
野生船艦設定，數值為：最大數量/生成機率(0~100)/每次生成群數/每群最小船數/每群最大船數

### B:Attack_Player
野生船艦是否可以主動攻擊玩家

### B:Depth_HadalVortex
繪製超深海熱旋的漩渦時是否要開啟景深，會影響跟透明方塊類，如水跟冰的互蓋。

### I:Consume_Grudge_Task
工作中消耗的怨念量，依序為煮飯、釣魚、採礦、合成。

### I:Exp_Gain_Task
工作完成獲得的經驗量，依序為煮飯、釣魚、採礦、合成。

### B:Task_Enable
設定船艦是否可以進行該工作，依序為煮飯、釣魚、採礦、合成。

### I:Tick_Fishing
設定釣魚工作的花費時間，依序為基礎時間、隨機時間。
實際花費時間 = 基礎時間 + (0 ~ 隨機時間)

### I:Tick_Mining
設定挖礦工作的花費時間，依序為基礎時間、隨機時間。
實際花費時間 = 基礎時間 + (0 ~ 隨機時間)


## loottable.cfg 新增：
寶箱內容物設定，每一行設定一個物品，每行的每個數值用逗號隔開，不要加空格

格式：
箱子ID, 物品名稱, 物品meta值, weight, chance, 最小個數, 最大個數

箱子ID：
0:初始寶箱, 1:雪屋, 2:地牢, 3:村莊鐵匠箱, 4:廢礦坑,
5:金字塔, 6:叢林神殿, 7:地獄堡壘, 8:終界門地城, 9:終界城市

物品meta值若設為-1則為隨機設定，只有本mod的物品有隨機meta的功能

rolls數值固定為：隨機 1 ~ 該箱子生成物總數的一半+1
bonus_rolls固定為 1

這邊roll, weight, chance請參照 wiki的loot table說明
物品名稱可用遊戲中的/give指令查看或者裝JEI看
物品meta值可以在遊戲中按F3+H顯示

範例：
在廢礦坑箱子增加艦砲裝備，艦砲種類隨機，weight為8，chance 100%，最少1個，最多1個
4,shincolle:EquipCannon,-1,8,100,1,1


## sounds.cfg 新增：
自訂個船艦音效，每行為一個船艦設定，每個數值為該狀態下有多少機率使用自訂音效
0表示使用預設音效，100表示只使用自訂音效

格式：
船艦ID, 發呆, 攻擊, 受傷, 死亡, 結婚跟結婚發呆, 擊退, 拾取, 餵食, 報時
船艦ID等同生怪蛋的meta值
物品meta值可以在遊戲中按F3+H顯示

音效新增步驟：
1. 放置音效.ogg檔到mod jar檔中的assets/shincolle/sounds資料夾
2. 在sounds.cfg設定檔中新增各音效機率值
3. 在mod jar檔中的assets/shincolle/sounds.json檔中新增音效設定

sounds.json 範例：
船艦ID 56, 受傷音效, 音效檔名為 hurt5601.ogg, hurt5602.ogg, hurt5603.ogg

"ship-hurt-56": { "sounds": [
"shincolle:hurt5601",
"shincolle:hurt5602",
"shincolle:hurt5603"
]},   <--注意還有下一項時必須加逗號，沒有下一項就不要加逗號

實際sounds.json格式參考wiki的sounds.json


## mining.cfg 新增：
自動挖礦的產物設定，每一行設定一個物品，每行的每個數值用逗號隔開，不要加空格

格式：
世界ID, 生態系ID, 物品名稱, 物品meta值, 權重, 最小個數, 最大個數, 船艦等級, 高度, 工具等級, 附魔權重

世界ID: 設為999999表示為所有世界通用設定，否則為指定世界
生態系ID: 設為-999999表示全生態系通用設定，否則為指定生態系
物品名稱: 可以在遊戲中以/give指令查看或者裝JEI看
物品meta值: 若設為-1則為隨機設定，只有本mod的物品有隨機meta的功能
權重: 出現比重，實際出現率 = 本物品權重 / 可出現的全部物品權重總合
船艦等級: 要多少等級以上的船艦才能挖到此物品
高度: 要多少高度以下的位置才能挖到此物品
工具等級: 要手持多少等級以上的工具才能挖到此物品，0為木/金、1為石頭、2為鐵、3為鑽
附魔權重: 設定是否接受挖礦鎬上的財富加成，實際挖出量 = 原挖出量 * (1 + (附魔權重 / 100) * 財富等級)
