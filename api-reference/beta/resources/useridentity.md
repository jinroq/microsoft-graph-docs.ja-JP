---
title: 型を割り当てられていません
description: 'Azure AD のレビューにアクセスして、この型は、アクセス レビューのレビュー担当者の Azure AD ユーザー id を表します。  '
ms.openlocfilehash: 6cbbe7aa017572bcd753a57edbf82751ac4986a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069480"
---
# <a name="useridentity-type"></a>型を割り当てられていません

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Azure AD[アクセスの確認](accessreviews-root.md)をするは、この型は、アクセス レビューのレビュー担当者の Azure AD ユーザー id を表します。  
Azure AD の監査ログのコンテキストでは、開始、または監査活動の影響を受けたユーザーの情報を表します。

このタイプは、[アイデンティティ](identity.md)を継承し、追加の 1 つのプロパティ、ユーザーのユーザー プリンシパル名を持ちます。

## <a name="methods"></a>メソッド

なし  要求の本文にこの型のオブジェクトを含めますと[、accessReview を作成](../api/accessreview-create.md)します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| `displayName` | `String` | Id の表示名です。 このできない可能性がある利用可能なまたは最新の状態に注意してください。    |
| `id`          | `String` | ID の一意識別子。  |
| `ipAddress`| `String`| アクティビティ (監査ログのみ) を実行するユーザーによって使用されるクライアントの IP アドレスを示します。|
| `userPrincipalName`|`String` | ユーザーの userPrincipalName 属性です。 |

## <a name="remarks"></a>注釈

状況によっては、アクターの一意識別子は利用できないことがあります。その場合、ID の **displayName** プロパティが返されますが、**id** プロパティはリソースから失われます。

## <a name="relationships"></a>リレーションシップ

なし。

## <a name="see-also"></a>関連項目

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[AccessReview のレビュー担当者を取得します。](../api/accessreview-listreviewers.md) |       コレクションを[割り当てられていません](useridentity.md)| AccessReview のレビュー担当者を取得します。 |
|[AccessReview の校閲者を追加します。](../api/accessreview-addreviewer.md) |      なし。   |   AccessReview には、レビュー担当者を追加します。 |
|[AccessReview のレビュー担当者を削除します。](../api/accessreview-removereviewer.md) | なし。  |   AccessReview からレビュー担当者を削除します。 |

## <a name="json-representation"></a>JSON 表記

ここでは、型の JSON 表現です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
"displayName", "thumbnails"
  ],
  "@odata.type": "microsoft.graph.userIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string",
 "userPrincipalName": "String"
}

```

<!-- {
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
