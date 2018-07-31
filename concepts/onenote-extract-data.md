# <a name="use-onenote-api-div-tags-to-extract-data-from-captures"></a>OneNote API div タグを使用してキャプチャからデータを抽出する 

**適用対象** OneDrive のコンシューマー ノートブック | Office 365 のエンタープライズ ノートブック

OneNote API を使用して、画像から名刺データを抽出したり、URL からレシピや製品データを抽出したりします。

<a name="attributes"></a>

## <a name="extraction-attributes"></a>抽出の属性

単に div を含めるだけで、データの抽出や変換ができます。div は [create-page](onenote-create-page.md) または [update-page](onenote_update_page.md) 要求で、ソース コンテンツ、抽出メソッド、およびフォールバックの動作を指定します。API は抽出したデータを、読みやすい形式でページに表示します。 

```html
<div
  data-render-src="image-or-url"
  data-render-method="extraction-method"
  data-render-fallback="fallback-action">
</div>
```

### <a name="data-render-src"></a>data-render-src

コンテンツ ソース。名刺の画像、または数多くの人気レシピや製品の Web サイトの絶対 URL にできます。必須。

URL を指定するときに最適な結果を得るために、ソースの Web ページの HTML で定義された正規 URL を使用してください (定義されている場合)。たとえば、正規 URL はソースの Web ページで次のように定義されます。

`<link rel="canonical" href="www.domainname.com/page/123/size12/type987" />` 


### <a name="data-render-method"></a>data-render-method

実行する抽出メソッド。必須。

| 値 | 説明 |
|:------|:------|
| extract.businesscard | 名刺の抽出。 |
| extract.recipe | レシピの抽出。 |
| extract.product | 製品リストの抽出。 |
| extract | 不明な種類の抽出。 |

最適の結果を得るために、コンテンツの種類 (`extract.businesscard`、`extract.recipe`、または `extract.product`) を指定してください (種類がわかっている場合)。 種類が不明の場合は、`extract` メソッドを使用してください。OneNote API が種類の自動検出を試行します。

### <a name="data-render-fallback"></a>data-render-fallback

抽出できない場合のフォールバック動作。省略すると、既定の **render** になります。 

| 値 | 説明 |
|:------|:------|
| render | レシピまたは製品の Web ページのソース画像またはスナップショットを表示します。 |
| none | 何も実行しません。<br /><br />このオプションは、抽出コンテンツに加えて、名刺または Web ページのスナップショットをページに必ず含める場合に役立ちます。例に示すように、要求には個別の `img` 要素を含めてください。 |

<a name="biz-card"></a>

## <a name="business-card-extractions"></a>名刺の抽出

OneNote API は、個人または会社の名刺の画像に基づいて、次の連絡先情報の検索および表示を試行します。

- 名前
- タイトル
- 組織
- 電話および FAX 番号
- 郵送先および実際の住所
- 電子メール アドレス
- Web サイト



<img alt="An example business card extraction" src="images/biz-card-extraction.png" width="200">

ページには、抽出された連絡先情報が含まれる vCard (.VCF ファイル) も組み込まれます。この vCard は、ページの HTML コンテンツを取得するときに連絡先情報を入手するのに便利な方法です。

### <a name="common-scenarios-for-business-card-extractions"></a>名刺抽出の一般的なシナリオ

#### <a name="extract-business-card-information-and-also-render-the-business-card-image"></a>名刺情報を抽出して、名刺の画像を表示する

`extract.businesscard` メソッドと `none` フォールバックを指定します。また、画像を参照する `src` 属性を含む `img` 要素も送信します。API ではコンテンツを抽出できない場合は、名刺の画像のみが表示されます。

```html 
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard"
    data-render-fallback="none">
</div>
<img src="name:scanned-card-image" />
```


#### <a name="extract-business-card-information-and-render-the-business-card-image-only-if-the-extraction-fails"></a>名刺情報を抽出する。抽出に失敗した場合のみ名刺の画像を表示する

`extract.businesscard` メソッドを指定して、既定の `render` フォールバックを使用します。API ではコンテンツを抽出できない場合は、その代わりに名刺の画像が表示されます。

