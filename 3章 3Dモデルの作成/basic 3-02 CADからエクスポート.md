# **3-2 CADからエクスポート**
# やること  
- CAD上でボルトナット等の部品を抑制または非表示にしてエクスポートされないようにします。
- CAD上でねじ穴やパイプ等を埋めてエクスポート時のポリゴン数を削減します。
- エクスポートでCADモデルがポリゴンに変換される際にポリゴン数が少なくなるよう、エクスポート設定を変更します。  
- CADモデルを3DCG系ソフトで扱えるようにするために、3Dモデルの一般的な形式(.stl)に変換してエクスポートします。  

# 用意するもの
- 各チームで使用しているCADソフト  
- 車両のフルアセンブリCADモデル

# 作業1 CAD上で不要なパーツを抑制/非表示にする
- ポリゴン数はAssettoCorsaでプレイする際のPCの負荷（主にGPU）に直結するので、エクスポートする前の段階でパーツを削減しておく必要があります。
- ボルトやナット等の部品はエクスポートすると非常にポリゴン数が多いモデルになります。また、個数も多いため車両全体のポリゴン数が大幅に増加してしまいます。  
- ボルトナット以外でも見た目に影響しないと思われるパーツはエクスポート内容に含めないようにすることで大幅なポリゴン数の削減になります。
- 後の工程で削除することも可能なので神経質になる必要はありません。CAD上でまとめて扱いやすいパーツを抑制/非表示すると効率が良いでしょう。    

# 作業2 CAD上でねじ穴やパイプを埋める


立方体モデルは12ポリゴンでも  
<img src="https://user-images.githubusercontent.com/81402033/147043253-bb1b88b2-adb6-4cb2-ba02-847addd52eb0.png" width="500">  

穴をあけると120ポリゴンに  
<img src="https://user-images.githubusercontent.com/81402033/147043447-1c85f45f-829d-4dff-87c7-ca5691063420.png" width="500">  

円柱は120ポリゴンでも  
<img src="https://user-images.githubusercontent.com/81402033/147043636-61a1557b-9012-48e0-ad7b-ecb8104343e9.png" width="500">  

パイプにすると232ポリゴンに  
<img src="https://user-images.githubusercontent.com/81402033/147043715-a5cdad85-d59e-4f1d-a318-2d6fd7a70552.png" width="500">  
このように、穴やパイプはポリゴン数が増える原因となるため、CADの段階で埋めてしまうことが望ましいです。 

# 作業3 エクスポート設定  
- CADからポリゴンモデルに変換される際の解像度を設定します。
- ソフトごとに少し異なる設定をする必要があるので使用しているCADソフトの項目を参照してください。（SOLIDWORKS以外のソフトは検証が甘いです。すみません。）
- エクスポート先はCarNameフォルダです。  

### SOLIDWORKS  
- `ファイル>指定保存` からファイルの種類`.stl`を選択。  
- `オプション`を開く。  
- 単位を`m`に設定する。  
- 解像度を粗表示にする。  
![SOLIDWORKSエクスポート1](https://user-images.githubusercontent.com/81402033/122487977-74f57280-d017-11eb-8f25-f9aef1cc626f.jpg)
![solidworksエクスポート設定](https://user-images.githubusercontent.com/81402033/142764722-4096aec9-2d8a-4178-b2e5-1844f97669a8.png)


___
### Creo  
- `ファイル`>`名前を付けて保存`>`コピーを保存`からタイプ`.stl`を選択。  
- `オプション`を開く。    
- 解像度を最低設定にする  
![creoエクスポート設定1](https://user-images.githubusercontent.com/81402033/122488123-c7cf2a00-d017-11eb-88d6-8f6118b37324.jpg)
![creoエクスポート設定2](https://user-images.githubusercontent.com/81402033/122488127-c9005700-d017-11eb-9fa6-897d9996d842.jpg)

___
### Autodesk Inventor  
- `ファイル`>`書き出し`>`CAD形式`からファイルの種類`.stl`を選択。
- `オプション`を開く。  
- 単位を`m`に設定する。  
- 解像度を最低にする。  
![inventorエクスポート設定1](https://user-images.githubusercontent.com/81402033/122487989-7c1c8080-d017-11eb-950c-296e27f9d10a.jpg)
![inventorエクスポート設定2](https://user-images.githubusercontent.com/81402033/122487993-7de64400-d017-11eb-8537-a356381aa5ee.jpg)
![inventorエクスポート設定3](https://user-images.githubusercontent.com/81402033/122487996-7fb00780-d017-11eb-90b9-88d96870fa51.jpg)

___
### Autodesk Fusion360
- `ファイル`>`3Dプリント`  
- 右側3Dプリントタブで`選択`、`メッシュを...`にチェック  
- 3Dビューポート内でメッシュを選択する。  
- リファインメントオプションで解像度を最低にする。
![fusion360エクスポート設定](https://user-images.githubusercontent.com/81402033/122695384-2cd68a00-d27b-11eb-9547-592136f9b100.png)
![fusion360エクスポート設定2](https://user-images.githubusercontent.com/81402033/122695392-306a1100-d27b-11eb-937d-1841fe562e75.png)

___
以上で 3-2 CADからエクスポート は終了です。

| Back | Next |
|:---:|:---:|
| [3-1 フォルダ作成](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/3-1%20%E3%83%95%E3%82%A9%E3%83%AB%E3%83%80%E4%BD%9C%E6%88%90.md) | [3-3 blenderの導入](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/3-3%203D%E3%83%A2%E3%83%87%E3%83%AA%E3%83%B3%E3%82%B0%E3%82%BD%E3%83%95%E3%83%88(blender)%E3%81%AE%E5%B0%8E%E5%85%A5.md) |

