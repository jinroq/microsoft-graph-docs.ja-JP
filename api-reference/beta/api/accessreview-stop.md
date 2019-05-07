---
title: AccessReview を停止する
description: Azure AD access レビュー機能で、現在アクティブな accessReview を停止します。  ターゲットオブジェクトは、1回限りのアクセスレビュー、または定期的なアクセスレビューのインスタンスのいずれかになります。  (定期的なアクセスレビューが今後のインスタンスを開始しないようにするには、それを更新して、スケジュールされた終了日を変更します)。  アクセスレビューが停止すると、レビュー担当者は入力を行うことができなくなり、アクセスレビューの決定を適用できるようになります。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d40d170269e930a242c2528b2bb161d210b78e34
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636738"
---
# <a name="stop-accessreview"></a>AccessReview を停止する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、現在アクティブな[accessreview](../resources/accessreview.md)を停止します。  ターゲットオブジェクトは、1回限りのアクセスレビュー、または定期的なアクセスレビューのインスタンスのいずれかになります。  (定期的なアクセスレビューが今後のインスタンスを開始しないようにするには、[それを更新して](accessreview-update.md)、スケジュールされた終了日を変更します)。  アクセスレビューが停止すると、レビュー担当者は入力を行うことができなくなり、アクセスレビューの決定を適用できるようになります。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | AccessReview.ReadWrite.All |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | サポートされていません。  |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/stop()
```
## <a name="request-headers"></a>要求ヘッダー
| 名前         | 型        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー \{トークン\}。必須。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。


## <a name="response"></a>応答
成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例
##### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/stop
```
##### <a name="response"></a>応答
>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/stop_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/stop_accessReview-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-stop.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-stop.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
