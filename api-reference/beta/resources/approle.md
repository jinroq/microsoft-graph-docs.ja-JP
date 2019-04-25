---
title: approle リソースの種類
description: 別のアプリケーションを呼び出しているクライアントアプリケーションによって要求されるか、または指定されたアプリケーションロールのユーザーまたはグループにアプリケーションを割り当てるために使用される可能性があるアプリケーションロールを表します。 serviceprincipal エンティティおよび application エンティティの**approles**プロパティは、 **approles**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 8a367406c64cf9d0d3da49716aeaf6ca3c1fa687
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535705"
---
# <a name="approle-resource-type"></a>approle リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

別のアプリケーションを呼び出しているクライアントアプリケーションによって要求されるか、または指定されたアプリケーションロールのユーザーまたはグループにアプリケーションを割り当てるために使用される可能性があるアプリケーションロールを表します。 [serviceprincipal](serviceprincipal.md)エンティティおよび[application](application.md)エンティティの**approles**プロパティは、 **approles**のコレクションです。

> 重要: この機能は現在のリリースでは無効になっています。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approle"
}-->

```json
{
  "allowedMemberTypes": ["string"],
  "description": "string",
  "displayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "value": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowedMemberTypes|String collection|"application" に設定するか、またはその両方に設定して、このアプリの役割定義をユーザーとグループに割り当てることができるようにするかどうかを指定します。 "User" に設定するか、または (デーモンサービスシナリオでこのアプリケーションにアクセスしている) 他のアプリケーションに割り当てます。|
|description|String|管理者アプリの割り当てと同意エクスペリエンスに表示されるアクセス許可ヘルプテキスト。|
|displayName|String|管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可の表示名。|
|id|Guid|approles コレクション内の**** 一意のロール識別子。|
|isEnabled|Boolean|ロール定義を作成または更新する場合は、 **true** (既定値) に設定する必要があります。 役割を削除するには、最初に**false**に設定する必要があります。  その時点で、以降の呼び出しでは、この役割が削除される可能性があります。|
|value|文字列|アプリケーションが認証トークンとアクセストークンで想定する必要があるロール要求の値を指定します。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/approle.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
