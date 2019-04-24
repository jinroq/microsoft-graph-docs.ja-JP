---
title: governanceSubject リソースの種類
description: 特権 id 管理 (PIM) で管理されているユーザー、グループ、およびサービスプリンシパルを表します。
localization_priority: Normal
ms.openlocfilehash: a83825a147429c81b3e83b2f2fb384672d2f527e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506435"
---
# <a name="governancesubject-resource-type"></a>governanceSubject リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特権 id 管理 (PIM) で管理されているユーザー、グループ、およびサービスプリンシパルを表します。


## <a name="properties"></a>プロパティ
| プロパティ  | 型       |説明|
|:----------|:----------|:----------|
|id         |String     | 件名の id。|
|type       |String     |件名の種類。 この値は、 ``User``、 ``Group``、と``ServicePrincipal``することができます。|
|displayName|String     |件名の表示名。|
|email      |String     |ユーザーの件名の電子メールアドレス。 件名が他の種類の場合は、空になります。|
|principalName|String   |ユーザーの件名のプリンシパル名。 件名が他の種類の場合は、空になります。|

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
