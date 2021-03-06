# この章でやること
効率よく作業を進めるために，この章で作ったものを格納するためのフォルダを作成します．ksEditor（3dモデルデータをassetto corsaにコンバートするためのソフト）でマテリアルやテクスチャを自動ロードするのにフォルダ構造が重要です．    
#### フォルダの作成
carname(半角小文字，任意の名前)フォルダを作成します．この章で作成する3Dモデルファイル全般を格納するフォルダです．  
**※ディレクトリに2バイト文字（日本語）を含まないように注意してください．** ksEditorでエラーの原因となります．  
carnameフォルダの中にtextureフォルダ（**名前重要！**）を作成します．
今後作成するテクスチャ画像ファイルはこのフォルダ内に保存します．  

第3章 3Dモデルの作成が終わるころにはフォルダの中はこのようになります．
![3Dモデル開発のフォルダ構造](https://user-images.githubusercontent.com/81402033/138374112-50e53019-490a-4ba5-bc23-c418ae2a3be2.png)
# 各ファイルの説明
#### textureフォルダ
テクチャを入れるフォルダです．ksEditorはこの名前のフォルダからテクスチャを自動ロードするのでフォルダ名は正確につけてください．**T**exture texture**s**はNG
#### carname.blend
blenderのファイルです．3Dモデルの作成はこのファイルで行います．
#### carname.blendN
[blenderのバックアップファイル](https://www.cgradproject.com/archives/2162/)です．blenderで保存するたびに更新されます．　拡張子の数字を消すとblendファイルとして開けるようになります．
#### carname.fbx
blenderからエクスポートした3Dモデルデータです．
#### carname.fbx.ini
ksEditor内のマテリアル設定がテキストファイル形式で保存されています．ksEditorでfbxを開くときにこのiniファイルからマテリアル設定がロードされるようになっています．  
#### carname.kn5
assetto corsa専用のファイルです.ksEditorでfbxからコンバートして作成します．
#### carname_fullassem.stl
CADからエクスポートした3Dモデルデータです．  
  
これで下準備は完了です。それでは作業に取り掛かりましょう！

| Back | Next |
|:---:|:---:|
| [2-n　2章の最後](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/3-1%20CAD%E3%81%8B%E3%82%89%E3%82%A8%E3%82%AF%E3%82%B9%E3%83%9D%E3%83%BC%E3%83%88.md) | [3-2 CADからエクスポート](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/3-2%20CAD%E3%81%8B%E3%82%89%E3%82%A8%E3%82%AF%E3%82%B9%E3%83%9D%E3%83%BC%E3%83%88.md) |
