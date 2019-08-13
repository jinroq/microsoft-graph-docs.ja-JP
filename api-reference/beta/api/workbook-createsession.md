---
title: セッションを作成する
description: 'この API を使用して、新しいブック セッションを作成します。 '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d967a8723d0e082cf1e570ae8d7416b1265f6335
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362026"
---
# <a name="create-session"></a>セッションを作成する

この API を使用して、新しいブック セッションを作成します。 

2 つのモードのいずれかで、Excel API を呼び出すことができます。 

1. 永続セッション - ブックに加えられたすべての変更は永続化 (保存) されます。これは通常の操作モードです。 
2. 非永続セッション - API によって加えられた変更は元の場所に保存されません。代わりに、その特定の API セッション中に加えられた変更を反映するファイルの一時コピーが Excel のバックエンド サーバーに保持されます。Excel のセッションの有効期限が切れると、変更は失われます。分析を行ったり、計算の結果やグラフのイメージを取得したりする必要があるものの、ドキュメントの状態には影響を与えないアプリには、このモードが便利です。   

API でセッションを表すには、`workbook-session-id: {session-id}` ヘッダーを使用します。 

>**注:** セッション ヘッダーは Excel API が機能するために必要ではありません。しかし、パフォーマンスを向上させるためにセッション ヘッダーを使用することをお勧めします。セッション ヘッダーを使用しない場合は、API の呼び出し時に行われた変更がファイルに永続化_されます_。  

## <a name="error-handling"></a>エラー処理

この要求に対して、504 HTTP エラーが表示されることがあります。 このエラーに対する適切な対応は、要求を繰り返すことです。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.ReadWrite    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/createSession

```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、[WorkbookSessionInfo](../resources/workbooksessioninfo.md) オブジェクトの JSON 表記を指定します。

## <a name="response"></a>応答

成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [WorkbookSessionInfo](../resources/workbooksessioninfo.md) オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistChanges": true
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-excel-session-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

要求本文で、[WorkbookSessionInfo](../resources/workbooksessioninfo.md) オブジェクトの JSON 表記を指定します。

##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookSessionInfo"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistChanges": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
