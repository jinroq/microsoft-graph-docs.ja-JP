---
title: Microsoft Graph によって OneNote コンテンツと構造を取得する
description: " Office 365 のエンタープライズ ノートブック"
ms.openlocfilehash: d5a1b382535988e48b5b710d3685a344c5f5a40d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092501"
---
# <a name="get-onenote-content-and-structure-with-microsoft-graph"></a>Microsoft Graph によって OneNote コンテンツと構造を取得する

**適用対象**: OneDrive のコンシューマー ノートブック | Office 365 のエンタープライズ ノートブック

OneNote のコンテンツと構造を取得するには、ターゲット エンドポイントに GET 要求を送信します。たとえば次のようにします。

`GET ../onenote/pages/{id}`

要求が成功すると、Microsoft Graph は 200 HTTP 状態コードと、要求したエンティティまたはコンテンツを返します。 OneNote のエンティティは、OData バージョン 4.0 仕様に準拠した JSON オブジェクトとして返されます。

クエリ文字列オプションを使用すると、クエリをフィルターしてパフォーマンスを向上させることができます。


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a>要求 URI の構築

要求 URI を構築するには、サービス ルート URL から開始します。

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

次に、取得するリソースのエンドポイントを追加します ([リソース パス](#resource-paths-for-get-requests)については次のセクションを参照してください)。

完全な要求 URI は、次に示す例のいずれかのようになります。

- `https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections`
- `https://graph.microsoft.com/v1.0/me/onenote/notes/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?select=title,self`

> **注:** [サービス ルート URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url) の詳細についてはリンク先をご覧ください。

<a name="resource-paths"></a>

## <a name="resource-paths-for-get-requests"></a>GET 要求のリソース パス

次のリソース パスを使用して、ページ、セクション、セクション グループ、ノートブック、画像、またはファイル リソースを取得します。

- [ページ コレクション](#page-collection)
- [ページ エンティティ](#page-entity)
- [ページ プレビュー](#page-preview)
- [ページ HTML コンテンツ](#page-html-content)
- [セクション コレクション](#section-collection)
- [セクション エンティティ](#section-entity)
- [SectionGroup コレクション](#sectiongroup-collection)
- [SectionGroup エンティティ](#sectiongroup-entity)
- [ノートブック コレクション](#notebook-collection)
- [ノートブック エンティティ](#notebook-entity)
- [画像またはその他のファイル リソース](#image-or-other-file-resource)

<a name="get-pages"></a>

### <a name="page-collection"></a>ページ コレクション

すべてのノートブックのページ (メタデータ) を取得する。

`../pages[?filter,orderby,select,expand,top,skip,search,count]`

<br/>

特定のセクションからページ (メタデータ) を取得する。

`../sections/{section-id}/pages[?filter,orderby,select,expand,top,skip,search,count,pagelevel]`

<br/>
 
`search`クエリ文字列オプションは、コンシューマー ノートパソコンでのみ使用できます。

ページの既定の並べ替え順序は `lastModifiedTime desc` です。

既定のクエリは、親セクションを展開し、セクションの `id`、`name`、および `self` プロパティを選択します。

既定では、*GET ページ*要求に対して上位 20 のエントリのみが返されます。 **上位**クエリ文字列オプションを指定しない要求を行った場合、次の 20 エントリを取得するために使用できる `@odata.nextLink` リンクが応答で返されます。

セクションのページ コレクションの場合、**pagelevel** を使用して、ページのインデント レベルとセクション内でのその順序を返します。 

#### <a name="example"></a>例

`GET ../sections/{section-id}/pages?pagelevel=true`



<a name="get-page"></a> 

### <a name="page-entity"></a>ページ エンティティ

特定のページのメタデータを取得する 

`../pages/{page-id}[?select,expand,pagelevel]` 

<br/>

ページは、**parentNotebook** プロパティと **parentSection** プロパティを展開できます。

既定のクエリは、親セクションを展開し、セクションの `id`、`name`、および `self` プロパティを選択します。

**pagelevel** を使用して、ページのインデント レベルと親セクション内でのその順序を返します。 

#### <a name="example"></a>例

`GET ../pages/{page-id}?pagelevel=true`



<a name="get-page-preview"></a> 

### <a name="page-preview"></a>ページ プレビュー

ページのテキストと画像のプレビュー コンテンツを取得する。

`../pages/{page-id}/preview`

<br/>


JSON 応答には、ページに含まれているものを特定するために使用できる、プレビュー コンテンツが含まれています。

```json
{
  "@odata.context":"https://www.onenote.com/api/v1.0/$metadata#Microsoft.OneNote.Api.PagePreview",
  "previewText":"text-snippet",
  "links":{
    "previewImageUrl":{
      "href":"https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png"
    }
  }
}
```

**previewText** プロパティには、ページからのテキスト スニペットが含まれています。 Microsoft Graph は、最大 300 文字の完全な文字列を返します。 

ページにプレビュー UI のビルドに使用できる画像が含まれている場合、**previewImageUrl** オブジェクトの **href** プロパティには、事前認証されたパブリックの [image resource](#image-or-other-file-resource) のリンクが含まれます。 このリンクは HTML で使用できます。 それ以外の場合、**href** は、null 値を返します。

#### <a name="example"></a>例 

`<img src="https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png" />`


<a name="get-page-content"></a> 

### <a name="page-html-content"></a>ページ HTML コンテンツ

ページの HTML コンテンツを取得する。

`../pages/{page-id}/content[?includeIDs,preAuthenticated]`

(*[返される HTML コンテンツ](onenote-input-output-html.md)の詳細についてはリンク先をご覧ください*) 

<br/>

**includeIDs=true** クエリ文字列オプションを使用して、[ページを更新](onenote-update-page.md)するために使用する生成 ID を取得します。

**preAuthenticated=true** クエリ文字列オプションを使用して、ページ上の[画像リソース](#image-or-other-file-resource)のパブリック URL を取得します。パブリック URL は 1 時間有効です。 



<a name="get-sections"></a>

### <a name="section-collection"></a>セクション コレクション

ユーザーが所有するすべてのノートブックから、ネストされたセクション グループのセクションを含む、すべてのセクションを取得する。

`../sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

特定のセクション グループの直下にあるすべてのセクションを取得する。

`../sectionGroups/{sectiongroup-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

特定のノートブックの直下にあるすべてのセクションを取得する。

`../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

セクションは、**parentNotebook** プロパティと **parentSectionGroup** プロパティを展開できます。

セクションの既定の並べ替え順序は `name asc` です。

既定のクエリは、親ノートブックおよび親セクション グループを展開し、`id`、`name`、および `self` プロパティを選択します。



<a name="get-section"></a>

### <a name="section-entity"></a>セクション エンティティ

特定のセクションを取得します。

`../sections/{section-id}[?select,expand]` 

<br/>

セクションは、**parentNotebook** プロパティと **parentSectionGroup** プロパティを展開できます。

既定のクエリは、親ノートブックおよび親セクション グループを展開し、`id`、`name`、および `self` プロパティを選択します。



<a name="get-section-groups"></a>

### <a name="sectiongroup-collection"></a>SectionGroup コレクション

ユーザーが所有するすべてのノートブックから、ネストされたセクション グループを含む、すべてのセクション グループを取得する。

`../sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

特定のノートブックの直下にあるすべてのセクション グループを取得する。 

`../notebooks/{notebook-id}/sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

セクション グループは、**セクション**、**sectionGroups**、**parentNotebook**、および **parentSectionGroup** プロパティを展開できます。

セクション グループの既定の並べ替え順序は `name asc` です。

既定のクエリは、親ノートブックおよび親セクション グループを展開し、`id`、`name`、および `self` プロパティを選択します。



<a name="get-section-group"></a>

### <a name="sectiongroup-entity"></a>SectionGroup エンティティ

特定のセクション グループを取得します。

`../sectionGroups/{sectiongroup-id}[?select,expand]` 

<br/>

セクション グループは、**セクション**、**sectionGroups**、**parentNotebook**、および **parentSectionGroup** プロパティを展開できます。

既定のクエリは、親ノートブックおよび親セクション グループを展開し、`id`、`name`、および `self` プロパティを選択します。



<a name="get-notebooks"></a>

### <a name="notebook-collection"></a>ノートブック コレクション

ユーザーによって所有されるすべてのノートブックを取得する。 

`../notebooks[?filter,orderby,select,top,skip,expand,count]` 

<br/>

ノートブックは、**セクション**および **sectionGroups** プロパティを展開できます。

ノートブックの既定の並べ替え順序は `name asc` です。 



<a name="get-notebook"></a>

### <a name="notebook-entity"></a>ノートブック エンティティ

特定のノートブックを取得します。

`../notebooks/{notebook-id}[?select,expand]` 

<br/>

ノートブックは、**セクション**および **sectionGroups** プロパティを展開できます。



<a name="get-resource"></a>

### <a name="image-or-other-file-resource"></a>画像またはその他のファイル リソース

特定のリソースのバイナリ データを取得する。 

`../resources/{resource-id}/$value` 

<br/>

ファイルのリソース URI は、ページの[出力 HTML](onenote-input-output-html.md) にあります。

たとえば、**img** タグには、**data-fullres-src** 属性に元の画像のエンドポイント、**src** 属性に最適化された画像のエンドポイントが含まれます。 

#### <a name="example"></a>例

```html
<img 
    src="https://www.onenote.com/api/v1.0/me/notes/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://www.onenote.com/api/v1.0/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

**object** タグには、**data** 属性のファイル リソースのエンドポイントが含まれています。 

#### <a name="example"></a>例

```html
<object
    data="https://www.onenote.com/api/v1.0/me/notes/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" ... />
```

ページにある画像リソースへの事前認証された公開 URL を取得するには、[ページのコンテンツを取得する](#page-html-content)際にクエリ文字列に `preAuthenticated=true` を含めます (**例:**  `GET ../pages/{page-id}/content?preAuthenticated=true`)。 [出力 HTML](onenote-input-output-html.md#output-html-examples-for-images) に返されるパブリック URL は 1 時間有効です。 このフラグを設定していない場合、取得された画像は非公開で、またページのコンテンツの残りの部分と同様、それらを取得するために承認を必要とするため、ブラウザーで直接レンダリングすることはありません。 

> **注:** リソースのコレクションの取得はサポートされていません。 

ファイル リソースを取得する場合、**Accept** コンテンツ タイプを要求に含める必要はありません。

GET 要求の詳細については、Microsoft Graph API REST リファレンスの中の次のリソースを参照してください。

- [ページを取得する](/graph/api/page-get?view=graph-rest-1.0)
- [Get section](/graph/api/section-get?view=graph-rest-1.0)
- [Get sectionGroup](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [ノートブックを取得する](/graph/api/notebook-get?view=graph-rest-1.0) 




<a name="example"></a>

## <a name="example-get-requests"></a>GET 要求の例

OneNote のエンティティおよび検索ページ コンテンツを照会して、必要な情報だけを取得することができます。 次の例は、Microsoft Graph への GET 要求で、[サポートされているクエリ文字列オプション](#supported-odata-query-string-options)を使用するいくつかの方法を示しています。 

**次の点にご注意ください。**

- GET 要求はすべて、[サービス ルート URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url) で始まります。 <br/><br/>**例**: `https://www.onenote.com/api/v1.0/me/notes` および `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`

- URL クエリ文字列のスペースには %20 エンコードを使用する必要があります。<br/><br/>**例**: `filter=title%20eq%20'biology'`

- プロパティ名と OData 文字列比較では大文字と小文字が区別されます。 文字列比較には OData **tolower** 関数を使用することをお勧めします。<br/><br/>**例**: `filter=tolower(name) eq 'spring'`
 

### <a name="search--filter"></a>search & filter  

特定のアプリによって作成された、*recipe* という用語が含まれるページすべてを取得します (`search` はコンシューマー ノートブックでのみ使用可能)。

```
[GET] ../pages?search=recipe&filter=createdByAppId eq 'WLID-000000004C12821A'
```
 
### <a name="search--select"></a>search & select  

*golgi app* という用語が含まれるすべてのページの、タイトル、OneNote クライアントのリンク、**contentUrl** リンクを取得します (`search` はコンシューマー ノートブックでのみ使用可能)。

```
[GET] ../pages?search=golgi app&select=title,links,contentUrl
```
 
### <a name="expand"></a>expand 

すべてのノートブックを取得し、そのセクションとセクション グループを展開します。  

```
[GET] ../notebooks?expand=sections,sectionGroups
```

<br/>

特定のセクション グループを取得し、そのセクションとセクション グループを展開します。  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections,sectionGroups
```

<br/>

ページを取得し、その親セクションと親ノートブックを展開します。

```
[GET] ../pages/{page-id}?expand=parentSection,parentNotebook
```

### <a name="expand-multiple-levels"></a>expand (複数レベル)  

すべてのノートブックを取得してセクションとセクション グループを展開し、各セクション グループのすべてのセクションを展開します。  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections)
```
 
> **注:** 子エンティティの親を展開、または親エンティティの子を展開すると、循環参照が作成されますが、これはサポートされていません。

 
### <a name="expand--select-multiple-levels"></a>expand & select (複数レベル)  

特定のセクション グループの名前と **self** リンクを取得し、そのすべてのセクションの名前と **self** リンクを取得します。  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections(select=name,self)&select=name,self
```

<br/>

すべてのセクションの名前と **self** リンクを取得し、各セクションの親ノートブックの名前と作成時刻を取得します。  

```
[GET] ../sections?expand=parentNotebook(select=name,createdTime)&select=name,self
```

<br/>
 
すべてのページのタイトルと ID を取得し、親セクションと親ノートブックの名前を取得します。

```
[GET] ../pages?select=id,title&expand=parentSection(select=name),parentNotebook(select=name)
```

### <a name="expand--levels-multiple-levels"></a>expand & levels (複数レベル)  

すべてのノートブック、セクション、セクション グループを取得します。  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections,sectionGroups(levels=max;expand=sections))
```
 
### <a name="filter"></a>filter

2014 年 10 月に作成されたセクションすべてを取得します。

```
[GET] ../sections?filter=createdTime ge 2014-10-01 and createdTime le 2014-10-31
```

<br/>

2015 年 1 月 1 日以降に特定のアプリによって作成されたページを取得します。

```
[GET] ../pages?filter=createdByAppId eq 'WLID-0000000048118631' and createdTime ge 2015-01-01
```

### <a name="filter--expand"></a>filter & expand  

特定のノートブックに含まれるすべてのページを取得します。既定では、この API は 20 エントリを戻します。

```
[GET] ../pages?filter=parentNotebook/id eq '{notebook-id}'&expand=parentNotebook
```

<br/>

*学校*のノートブックにあるすべてのセクションの名前と **pagesUrl** リンクを取得します。 OData の文字列比較は大文字小文字が区別されるので、ベスト プラクティスとして **tolower** 関数を使用します。

```
[GET] ../notebooks?filter=tolower(name) eq 'school'&expand=sections(select=name,pagesUrl)
```

### <a name="filter--select--orderby"></a>filter & select & orderby   

セクション名に *spring* という語が含まれるすべてのセクションの名前と **pagesUrl** リンクを取得します。セクションを最終変更日で並べ替えます。

```
[GET] ../sections?filter=contains(tolower(name),'spring')&select=name,pagesUrl&orderby=lastModifiedTime desc
```
 
### <a name="orderby"></a>orderby

**createdByAppId** プロパティ、次に作成時刻を基準に順序を並べ替えて、最初の 20 ページを取得します。既定では、この API は 20 エントリを戻します。

```
[GET] ../pages?orderby=createdByAppId,createdTime desc
```

### <a name="search--filter--top"></a>search & filter & top 

*cell division* という語句を含む、2015 年 1 月 1 日以降に作成されたページで新しいものを 5 つ取得します。 既定ではこの API は 20 エントリを返します。最大では 100 エントリを返します。 ページの既定の並べ替え順序は `lastModifiedTime desc` です (`search` は、コンシューマー ノートブックでのみ使用可能)。

```
[GET] ../pages?search="cell division"&filter=createdTime ge 2015-01-01&top=5
```

### <a name="search--filter--top--skip"></a>search & filter & top & skip  

結果セット内の次の 5 ページを取得します (`search` は、コンシューマー ノートブックでのみ使用可能)。

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=5
```

<br/>

それから次の 5 ページを取得します (`search` は、コンシューマー ノートブックでのみ使用可能)。

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=10
```

> **注:** **search** と **filter** がどちらも同じ要求に適用される場合、結果には両方の条件に一致するエンティティのみが含まれます。
 
### <a name="select"></a>select

ユーザーのノートブック内にあるすべてのセクションの名前、作成時刻、**self** リンクを取得します。

```
[GET] ../sections?select=name,createdTime,self
```

<br/>

特定のページのタイトル、作成時刻、OneNote クライアント リンクを取得します。

```
[GET] ../pages/{page-id}?select=title,createdTime,links
```

### <a name="select--expand--filter-multiple-levels"></a>select & expand & filter (複数レベル)  

ユーザーの既定ノートブックにあるすべてのセクションの名前と **pagesUrl** リンクを取得します。

```
[GET] ../notebooks?select=name&expand=sections(select=name,pagesUrl)&filter=isDefault eq true
```

### <a name="top--select--orderby"></a>top & select & orderby 

最初の 50 ページのタイトルと **self** リンクを取得します。タイトルのアルファベット順に並べられます。既定ではこの API は 20 エントリを返します。最大では 100 エントリを返します。ページの既定の並べ替え順序は `lastModifiedTime desc` です。

```
[GET] ../pages?top=50&select=title,self&orderby=title
```

### <a name="skip--top--select--orderby"></a>skip & top & select & orderby  

51 ページ目から 100 ページ目までを取得します。既定ではこの API は 20 エントリを返します。最大では 100 エントリを返します。

```
[GET] ../pages?skip=50&top=50&select=title,self&orderby=title
```

> **注:** 既定のエントリ数を取得する pages に対する GET 要求 (つまり、**top** 式を指定しない要求) は、応答で次の 20 エントリを取得するために使用できる **@odata.nextLink** リンクを戻します。
 

<a name="supported-odata-query-string-options"></a>

## <a name="supported-odata-query-string-options"></a>サポートされている OData クエリ文字列オプション

Microsoft Graph に GET 要求を送信する場合、OData クエリ文字列オプションを使用してクエリをカスタマイズして、必要な情報だけを取得できます。 このオプションを使用することにより、サービスへの呼び出し回数が減り、応答ペイロードのサイズが小さくなるので、パフォーマンスも向上します。

> **注:** この記事の例では読みやすくするために、URL クエリ文字列内のスペースで必要な %20 パーセント エンコードを使用していません: `filter=isDefault%20eq%20true`
 
| クエリ オプション | 例と説明 |  
|------|------|  
| count | <p>`count=true`</p><p>コレクション内のエンティティのカウントです。この値は、応答の **@odata.count** プロパティで戻ります。</p> |  
| expand | <p>`expand=sections,sectionGroups`</p><p>応答でインラインを返すナビゲーション プロパティ。**expand** 式には次のプロパティがサポートされています。<br /> - ページ: **parentNotebook**、**parentSection**<br /> - セクション: **parentNotebook**、**parentSectionGroup**<br /> - セクション グループ: **sections**、**sectionGroups**、**parentNotebook**、**parentSectionGroup**<br /> - ノートブック: **sections**、**sectionGroups**</p><p>既定では、ページの GET 要求は **parentSection** を展開し、セクションの **id**、**name**、**self** の各プロパティを選択します。セクションとセクションのグループの既定の GET 要求は **parentNotebook** と **parentSectionGroup** の両方を展開し、親の **id**、**name**、**self** の各プロパティを選択します。</p><p>1 つのエンティティまたはコレクションに使用できます。<br />コンマを使用して複数のプロパティを区切ります。<br />プロパティ名では、大文字と小文字を区別します。</p> |   
| filter | <p>`filter=isDefault eq true`</p><p>結果セットの入力に含めるかどうかを決めるブール式。サポートされている OData 演算子と関数:<br /> - 比較演算子: **eq**、**ne**、**gt**、**ge**、**lt**、**le**<br /> - 論理演算子: **and**、**or**、**not**<br /> - 文字列関数: **contains**、**endswith**、**startswith**、**length**、**indexof**、**substring**、**tolower**、**toupper**、**trim**、**concat**</p><p>[プロパティ](#onenote-entity-properties)名と OData 文字列比較では大文字と小文字が区別されます。 文字列比較には OData **tolower** 関数を使用することをお勧めします。<br /><br />**例**: `filter=tolower(name) eq 'spring'`</p> |  
| orderby | <p>`orderby=title,createdTime desc`</p><p>並べ替え基準を示す[プロパティ](#onenote-entity-properties)です。オプションで、**asc** (既定) または **desc** 並べ替え順序を指定します。要求対象コレクション内のエンティティの任意のプロパティで並べ替えが可能です。</p><p>ノートブック、セクション グループ、セクションの既定の並べ替え順序は `name asc` で、ページの場合には `lastModifiedTime desc` (最新の変更ページが先頭になります)。</p><p>複数のプロパティはコンマで区切り、任意の順序で一覧表示します。 プロパティ名では、大文字と小文字を区別します。</p> |  
| search | <p>`search=cell div`</p><p>コンシューマー ノートパソコンでのみ使用可能。</p><p>ページ タイトル、ページ本文、画像の代替テキスト、画像の OCR テキストで検索する用語または語句です。既定では、検索クエリは関連度で並べ替えて結果を返します。</p><p>OneNote は、Bing のフルテキスト検索を使用して、語句の検索、語形変化、スペルの曖昧さ、関連性とランキング、単語分割、複数の言語、他のフルテキスト検索機能をサポートします。 検索文字列では、大文字と小文字が区別されません。</p><p>ユーザーが所有しているノートブック内のページにのみ適用されます。 インデックス付けされたコンテンツは非公開であり、所有者のみがアクセスできます。 パスワードで保護されたページにはインデックスは付けられません。 `pages` エンドポイントにのみ適用されます。</p> |  
| select | <p>`select=id,title`</p><p>返す[プロパティ](#onenote-entity-properties)。 1 つのエンティティまたはコレクションに使用できます。 コンマを使用して複数のプロパティを区切ります。 プロパティ名では、大文字と小文字を区別します。</p> |  
| skip | <p>`skip=10`</p><p>結果セットでスキップするエントリの数。通常、結果のページングに使用されます。</p> |  
| top | <p>`top=50`</p><p>結果セット内で返すエントリ数で、最大数は 100 です。既定値は 20 です。</p> |  

Microsoft Graph にも、親セクション内でページのレベルと順序を取得する `pagelevel` クエリ文字列オプションが用意されています。 特定のセクションのページのクエリ、または特定のページのクエリにのみ適用されます。 

#### <a name="examples"></a>例 

- `GET ../sections/{section-id}/pages?pagelevel=true` 
- `GET ../pages/{page-id}?pagelevel=true` 

### <a name="supported-odata-operators-and-functions"></a>サポートされている OData 演算子と関数

Microsoft Graph は、**フィルター**式で次の OData 演算子および関数をサポートしています。 OData 式を使用する場合には、次の点に注意してください。

- URL クエリ文字列のスペースは `%20` エンコードで置換する必要があります。<br/><br/>**例:** `filter=isDefault%20eq%20true`

- プロパティ名と OData 文字列比較では大文字と小文字が区別されます。 文字列比較には OData **tolower** 関数を使用することをお勧めします。<br/><br/>**例:** `filter=tolower(name) eq 'spring'`


| 比較演算子 | 例 |  
|------|------|  
| eq<br />(等しい) | `createdByAppId eq '{app-id}'` |  
| ne<br />(等しくない) | `userRole ne 'Owner'` |  
| gt<br />(より大きい) | `createdTime gt 2014-02-23` |  
| ge<br />(以上) | `lastModifiedTime ge 2014-05-05T07:00:00Z` |  
| lt<br />(より小さい) | `createdTime lt 2014-02-23` |  
| le<br />(以下) | `lastModifiedTime le 2014-02-23` |  

<br/>

| 論理演算子 | 例 |  
|------|------|  
| and | `createdTime le 2014-01-30 and createdTime gt 2014-01-23` |  
| or | `createdByAppId eq '{app-id}' or createdByAppId eq '{app-id}'` |  
| not | `not contains(tolower(title),'school')` |  

<br/>
  
| String 関数 | 例 |  
|------|------|   
| contains | `contains(tolower(title),'spring')` |  
| endswith | `endswith(tolower(title),'spring')` |  
| startswith | `startswith(tolower(title),'spring')` |  
| length | `length(title) eq 19` |  
| indexof | `indexof(tolower(title),'spring') eq 1` |  
| substring | `substring(tolower(title),1) eq 'spring'` |  
| tolower | `tolower(title) eq 'spring'` |  
| toupper | `toupper(title) eq 'SPRING'` |  
| trim | `trim(tolower(title)) eq 'spring'` |  
| concat | `concat(title,'- by MyRecipesApp') eq 'Carrot Cake Recipe - by MyRecipesApp'` |  
 

<a name="properties"></a>

## <a name="onenote-entity-properties"></a>OneNote エンティティのプロパティ

**filter**、**select**、**expand**、および **orderby** クエリ式には、OneNote エンティティのプロパティを含めることができます。 

#### <a name="example"></a>例

`../sections?filter=createdTime ge 2015-01-01&select=name,pagesUrl&orderby=lastModifiedTime desc` 

クエリ式のプロパティ名は大文字小文字を区別します。

プロパティとプロパティの種類の一覧については、Microsoft Graph API REST リファレンスの中の次のリソースを参照してください。

- [ページを取得する](/graph/api/page-get?view=graph-rest-1.0)
- [Get section](/graph/api/section-get?view=graph-rest-1.0)
- [Get sectionGroup](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [ノートブックを取得する](/graph/api/notebook-get?view=graph-rest-1.0) 



**expand** クエリ文字列オプションは、以下のナビゲーション プロパティとともに使用できます。

- ページ: **parentNotebook**、**parentSection**
- セクション: **parentNotebook**、**parentSectionGroup**
- セクション グループ: **sections**、**sectionGroups**、**parentNotebook**、**parentSectionGroup**
- ノートブック: **sections**、**sectionGroups**


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-get-requests"></a>要求および *GET* 要求の応答に関する情報

| 要求データ | 説明 |  
|------|------|  
| プロトコル | すべての要求は SSL/TLS HTTPS プロトコルを使用します。 |  
| 承認ヘッダー | <p>`Bearer {token}`。`{token}` は、登録済みアプリの有効な OAuth 2.0 アクセス トークンです。</p><p>これがないか、無効の場合、401 ステータス コードで要求は失敗します。「[認証とアクセス許可](permissions-reference.md)」を参照してください。</p> |  
| Accept ヘッダー | <p> OneNote エンティティとエンティティ セットの場合、`application/json`</p><p> ページ コンテンツの場合、`text/html`</p> | 

<br/>

| 応答データ | 説明 |  
|------|------|  
| 成功コード | 200 HTTP ステータス コード。 |  
| 応答本文 | JSON 形式のエンティティまたはエンティティ セット、ページ HTML、またはファイル リソースのバイナリ データの OData 表現。  |  
| エラー | 要求が失敗すると、API は応答本文の **@api.diagnostics** オブジェクトに[エラー](onenote-error-codes.md)を返します。 |  
| X-CorrelationId ヘッダー | 要求を一意に識別する GUID。Microsoft サポートと問題のトラブルシューティングを行う際に、この値を Date ヘッダーの値とともに使用できます。 |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-notes-service-root-url"></a>Microsoft Graph のノート サービスのルート URL の構築

Microsoft Graph ノートのルート URL は、Microsoft Graph ノートへのすべての呼び出しで次の形式を使用します。

`https://graph.microsoft.com/{version}/me/onenote/`  

URL の `version` セグメントは、使用する Microsoft Graph のバージョンを示しています。 安定した運用コードには `v1.0` を使用します。 開発中の機能を試すには `beta` を使用します。 ベータ版の機能は変更される可能性があるため、運用コードでは使用しないでください。 

現在のユーザーがアクセスできる OneNote コンテンツには `me` を使用します (所有と共有)。 指定されたユーザー (URL 内) が現在のユーザーと共有している OneNote コンテンツには `users/{id}` を使用します。 ユーザー ID を取得するには [Microsoft Graph](https://graph.microsoft.com/v1.0/users) を使用します。 


<a name="permissions"></a>

## <a name="permissions-for-get-requests"></a>GET 要求のアクセス許可

OneNote のコンテンツまたは構造を取得するには、適切なアクセス許可を要求する必要があります。 

次のスコープは、Microsoft Graph に対する GET 要求を許可します。 アプリの動作に必要な最低限のアクセス許可を選択してください。

次から選択します。

- Notes.read
- Notes.ReadWrite
- Notes.ReadWrite.All

アクセス許可の範囲とその動作方法の詳細については、「[Microsoft Graph のアクセス許可のリファレンス](permissions-reference.md)」を参照してください。

<a name="see-also"></a>

## <a name="see-also"></a>関連項目

- [OneNote ページの入出力 HTML](onenote-input-output-html.md)
- [OneNote との統合](integrate-with-onenote.md)
- [OneNote の開発者ブログ](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Stack Overflow 掲載の OneNote の開発に関する質問](https://go.microsoft.com/fwlink/?LinkID=390182)
- [OneNote GitHub のリポジトリ](https://go.microsoft.com/fwlink/?LinkID=390178)  
