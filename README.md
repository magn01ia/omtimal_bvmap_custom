# omtimal_bvmap_mod
[国土地理院最適化ベクトルタイル](https://github.com/gsi-cyberjapan/optimal_bvmap)にて公開されているスタイルを  
[unvt/nanban(国連ベクトルタイルツールキットのDockerコンテナ)](https://github.com/unvt/nanban)  
に同梱されている[unvt/charites](https://github.com/unvt/charites)を利用して編集したもの。　　

charites convert std.json  
↓
建築物3Dのymlファイルを追加  
↓
charites build std.yml  

## 変更点
### 建築物の3D表示
vt-codeで分類されている建築物の種別によってfill-extrusion-heightで高さ情報を与える。  

3103(高層建物):100  
3102(堅ろう建物):50  
3112(堅ろう無壁舎):30    
その他はすべて10とした。
