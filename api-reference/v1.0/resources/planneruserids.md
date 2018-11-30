---
title: plannerUserIds リソースの種類
description: '**PlannerUserIds**リソースは、plan を共有するユーザー ID のリストを表します。これはオープン型です。Office 365 グループを活用している場合は、グループの API を使用してグループのメンバーシップを管理し、グループの計画を共有します。グループの既存のメンバーもこのコレクションに追加できますが、このグループが所有する計画へのアクセスは必要とされません。'
ms.openlocfilehash: f2115cb31825f30190701bc2ab6b0d29669c4665
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024188"
---
# <a name="planneruserids-resource-type"></a>plannerUserIds リソースの種類

**PlannerUserIds**リソースは、[plan](plannerplan.md) を共有するユーザー ID のリストを表します。これはオープン型です。Office 365 グループを活用している場合は、グループの API を使用してグループのメンバーシップを管理し、[グループの](group.md)計画を共有します。グループの既存のメンバーもこのコレクションに追加できますが、このグループが所有する計画へのアクセスは必要とされません。


## <a name="properties"></a>プロパティ
クライアントは、オープン型のプロパティを定義できます。この例では、クライアントは、値が `true` ブール値となるプロパティとしてユーザー ID を指定する必要があります。ユーザー ID が共有されなくなると、プロパティはその値が `false` ブール値に設定され、自動的に削除されます。


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
  "@odata.type": "microsoft.graph.plannerUserIds"
}-->

```json
{
  "String-value": true
}
```

// 例
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->