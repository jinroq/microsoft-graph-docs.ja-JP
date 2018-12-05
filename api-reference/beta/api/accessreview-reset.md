---
title: AccessReview をリセットします。
description: Azure AD アクセスでは、レビュー機能は、現在アクティブな accessReview の決定をリセットします。  ターゲット オブジェクトは、1 回限りのアクセスの確認、または定期的なアクセス確認のインスタンスのいずれかにできます。  以前の決定は記録されなくが、校閲者が意思決定を更新するのには続行できます。
ms.openlocfilehash: b633a56926b56b33c509214d7574971056831967
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067683"
---
# <a name="reset-accessreview"></a>AccessReview をリセットします。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Azure AD では、 [access](../resources/accessreviews-root.md)の機能は、現在アクティブな[accessReview](../resources/accessreview.md)の決定をリセットします。  ターゲット オブジェクトは、1 回限りのアクセスの確認、または定期的なアクセス確認のインスタンスのいずれかにできます。  以前の決定は記録されなくが、校閲者が意思決定を更新するのには続行できます。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | AccessReview.ReadWrite.All |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/resetDecisions()
```
## <a name="request-headers"></a>要求ヘッダー
| 名前         | 型        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー\{トークン\}。 必須。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。


## <a name="response"></a>応答
成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例
##### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/resetDecisions()
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Reset accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->