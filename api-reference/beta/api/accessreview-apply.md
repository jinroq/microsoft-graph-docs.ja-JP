---
title: AccessReview を適用する
description: 'Azure AD access レビュー機能で、完了した accessReview の決定を適用します。  ターゲットオブジェクトは、1回限りのアクセスレビュー、または定期的なアクセスレビューのインスタンスのいずれかになります。  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c8327e8ebc24ed2e4c278117a7e271b89c6d4629
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440135"
---
# <a name="apply-accessreview"></a>AccessReview を適用する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、完了した[accessreview](../resources/accessreview.md)の決定を適用します。  ターゲットオブジェクトは、1回限りのアクセスレビュー、または定期的なアクセスレビューのインスタンスのいずれかになります。  


終了日に達したか、管理者が手動で停止したためにアクセスレビューが終了し、レビューのために自動適用が構成されていない場合は、[適用] を呼び出して変更を適用できます。 適用が行われるまで、アクセス権を削除するための決定はソースリソースに表示されず、インスタンスのユーザーはグループメンバーシップを保持します。 [適用] を呼び出すと、レビューの結果が、グループまたはアプリケーションを更新することによって実装されます。 ユーザーのアクセスがレビューで拒否された場合、管理者がこの API を呼び出すと、Azure AD はそれらのメンバーシップまたはアプリケーション割り当てを削除します。 

アクセスレビューが完了し、自動適用が構成されると、レビューの状態は [完了] から [中間状態] に変わり、最後に [適用済みの状態] に変わります。 却下されたユーザーが存在する場合は、リソースグループのメンバーシップまたはアプリの割り当てから数分で削除されることを確認する必要があります。

構成済みの自動適用レビュー、または [適用] を選択しても、オンプレミスディレクトリまたは動的グループで発生するグループには影響しません。 オンプレミスで発生したグループを変更する場合は、結果をダウンロードして、そのディレクトリ内のグループの表現にその変更を適用します。


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
POST /accessReviews('<id>')/applyDecisions()
```
## <a name="request-headers"></a>要求ヘッダー
| 名前         | 型        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー \{トークン\}。必須。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。


## <a name="response"></a>応答
成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="see-also"></a>関連項目

- [アクセスレビューを完了する方法](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a>例
##### <a name="request"></a>要求

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/applyDecisions
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/apply-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/apply-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/apply-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>応答
>**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Apply accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
