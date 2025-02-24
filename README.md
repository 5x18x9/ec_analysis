---
# ECサイト分析プロジェクト

目次
- [プロジェクトの背景](#プロジェクトの背景)
- [データセット](#データセット)
   - [ERD](#ERD)
   - [データの前提条件](#データの前提条件)
- [分析](#分析)
   - [サマリー](#サマリー)
   -  [訪問数・流入動向](#訪問数・流入動向)
   -   [ユーザー](#ユーザー)
   -   [売上動向](#売上動向)
- [改善施策](#改善施策)
- [注意事項](#注意事項)


## プロジェクトの背景
このサービスは2019年にローンチしたグローバルEコマースサイトで、大人向けの男女のアパレル商品を販売しています。本プロジェクトの目的は、ECサイトの成長戦略を策定するために、売上・集客・ユーザー行動のデータを分析し、改善施策を提案することです。

## データセット
### ERD
本データセットは７つのテーブルで構成されています。本部分析ではユーザー情報、購入情報に関連した5つのテーブルを使用しました。
<img width="1263" alt="image" src="https://github.com/user-attachments/assets/1a92f77d-d1d0-4e39-8b14-ced33fd5c2df" />

### データの前提条件
本データセットは、テストや分析を目的として公開されているデータを使用しているため、実際のデータと異なっている点があります。
例）
- 商品別の利益率の差異がない
- 季節変動がない
- CVRが高い
- チャネル別のパフォーマンスに差異がみられない

上記を踏まえた上で、数値の違和感を最小にするため2022年までのデータを対象とし、以下の観点で得られる示唆をまとめました。
- 売上成長の要因分析
- トラフィック分析
- リピート率、休眠率などの顧客行動分析

## 分析
### サマリー
2019年のローンチから売上は右肩上がりで推移し、2022年の売上は107万ドルに到達、YoY56%と順調に規模を拡大しています。特に新規ユーザーの獲得は好調で、購入CVRは11%、前年比+57%と大幅に改善しています。しかし、新規購入率および休眠ユーザー率は徐々に低下しているものの、直近ではいずれも86%と高水準です。また、購入頻度は前年と同水準の1.1回にとどまり、新規ユーザーのリピーターへの成長が課題となっています。
売上の増加は購入ユーザー数と取引回数の増加によるものですが、今後の施策として、新規獲得の最適化に加え、リピーター育成と休眠ユーザーのアクティブ化を重点的に進める必要があります。

### 訪問数・流入動向
 - 訪問数は11万でYoY+3.8％
 - 新規登録トラフィックの70%がPaid search経由、セッションの45%がEmail経由
 - 新規登録から90日以内に購入したユーザーの割合が約9%、YoY+27％
 - セッションCVRが23%でYoY+43%と大幅に改善
 - 
![Image](https://private-user-images.githubusercontent.com/191242577/415471293-96c5f75d-9eec-452c-ba1e-deda6c040a0d.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDAxMDcyOTQsIm5iZiI6MTc0MDEwNjk5NCwicGF0aCI6Ii8xOTEyNDI1NzcvNDE1NDcxMjkzLTk2YzVmNzVkLTllZWMtNDUyYy1iYTFlLWRlZGE2YzA0MGEwZC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwMjIxJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDIyMVQwMzAzMTRaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT00NmVlNjQ4ZWUzYjM4OTNhYzI4OTFkMDRlZjlkNmExNjcyMjI0ZmY2MzY4YzhjNDg1ZmVkYThlNWJiYTkyN2M4JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.H5JmBMqphHgsht7yUaNDKsyyKS9i3ep8KZEKiSt9pW8)

### ユーザー
 - 購入ユーザー数は着実に伸びており、2022年の購入ユーザーは1万人を超え成長率はYoY60％
 - 初回購入の割合は年約-5％程度のペースで減少しており、直近では86％
 - 休眠ユーザーの割合も徐々に減少しているが、直近で86%と高水準
 - 購入頻度は、昨年と同水準の1.1回に留まっている

![Image](https://private-user-images.githubusercontent.com/191242577/415025477-973171dd-a8f6-4ae8-a5a3-3684a8797b12.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDAwMjg5MTgsIm5iZiI6MTc0MDAyODYxOCwicGF0aCI6Ii8xOTEyNDI1NzcvNDE1MDI1NDc3LTk3MzE3MWRkLWE4ZjYtNGFlOC1hNWEzLTM2ODRhODc5N2IxMi5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwMjIwJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDIyMFQwNTE2NThaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1mOTIzMzZhOTliNzM5Njg2NDZiNjMwN2E2MDM2ZTI3NzQ5MTZlYzVhZDMwNjRkMzhhOGZkZWVlODE0MzUzYTE5JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.xq2sPYSy-7uKGXwaUjqmnfWz00wHjUjzPELf_JR5qhU)


### 売上動向
 - 2019年から売上が急拡大し、2022年は107万ドルに到達、YoY56％と好調
 - 国別の売上は中国が37万ドル（34%）、とアメリカが25万ドル（22％）で全体の過半数を占める
 - 売上増加の主要要因は、購入ユーザー数と決済数の大幅な増加
 - 購入CVRは11%でYoY+57％

![Image](https://private-user-images.githubusercontent.com/191242577/415507669-5f5de8c9-d394-4c11-a5ad-9f67dedef874.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDAxMTU0MzYsIm5iZiI6MTc0MDExNTEzNiwicGF0aCI6Ii8xOTEyNDI1NzcvNDE1NTA3NjY5LTVmNWRlOGM5LWQzOTQtNGMxMS1hNWFkLTlmNjdkZWRlZjg3NC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwMjIxJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDIyMVQwNTE4NTZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1jNWYzNmI5ZTJmOTgzYjkxZTE5YzdmYzZjZmRjMjcxMWMxZDRiM2ViMjA5MDMxZWZhZjM4NjE4MDdjNWE4MjcyJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.B-ZPEt3Qo47MmzCp51XofXkKA1hq34Oq9A5WHZGiEAA)



## 改善施策
### リピート購入を強化
- SNS活用（有益な情報を発信し再訪・再購入に繋げる）
- 2回目の購入から使えるクーポンを配布（2回目の購入フック）
- 四半期に一度の特大セールを開催（定期的に訪問の動機を作る）

### Paid広告依存のリスクを軽減
- 広告の最適化（チャネル別のROASを分析し最適化）
- SNS活用（SNSの運用を強化）
- SEO強化（自然流入強化）

### 休眠ユーザーをアクティブ化
-ターゲティングメール配信（過去の購入履歴やお気に入り商品に基づいたパーソナライズドメール）
-リターゲティング広告（休眠ユーザーの再獲得）


 ## 注意事項
 - 未ログインユーザーのuser_idはセッションIDをユニークユーザーとしてカウントしています。
 - eventsテーブルのpurchaseイベントは商品ごとにpurchaseイベントが発火しているが、ordersテーブルで同じorder_idでも、eventsテーブルでsession_id, created_at, traffic_sourceが違うケースが多数存在している理由は不明です。
 - traffic_sourceのSearch,Organic,Adwordsの定義が明確ではないが、searchはPaid searchと仮定しています。
 - 直帰の定義は、1イベントのみのセッションを直帰としています。
