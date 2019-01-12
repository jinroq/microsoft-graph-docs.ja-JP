---
title: educationSchool リソースの種類
description: '学校。 現時点で、**educationSchool** リソースは administrativeUnit リソースと一致していて、同じ ID を共有しています。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 17a5c3ad2f28e802bb6cad3a97d1cb723b3407d6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918246"
---
# <a name="educationschool-resource-type"></a>educationSchool リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

学校。 現時点で、**educationSchool** リソースは [administrativeUnit](administrativeunit.md) リソースと一致していて、同じ ID を共有しています。  

このリソースは、[educationOrganization](educationorganization.md) のサブタイプです。




## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get](../api/educationschool-get.md) | [educationSchool](educationschool.md) |**educationSchool** オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Add class](../api/educationschool-post-classes.md) |[educationClass](educationclass.md)| classes ナビゲーション プロパティに投稿することで、学校の新しい **educationClass** を追加します。|
|[List classes](../api/educationschool-list-classes.md) |[educationClass](educationclass.md) コレクション| **educationClass** オブジェクト コレクションを取得します。|
|[Remove class](../api/educationschool-delete-classes.md) |[educationClass](educationclass.md)| classes ナビゲーション プロパティによって、学校から **educationClass** を削除します。|
|[Add user](../api/educationschool-post-users.md) |[educationUser](educationuser.md)| **users** ナビゲーション プロパティを投稿することで、学校の新しい **educationUser** を追加します。|
|[List users](../api/educationschool-list-users.md) |[educationUser](educationuser.md) コレクション| **educationUser** オブジェクト コレクションを取得します。|
|[Remove user](../api/educationschool-delete-users.md) |[educationUser](educationuser.md)| **users** ナビゲーション プロパティによって、学校から **educationUser** を削除します。|
|[Get administrativeUnit](../api/educationschool-get-administrativeunit.md) |[administrativeUnit](administrativeunit.md)| この **educationSchool** に対応する **administrativeUnit** を取得します。|
|[Update](../api/educationschool-update.md) | [educationSchool](educationschool.md) |**educationSchool** オブジェクトを更新します。 |
|[Delete](../api/educationschool-delete.md) | なし |**educationSchool** オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|ID|String|この学校の GUID。|
|displayName| String| 学校の表示名。| 
|説明| String | 学校の説明。| 
|status| 文字列| 読み取り専用。 使用可能な値: `inactive`、`active`、`expired`、`deleteable`。|
|externalSource| 文字列| 読み取り専用。  使用可能な値: `sis`、`manual`、`unknownFutureValue`。|
|principalEmail| String| プリンシパルの電子メール アドレス。|
|principalName| String | プリンシパルの名前。|
|externalPrincipalId| String | 同期システム内のプリンシパルの ID。 |
|highestGrade|String| 授業を受けている最高学年。 |
|lowestGrade|String| 授業を受けている最低学年。 |
|schoolNumber|String| 学校番号。|
|externalId|String| 同期システム内の学校の ID。 |
|phone|String| 学校の電話番号。 |
|fax|String| 学校の FAX 番号。 |
|address|[physicalAddress](physicaladdress.md)| 学校の住所。|
|createdBy|[identitySet](identityset.md)|学校を作成したエンティティ。|


## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|classes|[educationClass](educationclass.md) コレクション| 学校で授業しているクラス。 Null 許容型。|
|users|[educationUser](educationuser.md) コレクション| 学校のユーザー。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSchool"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "highestGrade": "String",
  "lowestGrade": "String",
  "schoolNumber": "String",
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalId": "String",
  "fax": "String",
  "phone": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
