|dms名|match|AddItem使用|
|---|---|---|
|E-Hentai.dms|http&#58;//g.e-hentai.org/[^g]|×|
|[bobx.dms](#bobxdms)|http&#58;//www.bobx.com/[^g]|×|
|flickr.dms|https?://www.flickr.com/photos/|×|
|fuskator_full.dms|http&#58;//fuskator.com/full/[^g]|○|
|imgchili.dms|http&#58;//imgchili.net/[^g]|×|
|imgur.dms|http&#58;//imgur.com/[^g]|○|
|jkforum.dms|http&#58;//www.jkforum.net/[^g]|○|
|my_poco_cn.dms|http&#58;//my.poco.cn/[^g]|○|
|photo_poco_cn_lastphoto.dms|http&#58;//photo.poco.cn/lastphoto[^g]|○|
|[twitter.dms](#twitterdms)|twitter.com/[^/]+/status|○|
|xhamster_photos.dms|http&#58;//[^/]*xhamster.com/photos/gallery/[^g]|○|

AddItem使用が○のスクリプトについては、  
https://github.com/rentan/Irvine/tree/master/Dorothy2/common  
のAddItemクラスを使用しています。

---

#### E-Hentai.dms

#### bobx.dms
リンクのインポートでフォトセットの画像一覧のページ、例えば  
http://www.bobx.com/av-idol/mayu-kamiya/photoset/graphis-_115-hatsunugi-0-10-10.html  
を階層数0でリンクを取得。

http://www.bobx.com/av-idol/mayu-kamiya/large-mayu-kamiya-1459661/  
http://www.bobx.com/av-idol/mayu-kamiya/large-mayu-kamiya-1459662/  
　：  
のような large- となっているURLをアイテム登録。

#### flickr.dms
#### fuskator_full.dms
#### imgchili.dms
#### imgur.dms
#### jkforum.dms
#### my_poco_cn.dms
#### photo_poco_cn_lastphoto.dms
#### twitter.dms
画像ツイートのstatusのURL、例えば  
https://twitter.com/suzukisakiika/status/667982087140413440  
をアイテム登録すると2つの画像がアイテム追加されます。  
複数のツイートの画像をダウンロードしたい場合は画像のタイムラインのページ、例えば  
https://twitter.com/suzukisakiika/media  
で「IrvineにすべてのURLを送る」を実行してstatusのURLを登録すればOK。

#### xhamster_photos.dms
