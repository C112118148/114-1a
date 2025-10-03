```mermaid
gantt
    title 甘特圖
    dateFormat  YYYY-MM-DD
    section Section
    研擬計畫     :a1, 2014-01-01, 1d
    任務分配     :a2,after a1 , 4d
    取得硬體     :a3,after a1  , 17d
    程式開發     :a4,after a2, 70d
    安裝硬體     :a5,after a3, 10d
    程式測試     :a6,after a4, 30d
    撰寫使用手冊     :a7,after a5, 25d
    轉換檔案     :a8,after a5, 20d
    系統測試     :a9,after a6, 25d
    使用者訓練     :a10,after a7 and a8, 20d
    使用者測試     :a11,after a9 and a10, 25d

```

```mermaid
flowchart TD
    A["研擬計畫<br>編號:1<br>所需時間: 1天"]
    B["任務分配<br>編號:2<br>所需時間: 4天"]
    C["取得硬體<br>編號:3<br>所需時間: 17天"]
    D["程式開發<br>編號:4<br>所需時間: 70天"]
    E["安裝硬體<br>編號:5<br>所需時間: 10天"]
    F["程式測試<br>編號:6<br>所需時間: 30天"]
    G["撰寫使用手冊<br>編號:7<br>所需時間: 25天"]
    H["轉換檔案<br>編號:8<br>所需時間: 20天"]
    I["系統測試<br>編號:9<br>所需時間: 25天"]
    J["使用者訓練<br>編號:10<br>所需時間: 20天"]
    K["使用者測試<br>編號:11<br>所需時間: 25天"]

    A --> B
    A --> C
    B --> D
    C --> E
    D --> F
    E --> G
    E --> H
    F --> I
    G --> J
    H --> J
    I --> K
    J --> K
```
## 關鍵路徑:1(研擬計畫)->2(任務分配)->4(程式開發)->6(程式測試)->9(系統測試)->11(使用者測試)
