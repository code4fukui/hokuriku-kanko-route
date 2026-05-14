# hokuriku-kanko-route

このプロジェクトは、日本の北陸地方における観光客の移動や混雑状況をインタラクティブに可視化するものです。金沢大学が収集し、北陸インバウンド観光DX・データコンソーシアムが公開しているWi-Fiパケットセンシングのオープンデータを活用しています。生データを加工したものは、[code4fukui/mac-address](https://github.com/code4fukui/mac-address) リポジトリで提供されています。

## デモ

-   **[北陸観光移動軌跡](https://code4fukui.github.io/hokuriku-kanko-route/)**
    
    訪問者の流れを可視化したインタラクティブな地図です。各地点は訪問者数に応じたサイズの円で示されます。特定の地点を選択すると、そこを起点とする人気のルート（青線）や、個別の匿名ユーザーの移動軌跡（緑線）を確認できます。

-   **[北陸観光Wi-Fiパケットセンシングによる時間帯別混雑状況目安](https://code4fukui.github.io/hokuriku-kanko-route/traffic.html)**
    
    訪問者数を比較するための折れ線グラフです。最大4つの観光施設を選択し、時間帯別の混雑状況を可視化して比較できます。

## 特徴

-   **移動軌跡マップ:** 観光スポット間の人気ルートを可視化し、個別の匿名訪問者の経路を表示します。
-   **混雑状況チャート:** ユーザーが選択した複数の地点における、時間帯別の訪問者数の推移を比較します。
-   **インタラクティブなインターフェース:** 地点や個別ユーザーでデータを絞り込み、移動パターンを探索できます。
-   **クライアントサイド動作:** サーバー側のセットアップは不要で、すべてブラウザ上で動作します。

## 使い方

### ライブデモの利用

このツールを最も簡単に利用する方法は、上記のリンクからライブデモにアクセスすることです。

### ローカルでの実行

1.  リポジトリをクローンします:
    ```sh
    git clone https://github.com/code4fukui/hokuriku-kanko-route.git
    ```
2.  プロジェクトのディレクトリに移動します:
    ```sh
    cd hokuriku-kanko-route
    ```
3.  `index.html`（移動軌跡マップ）または `traffic.html`（混雑状況チャート）を直接ウェブブラウザで開きます。

## データソース

-   **加工済みデータ:** [code4fukui/mac-address](https://github.com/code4fukui/mac-address) - オリジナルのWi-Fiパケットセンシングデータから作成されたCSVファイル。
-   **オリジナルデータ:** [hokuriku-inbound-kanko/mac-address](https://github.com/hokuriku-inbound-kanko/mac-address) - 金沢大学による生のWi-Fiパケットセンシングデータ。
-   **データ公開元:** [北陸インバウンド観光DX・データコンソーシアム](https://kanko-dx.jp/case-study/1784/)
-   **データポータル:** [TIFDATA 北陸観光データポータル](https://tifdata.jp/)

## ライセンス

MIT License — 詳細は [LICENSE](LICENSE) を参照してください。