```html
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard">
</div>
```
 
名刺の抽出では、画像はマルチパートの要求の名前付きパートとして送信されます。要求で画像を送信する例については、「[画像とファイルの追加](onenote_images_files.md)」を参照してください。


<a name="recipe"></a>

## <a name="recipe-extractions"></a>レシピの抽出

OneNote API は、レシピの URL に基づいて、次の情報の検索および表示を試行します。

- 完成例の画像
- 評価
- 材料
- 手順
- 準備、調理、および合計の時間
- 分量


<img alt="An example recipe extraction" src="images/recipe-extraction.png" width="200">

この API は、*Allrecipes.com*、*FoodNetwork.com*、および *SeriousEats.com* など、数多くの人気サイトのレシピ用に最適化されています。

### <a name="common-scenarios-for-recipe-extractions"></a>レシピ抽出の一般的なシナリオ

#### <a name="extract-recipe-information-and-also-render-a-snapshot-of-the-recipe-webpage"></a>レシピ情報を抽出して、レシピの Web ページのスナップショットも表示する

`extract.recipe` メソッドと `none` フォールバックを指定します。また、レシピの URL に設定した `data-render-src` 属性を含む `img` 要素も送信します。API ではコンテンツを抽出できない場合は、レシピの Web ページのスナップショットのみが表示されます。

おそらく、このシナリオが最も多くの情報を提供することになります。Web ページには、お客様のレビューや提案などの追加情報が含まれている場合があるためです。

```html 
<div
    data-render-src="http://allrecipes.com/recipe/guacamole/"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<img data-render-src="http://allrecipes.com/recipe/guacamole/" />
```
 

#### <a name="extract-recipe-information-and-render-a-snapshot-of-the-recipe-webpage-only-if-the-extraction-fails"></a>レシピ情報を抽出する。抽出に失敗した場合のみレシピの Web ページのスナップショットも表示する

`extract.recipe` メソッドを指定して、既定の render フォールバックを使用します。API ではコンテンツを抽出できない場合は、その代わりにレシピの Web ページのスナップショットが表示されます。

```html  
<div
    data-render-src="http://www.foodnetwork.com/recipes/alton-brown/creme-brulee-recipe.html"
    data-render-method="extract.recipe">
</div>
```


#### <a name="extract-recipe-information-and-also-render-a-link-to-the-recipe"></a>レシピ情報を抽出し、そのレシピへのリンクも表示する

`extract.recipe` メソッドと `none` フォールバックを指定します。レシピの URL に設定された `src` 属性を含む `a` 要素も送信します (または、ページに追加するその他の情報を送信することもできます)。API ではコンテンツを抽出できない場合は、レシピのリンクのみが表示されます。

```html  
<div
    data-render-src="http://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<a href="http://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html">Recipe URL</a>
``` 


<a name="product"></a>

## <a name="product-listing-extractions"></a>製品リストの抽出

- タイトル
- 評価
- 主要画像
- 説明
- 機能
- 仕様



<img alt="An example product listing extraction" src="images/product-extraction.png" width="200">

この API は、*Amazon.com* や *HomeDepot.com* など、数多くの人気サイトの製品用に最適化されています。

### <a name="common-scenarios-for-recipe-extractions"></a>レシピ抽出の一般的なシナリオ

#### <a name="extract-product-information-and-also-render-a-snapshot-of-the-product-webpage"></a>製品情報を抽出して、製品の Web のスナップショットも表示する

`extract.product` メソッドと `none` フォールバックを指定します。また、製品の URL に設定した `data-render-src` 属性を含む `img` 要素も送信します。API ではコンテンツを抽出できない場合は、製品の Web ページのスナップショットのみが表示されます。

おそらく、このシナリオが最も多くの情報を提供することになります。Web ページには、お客様のレビューや提案などの追加情報が含まれている場合があるためです。

```html 
<div
    data-render-src="http://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<img data-render-src="http://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO" />
```


#### <a name="extract-product-information-and-render-a-snapshot-of-the-product-webpage-only-if-the-extraction-fails"></a>製品情報を抽出する。抽出に失敗した場合のみ製品の Web ページのスナップショットも表示する

