---
title: OneNote ページ コンテンツを更新する
description: " Office 365 のエンタープライズ ノートブック"
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 1c7aad42687dac87eda907f66e99ff1a4b11b861
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778741"
---
# <a name="update-onenote-page-content"></a>OneNote ページ コンテンツを更新する

**適用対象** OneDrive のコンシューマー ノートブック | Office 365 のエンタープライズ ノートブック


OneNote ページのコンテンツを更新する場合は、ページの *content* エンドポイントに PATCH 要求を送信します。

`PATCH ../notes/pages/{id}/content`</p>

メッセージの本文で JSON 変更オブジェクトを送信します。要求が成功すると、Microsoft Graph は 204 HTTP 状態コードを返します。


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a>要求 URI の構築

要求 URI を構築するには、サービス ルート URL から開始します。

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

次に、ページの *content* エンドポイントを追加します。

- **ページ HTML と、すべての定義済み *data-id* の値を取得する**<br/><br/>`../pages/{id}/content`   

- **ページ HTML、すべての定義済み *data-id* の値、およびすべての生成された *id* の値を取得する**<br/><br/>`../pages/{page-id}/content?includeIDs=true` 

**data-id** と **id** の値は、更新する要素の **target** 識別子として使用されます。

 
完全な要求 URI は、次のようになります。<br/><br/>`https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content`


[サービス ルート URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url) の詳細についてはリンク先をご覧ください。


<a name="message-body"></a>

## <a name="construct-the-message-body"></a>メッセージ本文の構築

OneNote ページの HTML には、**div** 要素、**img** 要素、**ol** 要素などの構造に編成されたテキスト、画像などのコンテンツが含まれています。OneNote ページのコンテンツを更新する場合は、ページ上で HTML 要素を追加および置換します。

変更内容は JSON 変更オブジェクトの配列としてメッセージ本文に入れて送信します。ターゲット要素、新しい HTML コンテンツ、コンテンツに対する操作が各オブジェクトにより指定されます。

2 つの変更を定義する配列を次に示します。最初の変更では画像が兄弟として段落の上に挿入され、2 番目の変更ではアイテムが最後の子としてリストに追加されます。

```json
[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="Image above the target paragraph" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the end of the list</li>'
  }
]
```

