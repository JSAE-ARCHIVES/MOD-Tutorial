# やること
- エクスポートしておいたstlファイルをblenderにインポートします。使用していたCADソフトの座標系によりインポート設定が変わる場合があります。  
- インポートしたモデルの位置調整を行います。

# インポート設定  
`blender`を起動して新規ファイルで`全般`を選択します。  
![blendファイルの新規作成](https://user-images.githubusercontent.com/81402033/138378518-98c7edc2-c17a-4736-b5ef-a47be6c2e332.png)
`ファイル`>`名前を付けて保存`で保存します。
保存場所はCarNameフォルダです．

`Aキー`でビューポート内のすべてのオブジェクトを選択し`Xキー`で削除
`Shift+C`で3Dカーソルを原点に配置します。（3Dカーソルの位置にモデルがインポートされるため）  
`ファイル`>`インポート`>`stl`でインポート。

![stlインポート1](https://user-images.githubusercontent.com/81402033/122321602-140a6380-cf5f-11eb-8c76-b0ab9d23a7cd.jpg)

## SOLIDWORKSの場合
右側のパネルで`トランスフォーム`>`Zが前方`、`Yが上`に設定
`STLをインポート`をクリック。

![solidworksインポート設定](https://user-images.githubusercontent.com/81402033/122321537-f76e2b80-cf5e-11eb-862e-0b1d6e1e5e30.jpg)

## Creoの場合  
右側のパネルで`トランスフォーム`>`スケール`を0.001に設定  
`Zが前方`、`Yが上`に設定
`STLをインポート`をクリック。  

![creoインポート設定](https://user-images.githubusercontent.com/81402033/122489249-28f7fd00-d01a-11eb-9ee2-01b08dd6e5f1.png)

## Autodesk Inventorの場合  
右側のパネルで`トランスフォーム`>`Zが前方`、`Yが上`に設定
`STLをインポート`をクリック。  

![inventorインポート設定](https://user-images.githubusercontent.com/81402033/122489479-c6ebc780-d01a-11eb-9dd5-90bffffa77cc.png)

## Autodesk Fusion360の場合  
右側のパネルで`トランスフォーム`>`スケール`を0.001に設定  
`Yが前方`、`Zが上`に設定
`STLをインポート`をクリック。  

![fusion360インポート設定](https://user-images.githubusercontent.com/81402033/122491593-3f548780-d01f-11eb-8c5a-7ee5793b5fbf.png)

## よくあるトラブル
#### インポートしたはずなのにblenderの3Dビューポート上に表示されない  
エクスポート/インポート時のスケール設定を確認してください。極端に大きいまたは小さいと3Dビューポート上でうまく表示されないことがあります。  

## 位置合わせ
左右の位置合わせ
- 編集モードで左右対称なパーツ（翼端板x2，IA，etc...）を`L`で選択>`Shift+S`でカーソルを選択物へを選択すると選択した頂点の中心に3Dカーソルが移動する。  
- オブジェクトモードで，オブジェクト>原点を設定>原点を3Dカーソルへ移動  
- `Shift+C`で3Dカーソルをワールド原点にリセット  
- `Shift+S`>`選択物→カーソル`でモデルがワールド原点に揃う（左右）
上下の位置合わせ  
- 上下方向はタイヤがXY平面に接するように`G`>`Z`で位置を合わせる。
前後の位置合わせ   
- 前後方向は`G`>`Y`で車両の重心がblender内のz軸上になるように調整する。  
位置合わせの完了
- 位置の調整が終わったら`オブジェクト>適用>全トランスフォーム`で位置合わせは完了  

以上で`3-4 stlファイルをblenderにインポートする`は終了です。  

| Back | Next |
|:---:|:---:|
| [3-3 blenderの導入](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/3-3%203D%E3%83%A2%E3%83%87%E3%83%AA%E3%83%B3%E3%82%B0%E3%82%BD%E3%83%95%E3%83%88(blender)%E3%81%AE%E5%B0%8E%E5%85%A5.md) | [3-5 オブジェクトの分割](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/3-5%20%E3%82%AA%E3%83%96%E3%82%B8%E3%82%A7%E3%82%AF%E3%83%88%E3%81%AE%E5%88%86%E5%89%B2.md) |

