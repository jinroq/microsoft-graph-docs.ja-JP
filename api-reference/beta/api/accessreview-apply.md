---
title: AccessReview を適用します。
description: 'Azure AD のレビュー機能にアクセス、完成した accessReview の決定を適用します。  ターゲット オブジェクトは、1 回限りのアクセスの確認、または定期的なアクセス確認のインスタンスのいずれかにできます。  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e230a9638e865fbca69448f3a7683b95db954598
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951335"
---
# <a name="apply-accessreview"></a>AccessReview を適用します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、完成した[accessReview](../resources/accessreview.md)の決定を適用します。  ターゲット オブジェクトは、1 回限りのアクセスの確認、または定期的なアクセス確認のインスタンスのいずれかにできます。  


アクセス確認が完了したら、いずれかの終了日に到達したか、または管理者が手動で停止しているし、自動適用ためにでしたように構成されて、確認のため、変更を適用する適用を呼び出すことができます。 適用が行われるまでアクセス権を削除するのには意思決定には表示されませんソース リソースをユーザーがインスタンスにそれらのグループ メンバーシップを保持します。 呼び出すことによって適用、レビューの結果は、グループまたはアプリケーションを更新することによって実装されています。 ユーザーのアクセスが拒否された場合、レビューに管理者は、この API を呼び出すときに、Azure の AD は、メンバーシップ、またはアプリケーションの割り当てを削除します。 

アクセス確認が終了したら、自動適用後に構成していたレビューのステータスが完了から、中間の状態が変更され、最後に適用の状態に変更されます。 ことは、数分後にアプリケーションまたはメンバーシップの割り当てをグループ化は、リソースから削除されている場合に、拒否されたユーザーを参照してください。

レビューを適用するか、適用を選択すると、構成されている自動設置ディレクトリ内から発信されたグループまたは動的グループに影響がありません。 設置型の作成元のグループを変更する場合は、結果をダウンロードし、そのディレクトリ内のグループの形式にこれらの変更を適用します。


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
| 名前         | 種類        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー\{トークン\}。 必須。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。


## <a name="response"></a>応答
成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="see-also"></a>関連項目

- [アクセス確認を実行する方法](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a>例
##### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/applyDecisions()
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
  "description": "Apply accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
