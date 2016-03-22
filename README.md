|dms名|match|AddItem使用|
|---|---|---|
|[E-Hentai.dms](#e-hentaidms)|`http://g.e-hentai.org/s/[^g]`|×|
|[bobx.dms](#bobxdms)|`http://www.bobx.com/[^g]`|×|
|flickr.dms|`https?://www.flickr.com/photos/`|×|
|fuskator_full.dms|`http://fuskator.com/full/[^g]`|○|
|imgchili.dms|`http://imgchili.net/[^g]`|×|
|[imgur.dms](#imgurdms)|`http://imgur.com/[^g]`|○|
|jkforum.dms|`http://www.jkforum.net/[^g]`|○|
|my_poco_cn.dms|`http://my.poco.cn/[^g]`|○|
|photo_poco_cn_lastphoto.dms|`http://photo.poco.cn/lastphoto[^g]`|○|
|[twitter.dms](#twitterdms)|`twitter.com/[^/]+/status`|○|
|xhamster_photos.dms|`http://[^/]*xhamster.com/photos/gallery/[^g]`|○|

AddItem使用が○のスクリプトについては、  
https://github.com/rentan/Irvine/tree/master/Dorothy2/common  
のAddItemクラスを使用しています。

---

#### E-Hentai.dms
画像のサムネイル一覧のページ、例えば  
http://g.e-hentai.org/g/914744/04b52e129e/  
を階層0でリンクを取得する。

すると、  
http://g.e-hentai.org/s/01d7a1a653/914744-22  
http://g.e-hentai.org/s/0a57cc0513/914744-34  
　:  
のような画像単体のページのURLが取得できるので、それらをアイテム登録する。

#### bobx.dms
リンクのインポートでフォトセットの画像一覧のページ、例えば  
http://www.bobx.com/av-idol/mayu-kamiya/photoset/graphis-_115-hatsunugi-0-10-10.html  
を階層数0でリンクを取得する。

すると、
http://www.bobx.com/av-idol/mayu-kamiya/large-mayu-kamiya-1459661/  
http://www.bobx.com/av-idol/mayu-kamiya/large-mayu-kamiya-1459662/  
　:  
のような large- となっているURLが取得できるので、それらをアイテム登録する。

#### flickr.dms
#### fuskator_full.dms
#### imgchili.dms
#### imgur.dms
http://imgur.com/a/4BFk7  
http://imgur.com/a/uA9lL#0  
のようなアルバムのURLをアイテム登録すると、アルバムの全画像のURLのアイテムが追加される。

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
