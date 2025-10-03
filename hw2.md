```mermaid
gantt
    title 圖3-27 甘特圖
    dateFormat  YYYY-MM-DD
    axisFormat  %Y-%m-%d

    section 任務
    T1 研擬計畫          :active, t1, 2025-09-30, 1d
    T2 任務分配          :active, t2, after t1, 4d
    T3 取得硬體          :active, t3, after t1, 17d
    T4 程式開發          :active, t4, after t2, 70d
    T5 安裝硬體          :active, t5, after t3, 10d
    T6 程式測試          :active, t6, after t4, 30d
    T7 撰寫使用手冊      :active, t7, after t5, 25d
    T8 轉換檔案          :active, t8, after t5, 20d
    T9 系統測試          :active, t9, after t6, 25d
    T10 使用者訓練       :active, t10, after t7, 20d
    T11 使用者測試       :active, t11, after t9, 25d

```

```mermaid
---
title: 圖3-27 PERT圖
---
flowchart LR
    node1["研擬計畫<br/>編號:1<br/>開始:第1天<br/>結束:第1天<br/>需時:1天"]
    node2["任務分配<br/>編號:2<br/>開始:第2天<br/>結束:第5天<br/>需時:4天"]
    node3["取得硬體<br/>編號:3<br/>開始:第2天<br/>結束:第18天<br/>需時:17天"]
    node4["程式開發<br/>編號:4<br/>開始:第6天<br/>結束:第75天<br/>需時:70天"]
    node5["安裝硬體<br/>編號:5<br/>開始:第19天<br/>結束:第28天<br/>需時:10天"]
    node6["程式測試<br/>編號:6<br/>開始:第76天<br/>結束:第105天<br/>需時:30天"]
    node7["撰寫使用手冊<br/>編號:7<br/>開始:第29天<br/>結束:第53天<br/>需時:25天"]
    node8["轉換檔案<br/>編號:8<br/>開始:第29天<br/>結束:第48天<br/>需時:20天"]
    node9["系統測試<br/>編號:9<br/>開始:第106天<br/>結束:第130天<br/>需時:25天"]
    node10["使用者訓練<br/>編號:10<br/>開始:第54天<br/>結束:第73天<br/>需時:20天"]
    node11["使用者測試<br/>編號:11<br/>開始:第131天<br/>結束:第155天<br/>需時:25天"]

    node1 --> node2
    node1 --> node3
    node2 --> node4
    node3 --> node5
    node4 --> node6
    node5 --> node7
    node5 --> node8
    node6 --> node9
    node7 --> node10
    node8 --> node10
    node9 --> node11
    node10 --> node11

```

### 關鍵路徑: 1->2->4->6->9->11
