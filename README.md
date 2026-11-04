# Image to STL Converter

PNG / JPEG / WebP画像から3種類の方式でSTLモデルを生成する、GitHub Pages対応のブラウザアプリです。

## 機能
- **高さマップ**：画像の明暗を高さに変換
- **シルエット押し出し**：透明部分と明るさのしきい値から形状を生成
- **リソファン**：画像の明暗を厚みに変換
- Three.jsによる3Dプレビュー（回転・拡大縮小）
- Binary STLダウンロード
- 画像処理・モデル生成はブラウザ内で完結

## GitHub Pagesで公開する方法
1. リポジトリの **Settings → Pages** を開く
2. **Build and deployment → Source** を **Deploy from a branch** にする
3. Branch を **main**、フォルダーを **/(root)** にして **Save**
4. 数分後、GitHub Pagesの公開URLへアクセス

## 注意
Three.jsはjsDelivr CDNから読み込みます。利用にはインターネット接続が必要です。シルエット方式はピクセル格子に基づく輪郭表現のため、細かな曲線は解像度設定に依存します。印刷前にスライサーでメッシュを確認してください。