[その他の例](#example-requests)を参照してください。


### <a name="attributes-for-json-change-objects"></a>JSON 変更オブジェクトの属性

PATCH 要求の JSON オブジェクトの定義には、**target** 属性、**action** 属性、**position** 属性、および **content** 属性を使用します。

#### <a name="target"></a>ターゲット

更新する要素。値として次の ID のいずれかを指定する必要があります。

| Identifier | 説明 |  
|------|------|  
| #{data-id} | <p>この ID は、[ページを作成](onenote-create-page.md)するときや[更新](onenote-update-page.md)するときに、入力 HTML の要素で任意で定義されます。値の先頭に # を付けます。</p><p> 例:<br/>`'target':'#intro'` は要素 `<div data-id="intro" ...>` をターゲットとします</p> |  
| ID | <p>これは、Microsoft Graph から得られる[生成済み ID](#generated-ids) であり、ほとんどの置換操作で必要になります。 プレフィックス # を追加しないでください。</p><p> 例:<br/>`'target':'div:{33f8a2...}{37}'` は要素 `<div id="div:{33f8a2...}{37}" ...>` をターゲットとします</p><p>[入力 HTML](onenote-input-output-html.md) に定義されている **id** 値とこれらを混同しないでください。入力 HTML で送信される **id** 値は、すべて破棄されます。</p> |  
| body | ページ上で最初の div をターゲットにするキーワード。プレフィックス # を追加してはいけません。 |  
| title | ページ タイトルをターゲットにするキーワード。プレフィックス # を追加してはなりません。 |  
 
#### <a name="action"></a>action

ターゲット要素に対して実行するアクション。「[サポートされる要素とアクション](#supported-elements-and-actions)」を参照してください。

| アクション | 説明 |  
|------|------|  
| append | <p>指定されたコンテンツを最初または最後の子としてターゲットに追加します。追加される位置 (最初または最後) は、**position** 属性によって決まります。</p><p>**body**、**div**、**ol**、**ul** 要素にのみ適用されます。</p> |  
| insert | 指定されたコンテンツを兄弟としてターゲットの前または後に追加します。追加される位置 (前または後) は、**position** 属性によって決まります。 |  
| prepend | <p>指定されたコンテンツを最初の子としてターゲットに追加します。**append** + **before** のショートカット。</p><p>**body**、**div**、**ol**、**ul** 要素にのみ適用されます。</p> |  
| replace | <p>指定したコンテンツでターゲットを置換します。</p><p>ほとんどの **replace** アクションは、ターゲットの[生成された ID](#generated-ids) を使用する必要があります (ただし、div 内の **img** 要素と **object** 要素を除きます。これらは、**data-id** の使用もサポートしています)。</p> |  
 
#### <a name="position"></a>position

指定されたコンテンツを追加する位置。ターゲット要素を基準とした相対位置です。省略すると、既定値として **after** が使用されます。

| 位置 | 説明 |  
|------|------|  
| after (既定値) |<p>**append** の場合: ターゲット要素の最後の子。</p><p>**insert** の場合: ターゲット要素の後続の兄弟。</p> |
| before | <p>**append** の場合: ターゲット要素の最初の子。</p><p>**insert** の場合: ターゲット要素の先行の兄弟。</p> |

#### <a name="content"></a>content

ページに追加する整形式 HTML の文字列と画像またはファイル バイナリ データ。コンテンツにバイナリ データが含まれている場合、コンテンツ タイプとして `multipart/form-data` を利用し、"Commands" パートを含む要求を送信する必要があります ([例](#multipart-request-with-binary-content)参照)。 
 

<a name="generated-ids"></a>

### <a name="generated-ids"></a>生成された ID
Microsoft Graph は、更新可能なページで要素に対して **id** 値を生成します。 生成された ID を取得するには、GET 要求で `includeIDs=true` クエリ文字列を使用します。

`GET ../notes/pages/{page-id}/content?includeIDs=true` 

> **注:** API は、ページ作成要求およびページ更新要求の[入力 HTML](onenote-input-output-html.md) で定義された **id** の値をすべて破棄します。

次の例は、ページの[出力 HTML](onenote-input-output-html.md) の段落と画像に対して生成された ID を示します。

```html
<p id="p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}">Some text on the page</p>
<img id="img:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{45}" ... />
```

生成された **id** 値はページ更新後に変更されることがあるため、これらの値を使用する PATCH 要求を作成する前に、現行値を取得する必要があります。
 
ターゲット要素は、**data-id** または **id** 値を使用して次のように指定できます。

- **append** アクションと **insert** アクションでは、いずれの ID もターゲット値として使用できます。
- **replace** アクションでは、すべての要素について、生成された IDを使用する必要があります。ただし、ページ タイトル、および div 内の画像とオブジェクトを除きます。 
  - タイトルを置換する場合は、**title** キーワードを使用します。 
  - div 内の画像とオブジェクトを置換する場合は、**data-id** または **id** のどちらかを使用します。

次の例では、ターゲットに **id** 値を使用します。生成された ID と共に # プレフィックスを使用しないでください。

```json
[
   {
    'target':'p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}',
    'action':'insert',
    'position':'before',
    'content':'<p>This paragraph goes above the target paragraph.</p>'
  }
]
```

<a name="support-matrix"></a>

## <a name="supported-elements-and-actions"></a>サポートされる要素とアクション

ページ上の要素の多くは更新可能ですが、要素の種類ごとに特定のアクションがサポートされています。サポートされるターゲット要素と、各要素でサポートされる更新アクションを次の表に示します。

| 要素 | 置換 | 子の追加 | 兄弟の挿入 |  
|------|:------:|:------:|:------:|  
| body<br /> (ページの最初の div をターゲットとする) | いいえ | **はい** | いいえ |  
| div<br /> ([絶対配置](onenote-abs-pos.md)) | いいえ | **はい** | いいえ |  
| div<br /> (div 内) | **はい**<br/>(id のみ) | **はい** | **はい** |   
| img、object<br /> (div 内) | **はい** | no | **はい** |   
| ol、ul | **はい**<br/>(id のみ) | **はい** | **はい** |   
| table | **はい**<br/>(id のみ) | いいえ | **はい** |   
| p、li、h1-h6 | **はい**<br/>(id のみ) | いいえ | **はい** |   
| title | **はい** | いいえ | no |  
 
<br/>

次の要素では更新アクションはサポートされていません。

- img ([絶対配置](onenote-abs-pos.md))
- object ([絶対配置](onenote-abs-pos.md))
- tr、td
- meta
- head
- span
- a
- style タグ


<a name="examples"></a>

## <a name="example-requests"></a>要求の例

更新要求には、JSON 変更オブジェクトとして表現される変更が 1 つ以上含まれています。これらのオブジェクトでは、ページ上のさまざまなターゲットや、ターゲットに対するさまざまなアクションとコンテンツを定義できます。

次の例に、PATCH 要求で使用される JSON オブジェクトと完全な PATCH 要求を示します。

- [子要素の追加](#append-child-elements)
- [兄弟要素の挿入](#insert-sibling-elements)
- [要素の置換](#replace-elements)
- [完全な PATCH 要求](#complete-patch-request-examples)


<a name="append-examples"></a>

### <a name="append-child-elements"></a>子要素の追加

**append** アクションでは、**body**、**div** (div 内)、**ol**、**ul** 要素に子が追加されます。**position** 属性により、ターゲットの前または後に子を追加することが決定されます。既定の位置は**後**です。

#### <a name="append-to-a-div"></a>div への追加

次の例では、2 つの子ノードが **div1** 要素に追加されます。画像が最初の子として追加され、段落が 2 番目の子として追加されます。 

```json
[
 {
    'target':'#div1',
    'action':'append',
    'position':'before',
    'content':'<img data-id="first-child" src="image-url-or-part-name" />'
  },
  {
    'target':'#div1',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph appended to the div</p>'
  }
]
```
 

#### <a name="append-to-the-body-element"></a>*body* 要素への追加

**body** は、任意のページ上の最初の div 内に子要素を追加するためのショートカットとして使用できます。

次の例では、ページの最初の div に 2 つの段落を最初の子と最後の子として追加しています。**body** ターゲットと共に # を使用しないでください。この例では、**prepend** アクションを **append** + **before** のショートカットとして使用しています。

```json
[
  {
    'target':'body',
    'action':'prepend',
    'content':'<p data-id="first-child">New paragraph as first child in the first div</p>'
  },
  {
    'target':'body',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph as last child in the first div</p>'
  }
]
```
 

#### <a name="append-to-a-list"></a>リストへの追加

次の例では、リスト項目がターゲット リストに最後の子として追加されます。この項目では既定以外のリスト スタイルが使用されるため、**list-style-type** プロパティが定義されます。

```json
[
  {
    'target':'#circle-ul',
    'action':'append',
    'content':'<li style="list-style-type:circle">Item at the end of the list</li>'
  }
]
```
 

<a name="insert-examples"></a>

### <a name="insert-sibling-elements"></a>兄弟要素の挿入

**insert** アクションでは、兄弟がターゲット要素に追加されます。**position** 属性により、ターゲットの前または後に兄弟を挿入することが決定されます。既定の位置は**後**です。「[**insert** をサポートする要素](#supported-elements-and-actions)」をご覧ください。

#### <a name="insert-siblings"></a>兄弟の挿入

次の例では、ページに 2 つの兄弟ノードが挿入されます。**para1** 要素の上に画像が追加され、**para2** 要素の下に段落が追加されます。

```json
[
  {
     'target':'#para1',
     'action':'insert',
     'position':'before',
     'content':'<img src="image-url-or-part-name" alt="Image inserted above the target" />'
  },
  {
    'target':'#para2',
     'action':'insert',
     'content':'<p data-id="next-sibling">Paragraph inserted below the target</p>'
  }
]
```
 

<a name="replace-examples"></a>

### <a name="replace-elements"></a>要素の置換

**data-id** と生成された **id** のいずれかをターゲット値として使用し、div 内にある **img** 要素および **object** 要素を置換できます。ページ タイトルを置換する場合は、**title** キーワードを使用します。[**replace** をサポートするその他すべての要素](#supported-elements-and-actions)については、生成された ID を使用する必要があります。

#### <a name="replace-an-image"></a>画像の置換

次の例では、画像の **data-id** をターゲットとして使用して、div 内の画像が置換されます。 

```json
[
  {
    'target':'#img1',
    'action':'replace',
    'content':'<div data-id="new-div"><p>This div replaces the image</p></div>'
  }
]
```
 

#### <a name="update-a-table"></a>表の更新 

次の例は、生成された ID を使用して表を更新する方法を示します。**tr** 要素と **td** 要素の置換はサポートされていませんが、表全体を置換することができます。

```json
[
  {
    'target':'table:{de3e0977-94e4-4bb0-8fee-0379eaf47486}{11}',
    'action':'replace',
    'content':'<table data-id="football">
      <tr><td><p><b>Brazil</b></p></td><td><p>Germany</p></td></tr>
      <tr><td><p>France</p></td><td><p><b>Italy</b></p></td></tr>
      <tr><td><p>Netherlands</p></td><td><p><b>Spain</b></p></td></tr>
      <tr><td><p>Argentina</p></td><td><p><b>Germany</b></p></td></tr></table>'
  }
]
```
 

#### <a name="change-the-title"></a>タイトルの変更 

次の例は、ページのタイトルを変更する方法を示します。タイトルを変更するには、ターゲット値として **title** キーワードを使用します。title ターゲットでは # は使用しないでください。

```json
[
  {
    'target':'title',
    'action':'replace',
    'content':'New title'
  }
]
```
 

#### <a name="update-a-to-do-item"></a>To Do アイテムの更新

次に示す例では、replace アクションを使用して、To Do チェック ボックス アイテムを完了状態に変更します。

```json
[
  {
    'target':'#task1',
    'action':'replace',
    'content':'<p data-tag="to-do:completed" data-id="task1">First task</p>'
  }
]
```

**data-tag** 属性の使用法の詳細については、「[ノート シールを使用する](onenote-note-tags.md)」を参照してください。


<a name="complete-requests"></a>

### <a name="complete-patch-request-examples"></a>完全な PATCH 要求の例

次の例に、完全な PATCH 要求を示します。

#### <a name="request-with-text-content-only"></a>テキスト コンテンツのみの要求

次の例では、PATCH 要求でコンテンツ タイプとして **application/json** が使用されています。 コンテンツにバイナリ データが含まれていないとき、この形式を使用できます。

```json
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: application/json
Authorization: Bearer {token}

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url" alt="New image from a URL" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]
```
 
<a name="multipart"></a>

#### <a name="multipart-request-with-binary-content"></a>バイナリ コンテンツを含むマルチパート要求 

次の例は、バイナリ データを含んでいるマルチパート PATCH 要求を示しています。マルチパート要求には、**application/json** コンテンツ タイプを指定し、JSON 変更オブジェクトの配列を含める "Commands" 部分が必要になります。その他のデータ部分に、バイナリ データを含めることができます。部分の名前は、通常、ミリ秒単位での現在の時刻、またはランダムな GUID が付加された文字列になります。

```json
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: multipart/form-data; boundary=PartBoundary123
Authorization: Bearer {token}

--PartBoundary123
Content-Disposition: form-data; name="Commands"
Content-Type: application/json

[
  {
    'target':'img:{2998967e-69b3-413f-a221-c1a3b5cbe0fc}{42}',
    'action':'replace',
    'content':'<img src="name:image-part-name" alt="New binary image" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]

--PartBoundary123
Content-Disposition: form-data; name="image-part-name"
Content-Type: image/png

... binary image data ...

--PartBoundary123--
```

<a name="request-response-info"></a>

## <a name="request-and-response-information-for-patch-requests"></a>PATCH 要求の要求情報と応答情報

| 要求データ | 説明 |  
|------|------|  
| プロトコル | すべての要求は SSL/TLS HTTPS プロトコルを使用します。 |  
| 承認ヘッダー | <p>`Bearer {token}`。`{token}` は、登録済みアプリの有効な OAuth 2.0 アクセス トークンです。</p><p>これがないか、無効の場合、401 ステータス コードで要求は失敗します。「[認証とアクセス許可](permissions-reference.md)」を参照してください。</p> |  
| Content-Type ヘッダー | <p>JSON 変更オブジェクトの配列の `application/json`。メッセージ本文または[マルチパート要求](#multipart-request-with-binary-content)の必須の "Commands" パートで直接送信。</p><p>マルチパート要求はバイナリ データを送信するときに必須であり、コンテンツ タイプとして `multipart/form-data; boundary=part-boundary` を使用します。`{part-boundary}` は、各データ パートの開始と終了を伝える文字列です。</p> |  

<br/> 

| 応答データ | 説明 |  
|------|------|  
| 成功コード | 204 HTTP ステータス コード。PATCH 要求に対して JSON データは返されません。 |  
| エラー | Microsoft Graph から返されることのある OneNote エラーに関する詳細については、「[Microsoft Graph の OneNote API のエラー コード](onenote-error-codes.md)」をご覧ください。 |  
 
 

<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a>Microsoft Graph サービスのルート URL の構築

OneNote サービスのルート URL は、OneNote API へのすべての呼び出しで次の形式を使用します。

`https://graph.microsoft.com/{version}/me/onenote/`

URL の `version` セグメントは、使用する Microsoft Graph のバージョンを示しています。 安定した運用コードには `v1.0` を使用します。 開発中の機能を試すには `beta` を使用します。 ベータ版の機能は変更される可能性があるため、運用コードでは使用しないでください。

現在のユーザーがアクセスできる OneNote コンテンツには `me` を使用します (所有と共有)。 指定されたユーザー (URL 内) が現在のユーザーと共有している OneNote コンテンツには `users/{id}` を使用します。 [Azure AD Graph API](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog) の使用。


> **注:** `https://graph.microsoft.com/v1.0/users`で GET 要求を行うことにより、ユーザー ID を取得できます。



<a name="permissions"></a>

## <a name="permissions"></a>アクセス許可

OneNote ページを更新するには、適切なアクセス許可を要求する必要があります。アプリの動作に必要な最低限のアクセス許可を選択してください。

- Notes.ReadWrite
- Notes.ReadWrite.All

アクセス許可のスコープと動作のしくみの詳細については、「[OneNote のアクセス許可のスコープ](permissions-reference.md)」を参照してください。
   

<a name="see-also"></a>

## <a name="see-also"></a>関連項目

- [画像とファイルを追加する](onenote-images-files.md)
- [OneNote との統合](integrate-with-onenote.md)
- [OneNote の開発者ブログ](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Stack Overflow 掲載の OneNote の開発に関する質問](https://go.microsoft.com/fwlink/?LinkID=390182)
- [OneNote GitHub のリポジトリ](https://go.microsoft.com/fwlink/?LinkID=390178)  
