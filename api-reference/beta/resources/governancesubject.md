---
title: governanceSubject リソースの種類
description: ユーザー、グループ、および権限を持つユーザー情報管理 (PIM) では管理されているサービス ・ プリンシパルを表します。
localization_priority: Normal
ms.openlocfilehash: a83825a147429c81b3e83b2f2fb384672d2f527e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519165"
---
# <a name="governancesubject-resource-type"></a>governanceSubject リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザー、グループ、および権限を持つユーザー情報管理 (PIM) では管理されているサービス ・ プリンシパルを表します。


## <a name="properties"></a>プロパティ
| プロパティ  | 型       |説明|
|:----------|:----------|:----------|
|id         |String     | サブジェクトの id です。|
|type       |String     |サブジェクトの種類。 値は、 ``User``、``Group``と``ServicePrincipal``。|
|displayName|String     |件名の表示名です。|
|email      |String     |ユーザーのサブジェクトの電子メール アドレスです。 件名は、他の種類では、空であるか。|
|principalName|String   |ユーザーのサブジェクトのプリンシパルの名前です。 件名は、他の種類では、空であるか。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSubject"
}-->

```json
{
  "id": "String",  
  "displayName": "String",
  "email": "String",
  "principalName": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancesubject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
