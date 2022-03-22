# 3-3 使用するシフトの導入
# やること
1. blenderをインストールし初期設定を行います。  
1. blenderの基本操作を学習します。
1. ksEditorをダウンロードして起動できる状態にします．
# blenderとは？  
![blender_logo_socket](https://user-images.githubusercontent.com/81402033/122319391-89743500-cf5b-11eb-8c16-8e6cd646870a.png)

>Blender は3DCGアニメーションを作成するための統合環境アプリケーションです。オープンソースのフリーウェアであり、本格的かつ商用アプリにも負けない機能を持ち、世界中のユーザに利用されています。([Blender.jp](https://blender.jp/)より引用)  

blenderの操作ではショートカットキーを多用します。
# blenderのインストール
1. [blender公式サイト](https://www.blender.org/)に飛んでDownload Blenderの青いボタンを押す  
1. 使用するOSに合ったものを選択すると自動的にインストーラーがダウンロードされる  
1. ダブルクリックでインストーラーを起動  
1. I accept the terms in the Licence Agreementにチェックをつけて次へ  
1. インストール先はデフォルトのままでOK  
1. インストール完了  

# blenderの初期設定
1. blenderを起動
1．起動画面で全般をクリック
1. `Edit`>`Preferences...`で設定画面を開く  

![blender初期設定プリファレンス設定](https://user-images.githubusercontent.com/81402033/122319035-fdfaa400-cf5a-11eb-98be-c5cfc1147b04.jpg)


### blenderの日本語化
左側`Interface`の`Translation`>`Language`を`English`から`Japanese`に変更し、`Tooltips`、`Interface`にチェック  

![blender初期設定インターフェース](https://user-images.githubusercontent.com/81402033/122317825-179aec00-cf59-11eb-8c54-e2ae96fb2cbc.jpg)


### テンキーレスキーボードの場合
左側`入力`の`キーボード`>`テンキーを模倣`にチェック  

![blender初期設定テンキーの模倣](https://user-images.githubusercontent.com/81402033/122317986-58930080-cf59-11eb-8e20-ce2273c0f258.jpg)


### 視点の操作  
左側`視点の操作`の`周回とパン`>`選択部分を中心に回転`、`深度`にチェック  
`ズーム`>ズーム方法`継続`、ズーム座標軸`垂直`、`マウス位置でズーム`にチェック  

![blender初期設定視点の操作](https://user-images.githubusercontent.com/81402033/122318104-88da9f00-cf59-11eb-991c-a87ae839a77f.jpg)


### マウスの右クリックで選択  
筆者は右クリックで選択に慣れてしまったのでこのチュートリアルは右クリック選択で進行します。  
変更したい人は左側`キーマップ`の`プリファレンス`>`Select with Mouse Button`で好きなほうを選べます。  

![blender初期設定選択ボタン](https://user-images.githubusercontent.com/81402033/122318256-b9223d80-cf59-11eb-9e5e-5790a4b84ad6.jpg)

### システム
NVIDIA製のグラフィックボードを搭載してるPCの場合、チェックをつけておくとレンダービュー等で描画が早くなります。
### undo回数の設定
`Ctrl+Z`でアンドゥできる回数のを増やすことができます。特に理由がない場合は256にしておくことをお勧めします。PCの性能に不安がある場合は必要に応じた数に設定してください。  
![undo回数設定](https://user-images.githubusercontent.com/81402033/138585841-00b2462e-ed2b-452a-9642-24cd62443d01.png)

### 設定の保存
左下ボタンから`プレファレンスの保存`

![blender初期設定プリファレンスを保存](https://user-images.githubusercontent.com/81402033/122318501-1918e400-cf5a-11eb-80f4-7cba8123bae1.jpg)

### シーン統計情報の表示
右下のバージョン情報が書いてある部分を右クリック→シーン統計  
で超点数，ポリゴン数等が確認できる．
# blenderの基本操作

[blender基本操作](https://czpanel.com/lecture/blender/basic/operation/)  
[blenderの視点操作](https://blender-cg.net/mausu-sitenn/)  
[blenderチュートリアル](https://www.google.com/search?q=blender+%E3%83%81%E3%83%A5%E3%83%BC%E3%83%88%E3%83%AA%E3%82%A2%E3%83%AB&rlz=1C1ASUM_enJP944JP944&oq=blender+%E3%83%81%E3%83%A5%E3%83%BC%E3%83%88%E3%83%AA%E3%82%A2%E3%83%AB&aqs=chrome..69i57.4696j0j4&sourceid=chrome&ie=UTF-8)等で検索するとたくさんヒットするのでわからないことがあったら検索してください。  

以上でblenderの導入は終了です。

# ksEditorとは？
作成した3Dモデル(.fbx形式)をAssettoCorsa用の形式（.kn5）に変換します．  
マテリアルの質感の設定もksEditor上で行います．  

# KsEditorのダウンロード
[こちら](https://ascobash.wordpress.com/2015/07/22/kseditor/)のサイトにアクセスし，Download(v6)をクリック．  
ロシア語？のダウンロードサイトが表示されるので右下の白いボタンをクリックするとダウンロードが開始されます．  
ダウンロードしたzipファイルを展開するとたくさんファイルが入っていますが，ksEditor.exeというファイルを使用します．  
インストールせずにその都度.exeファイルを開いて起動するので展開したフォルダをわかりやすい場所に置いておくとよいでしょう．  
ksEditorは何度も起動することになると思うので，ショートカットを作成してデスクトップに置いておくか，起動してからタスクバーにピン止めすると便利です．  


| Back | Next |
|:---:|:---:|
| [3-2 CADからエクスポート](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/3-2%20CAD%E3%81%8B%E3%82%89%E3%82%A8%E3%82%AF%E3%82%B9%E3%83%9D%E3%83%BC%E3%83%88.md) | [3-4 stlファイルをblenderにインポートする](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/3-4%20stl%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%82%92blender%E3%81%AB%E3%82%A4%E3%83%B3%E3%83%9D%E3%83%BC%E3%83%88%E3%81%99%E3%82%8B.md) |