`extract.product` メソッドを指定して、既定の render フォールバックを使用します。API ではコンテンツを抽出できない場合は、その代わりに製品の Web ページのスナップショットが表示されます。

```html 
<div
    data-render-src="http://www.sears.com/craftsman-19hp-42-8221-turn-tight-174-hydrostatic-yard-tractor/p-07120381000P"
    data-render-method="extract.product">
</div>
```
 

#### <a name="extract-product-information-and-also-render-a-link-to-the-product"></a>製品情報を抽出し、その製品へのリンクも表示する

`extract.product` メソッドと `none` フォールバックを指定します。製品の URL に設定された `src` 属性を含む `a` 要素も送信します (または、ページに追加するその他の情報を送信することもできます)。API ではコンテンツを抽出できない場合は、ページのリンクのみが表示されます。

```html 
<div
    data-render-src="http://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<a href="http://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001">Product URL</a>
```


<a name="unknown"></a> 

## <a name="unknown-content-type-extractions"></a>不明な種類のコンテンツの抽出

送信するコンテンツの種類 (名刺、レシピ、製品) がわからない場合、修飾されていない `extract` メソッドを使用して、OneNote API が対象種類を自動検出するようにできます。この方法は、目的のアプリが各種のキャプチャを送信する場合に使用できます。

> **注:** 送信するコンテンツの種類がわかっている場合は、`extract.businesscard`、`extract.recipe`、または `extract.product` のメソッドを使用してください。 これにより、最適な抽出結果が得られるようになることがあります。
 
### <a name="common-scenarios-for-unknown-extractions"></a>不明な抽出の一般的なシナリオ

#### <a name="send-an-image-or-a-url-and-render-the-supplied-image-or-a-snapshot-of-the-webpage-if-the-extraction-fails"></a>画像または URL を送信して、抽出に失敗した場合は指定された画像または Web ページのスナップショットを表示する

API が自動的にコンテンツの種類を検出するように `extract` メソッドを指定して、既定の render フォールバックを使用します。API ではコンテンツを抽出できない場合は、その代わりに指定された画像または Web ページのスナップショットが表示されます。

```html 
<div
    data-render-src="some image or url"
    data-render-method="extract">
</div>
```


<a name="request-response-info"></a>

## <a name="response-information"></a>応答情報

| 応答データ | 説明 |  
|------|------|  
| 成功コード | 成功した POST 要求に対しては 201 HTTP ステータス コード、成功した PATCH 要求に対しては 204 HTTP ステータス コードが戻ります。 |  
| エラー| Microsoft Graph から返されることのある OneNote エラーに関する詳細については、「[Microsoft Graph の OneNote API のエラー コード](onenote_error_codes.md)」をご覧ください。 |  


<a name="permissions"></a>

## <a name="permissions"></a>アクセス許可

OneNote ページを作成または更新するには、適切なアクセス許可を要求する必要があります。アプリの動作に必要な最低限のアクセス許可を選択してください。

#### <a name="permissions-for-post-pages"></a>POST ページのアクセス許可

- Notes.Create
- Notes.ReadWrite
- Notes.ReadWrite.All  

#### <a name="permissions-for-patch-pages"></a>PATCH ページのアクセス許可

- Notes.ReadWrite
- Notes.ReadWrite.All

アクセス許可の範囲とその動作方法の詳細については、「[Microsoft Graph のアクセス許可のリファレンス](permissions_reference.md)」をご覧ください。


<a name="see-also"></a>

## <a name="see-also"></a>関連項目

- [OneNote ページを作成する](onenote-create-page.md)
- [OneNote ページ コンテンツを更新する](onenote_update_page.md)
- [画像とファイルを追加する](onenote_images_files.md)
- [OneNote との統合](integrate_with_onenote.md)
- [OneNote の開発者ブログ](http://go.microsoft.com/fwlink/?LinkID=390183)
- [Stack Overflow 掲載の OneNote の開発に関する質問](http://go.microsoft.com/fwlink/?LinkID=390182)
- [OneNote GitHub のリポジトリ](http://go.microsoft.com/fwlink/?LinkID=390178)  

