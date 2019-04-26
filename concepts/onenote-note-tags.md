---
title: OneNote ページでノート シールを使用する
description: " Office 365 のエンタープライズ ノートブック"
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: fb1067b2b564e8431aaa8a4bf8ca094a2b5d127d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555462"
---
# <a name="use-note-tags-in-onenote-pages"></a>OneNote ページでノート シールを使用する

**適用対象** OneDrive のコンシューマー ノートブック | Office 365 のエンタープライズ ノートブック

次の図に示すように、`data-tag` 属性を使用してチェック ボックス、星、その他の組み込みノート シールを OneNote ページに追加したり、更新したりします。

![OneNote ページに表示される 3 つのノート シール](images/note-tags-example.png)


<a name="attributes"></a>

## <a name="note-tag-attributes"></a>ノート シールの属性

OneNote ページの HTML では、ノート シールは `data-tag` 属性として示されます。次に例を示します。

- チェック マークのない To Do ホックス:  `<p data-tag="to-do">` 

- チェック マークのある To Do ホックス:  `<p data-tag="to-do:completed">` 

- 星:  `<h2 data-tag="important">` 

`data-tag` の値は shape で構成されますが、status の場合もあります (すべての[サポートされる値](#built-in-note-tags-for-onenote)をご覧ください)。

| プロパティ | 説明 |  
|:------|:------|  
| shape | ノート シールの識別子 (例: to-do`to-do` または important`important`)。 |  
| status | チェック ボックス ノート シールの状態。 チェック ボックスを完了状態に設定する場合にのみ使用します。 |  
 

<a name="note-tags"></a>

## <a name="add-or-update-note-tags"></a>ノート シールの追加または更新

組み込みのノート シールは、サポートされた要素で data-tag`data-tag` 属性を使用するだけで、追加したり更新したりすることができます。たとえば、重要としてマークされた段落があるとします。 For example, here's a paragraph marked as important:

```html
<p data-tag="important">...</p>
```

複数のノート シールをコンマで区切ります。

```html
<p data-tag="important, critical">...</p>
```

次の要素の data-tag`data-tag` を定義できます。

- p 
- ul、ol、li (詳細については、「[リストのノート シール](#note-tags-on-lists)」を参照)
- img 
- h1 - h6 
- title 

Microsoft Graph で使用できるノート シールのリストの「[組み込みノート シール](#built-in-note-tags-for-onenote)」を参照してください。 Microsoft Graph を使用したカスタム シールの追加または更新はサポートされていません。
 
### <a name="examples"></a>例

最初の項目が完了状態の簡単な To Do リストを以下に示します。

```html 
<p data-tag="to-do:completed" data-id="prep">Till garden bed</p> 
<p data-tag="to-do" data-id="spring">Plant peas and spinach</p>
<p data-tag="to-do" data-id="summer">Plant tomatoes and peppers</p>
```

上記の `<p>` タグには、それぞれ `data-id` 属性が含まれている点に注意してください。 このようにすると、チェック ボックス ノート シールの更新が簡単になります。 たとえば、次に示す要求では、春植え (spring planting) の To Do 項目に完了のマークを付けます。

```json
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: application/json
Authorization: Bearer {token}

[
   {
    'target':'#spring',
    'action':'replace',
    'content':'<p data-tag="to-do:completed"  data-id="spring">Plant peas and spinach</p>'
  }
]
```

次の要求は、すべての[組み込みノート シール](#built-in-note-tags-for-onenote)を含んだページを作成します。

```html 
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages

Content-Type: text/html
Authorization: Bearer {token}


<!DOCTYPE html>
<html>
  <head>
    <title data-tag="to-do:completed">All built-in note tags</title>
  </head>
  <body>
    <h1 data-tag="important">Paragraphs with built-in note tags</h1>
    <p data-tag="to-do">to-do</p>
    <p data-tag="important">important</p>
    <p data-tag="question">question</p>
    <p data-tag="definition">definition</p>
    <p data-tag="highlight">highlight</p>
    <p data-tag="contact">contact</p>
    <p data-tag="address">address</p>
    <p data-tag="phone-number">phone-number</p>
    <p data-tag="web-site-to-visit">web-site-to-visit</p>
    <p data-tag="idea">idea</p>
    <p data-tag="password">password</p>
    <p data-tag="critical">critical</p>
    <p data-tag="project-a">project-a</p>
    <p data-tag="project-b">project-b</p>
    <p data-tag="remember-for-later">remember-for-later</p>
    <p data-tag="movie-to-see">movie-to-see</p>
    <p data-tag="book-to-read">book-to-read</p>
    <p data-tag="music-to-listen-to">music-to-listen-to</p>
    <p data-tag="source-for-article">source-for-article</p>
    <p data-tag="remember-for-blog">remember-for-blog</p>
    <p data-tag="discuss-with-person-a">discuss-with-person-a</p>
    <p data-tag="discuss-with-person-b">discuss-with-person-b</p>
    <p data-tag="discuss-with-manager">discuss-with-manager</p>
    <p data-tag="send-in-email">send-in-email</p>
    <p data-tag="schedule-meeting">schedule-meeting</p>
    <p data-tag="call-back">call-back</p>
    <p data-tag="to-do-priority-1">to-do-priority-1</p>
    <p data-tag="to-do-priority-2">to-do-priority-2</p>
    <p data-tag="client-request">client-request</p>
    <h1 data-tag="important">Paragraphs with check boxes marked with "completed" status</h1>
    <p data-tag="to-do:completed">to-do:completed</p>
    <p data-tag="discuss-with-person-a:completed">discuss-with-person-a:completed</p>
    <p data-tag="discuss-with-person-b:completed">discuss-with-person-b:completed</p>
    <p data-tag="discuss-with-manager:completed">discuss-with-manager:completed</p>
    <p data-tag="schedule-meeting:completed">schedule-meeting:completed</p>
    <p data-tag="call-back:completed">call-back:completed</p>
    <p data-tag="to-do-priority-1:completed">to-do-priority-1:completed</p>
    <p data-tag="to-do-priority-2:completed">to-do-priority-2:completed</p>
    <p data-tag="client-request:completed">client-request:completed</p>
    <h1 data-tag="important">Multiple note tags</h1>
    <p data-tag="project-a,  client-request:completed">Two note tags:  project-a, client-request:completed</p>
    <p data-tag="idea, send-in-email, question">Three note tags:  idea, send-in-email, question</p>
    <h1 data-tag="important">Using note tags with other elements</h1>
    <p><b>Note tag on a list item:</b></p>
    <ul>
      <li data-tag="to-do-priority-1:completed">Make a to-do list</li>
    </ul>
    <p><b>Note tag on an image:</b></p>
    <img data-tag="source-for-article" src="https://placecorgi.com/200" />
    <p><b>Note tag with embedded style:</b></p>
    <p data-tag="important">Next time, <b>don't</b> forget to invite <span style="background-color:yellow">Dan</span>.</p>
  </body>
</html>
``` 

ページ作成の詳細については、「[OneNote ページの作成」を参照してください。ページ更新の詳細については、「OneNote ページの更新](onenote-create-page.md)」を参照してください。 ページ作成の詳細については、「OneNote ページの作成」を参照してください。ページ更新の詳細については、「[OneNote ページの更新](onenote-update-page.md)」を参照してください。


<a name="note-tags-lists"></a>

## <a name="note-tags-on-lists"></a>リストのノート シール

リストのノート シールの処理方法に関するいくつかのガイドラインを次に示します。

- Use `p` elements for to-do lists. To Do リストには p 要素を使用します。この要素は段落記号や行番号を表示しません。また、簡単に更新できます。

- すべてのリスト項目に対して**同じ**ノート シールを表示するリストを作成または更新する場合は、`ul` または `ol` に `data-tag` を定義します。 リスト全体を更新するには、`data-tag` または `ul` に `ol` を再定義する必要があります。

- 一部またはすべてのリストアイテムに**固有**のノートシールを表示するリストを作成また`data-tag`は`li`更新するには、要素`li`を定義し`ul` 、 `ol`要素をまたはにネストしないようにします。 リスト全体を更新するには、出力 HTML で返さ`ul`れたを削除し、ネスト`li`されていない要素のみを指定する必要があります。

- 特定`li`の要素を更新するに`li`は、要素を個別`data-tag`にターゲット`li`にして、要素にを定義します。 個別に処理された `li` 要素は、元のリストがどのように定義されていても、一意のノート シールを表示するように更新できます。

  ガイドラインは、Microsoft Graph によって適用される次の規則に基づいています。

  - The `data-tag` setting for a `ul` or `ol` overrides all settings on child `li` elements. ul`ul` または ol`ol` の data-tag`data-tag` の設定は、子の li`li` 要素ですべての設定を上書きします。これは、ul または ol は data-tag を指定しないが、その子の li 要素は指定する場合でも適用されます。

    For example, if you create a `ul` or `ol` that defines `data-tag="project-a"`, all its list items will display the *Project A* note tag. Or if the `ul` or `ol` doesn't define a `data-tag`, none of its items will display a note tag. This override happens regardless of any explicit settings on child `li` elements.

- 以下の条件下では、固有の data-tag`data-tag` 設定がリスト項目に適用されます。

  - 作成または更新要求では、li`li` 要素が ul`ul` や ol`ol` で入れ子になることはありません。

  - 更新要求では、li`li` 要素が個別に処理されます。

- 入力 HTML で送信される、入れ子になっていないli`li` 要素は、出力 HTML では ul`ul` で返されます。

- 出力 HTML では、すべての data-tag`data-tag` リストの設定はリスト項目の span`span` 要素で定義されます。


次のコードは、これらの規則の一部がどのように適用されるかを示しています。入力 HTML は、ノート シールが含まれる 2 つのリストを作成します。出力 HTML は、ページ コンテンツを取得するときに返されるリストです。

#### <a name="input-html"></a>入力 HTML

```html 
<!--To display the same note tag on all list items, define note tags on the ul or ol.--> 
<ul data-tag="project-a" data-id="agenda">
  <li>An item with a Project A note tag</li>
  <li>An item with a Project A note tag</li>
</ul>

<!--To display unique note tags on list items, don't nest li elements in a ul or ol.--> 
<li data-tag="idea" data-id="my-idea">An item with an Idea note tag</li>
<li data-tag="question" data-id="my-question">An item with a Question note tag</li>
```
 
#### <a name="output-html"></a>出力 HTML

```html 
<ul>
  <li><span data-tag="project-a">An item with a Project A note tag</span></li>
  <li><span data-tag="project-a">An item with a Project A note tag</span></li>
</ul>
<br />
<ul>
  <li style="..."><span data-tag="idea">An item with an Idea note tag</span></li>
  <li style="..."><span data-tag="question">An item with a Question note tag</span></li>
</ul>
```

<a name="output-html"></a>

## <a name="retrieve-note-tags"></a>ノート シールの取得

ページのコンテンツを取得する場合、組み込みのノート シールは出力 HTML に含まれています。

`GET ../api/v1.0/pages/{page-id}/content` 

出力`data-tag` HTML 内の属性には、常に図形の値が含まれており、[完了] に設定されているチェックボックスノートシールを表す場合は状態のみが含まれます。 次の例は、いくつかのノートシールを作成するために使用される入力 html と、返される出力 html を示しています。

#### <a name="input-html"></a>入力 HTML

```html 
<h1>Status meeting</h1>
<p data-tag="important">Next week's meeting has been moved to <b>Wednesday</b>.</p>
<p data-tag="question">What are the exact dates for the conference?</p>
<p>Upcoming training opportunities. See Katie for more info.</p>
<p data-tag="project-a">Around the room updates.</p>
<ul data-tag="critical">
  <li>Design handouts</li>
  <li>Plan keynote</li>
</ul>
```

#### <a name="output-html"></a>出力 HTML

```html 
<h1 style="...">Status meeting</h1>
<p data-tag="important">Next week's meeting has been moved to <span style="font-weight:bold">Wednesday</span>.</p>
<p data-tag="question">What are the exact dates for the conference?</p>
<p>Upcoming training opportunities. See Katie for more info.</p>
<p data-tag="project-a">Around the room updates.</p>
<ul>
  <li><span data-tag="critical">Design handouts</span></li>
  <li><span data-tag="critical">Plan keynote</span></li>
</ul>
```

リスト レベルで定義されている data-tag`data-tag` 属性は、そのリスト項目にプッシュされます。リストとノート シールの併用の詳細については、「リストのノート シール」を参照してください。 リスト レベルで定義されている data-tag 属性は、そのリスト項目にプッシュされます。リストとノート シールの併用の詳細については、「[リストのノート シール](#note-tags-on-lists)」を参照してください。

> **注:** 出力 HTML では、[定義] ノートシールと [後で記憶] ノートシールの`data-tag="remember-for-later"`両方がとして返されます。 `title` 要素はノート シールの情報を返しません。




<a name="built-in-tags"></a>

## <a name="built-in-note-tags-for-onenote"></a>OneNote の組み込みノート シール

OneNote には、次に示す組み込みのノート シールが用意されています。

![All built-in note tags.](images/note-tags-all.png)

`data-tag`属性に割り当てることができる値を次の表に示します。 Custom tags are not supported.

||タグ||
|:---|:---|:-----|
|`shape[:status]` |`to-do`<br/><br/>`to-do:completed`|`important`|
|`question`|`definition`|`highlight`|
|`contact`|`address`|`phone-number`|
|`web-site-to-visit`|`idea`|`password`|
|`critical`|`project-a`|`project-b`|
|`remember-for-later`|`movie-to-see`|`book-to-read`|
|`music-to-listen-to`|`source-for-article`|`remember-for-blog`|
|`discuss-with-person-a`<br/><br/>`discuss-with-person-a:completed`|`discuss-with-person-b`<br/><br/>`discuss-with-person-b:completed`|`discuss-with-manager`<br/><br/>`discuss-with-manager:completed`|
|`send-in-email`|`schedule-meeting`<br/><br/>`schedule-meeting:completed`|`call-back`<br/><br/>`call-back:completed`|
|`to-do-priority-1`<br/><br/>`to-do-priority-1:completed`|`to-do-priority-2`<br/><br/>`to-do-priority-2:completed`|`client-request`<br/><br/>`client-request:completed`|


<a name="request-response-info"></a>

## <a name="response-information"></a>応答情報

Microsoft Graph は、応答で次の情報を返します。

| 応答データ | 説明 |  
|------|------|  
| 成功コード | 成功した POST 要求に対しては 201 HTTP ステータス コード、成功した PATCH 要求に対しては 204 HTTP ステータス コードが戻ります。 |  
| エラー | Microsoft Graph から返されることのある OneNote エラーに関する詳細については、「[Microsoft Graph の OneNote API のエラー コード](onenote-error-codes.md)」を参照してください。 |  


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

アクセス許可のスコープと動作のしくみの詳細については、「[OneNote のアクセス許可のスコープ](permissions-reference.md)」を参照してください。


<a name="see-also"></a>

## <a name="see-also"></a>関連項目

- [OneNote ページを作成する](onenote-create-page.md)
- [OneNote ページ コンテンツを更新する](onenote-update-page.md)
- [OneNote との統合](integrate-with-onenote.md)
- [OneNote の開発者ブログ](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Stack Overflow 掲載の OneNote の開発に関する質問](https://go.microsoft.com/fwlink/?LinkID=390182)
- [OneNote GitHub のリポジトリ](https://go.microsoft.com/fwlink/?LinkID=390178)  
 


