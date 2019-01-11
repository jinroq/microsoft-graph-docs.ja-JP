---
title: plannerExternalReferences リソースの種類
description: '**PlannerExternalReferences** リソースは、タスク上での参照のコレクションを表します。これはオープン型です。タスクの詳細オブジェクトの一部です。プロパティ/値の組の値は、externalReference オブジェクトです。'
localization_priority: Normal
ms.openlocfilehash: aedfd0321843c4a906defe22f184bac7d293a6e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862077"
---
# <a name="plannerexternalreferences-resource-type"></a>plannerExternalReferences リソースの種類

**PlannerExternalReferences** リソースは、タスク上での参照のコレクションを表します。これはオープン型です。[タスクの詳細](plannertaskdetails.md)オブジェクトの一部です。プロパティ/値の組の値は、[externalReference](plannerexternalreference.md) オブジェクトです。


## <a name="properties"></a>プロパティ
クライアントは、オープン型のプロパティを定義できます。この例では、プロパティとその値を [externalReference](plannerexternalreference.md) オブジェクトにする必要があるため、クライアントは **HTTP/HTTPS** プロトコルに基づいて **有効な URL** を指定する必要があります。OData に基づき、オープン型のプロパティ名には、`.`、`:`、`%` の文字を含めることができないため、エンコードする必要があります。以下に例を示します。参照を削除するには、プロパティの値を `null` に設定します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
  "@odata.type": "microsoft.graph.plannerExternalReferences"
}-->


```json
{
  "String-value":
  {
    "alias": "String-value",
    "lastModifiedBy": "String-value",
    "lastModifiedDateTime": "String(timestamp)",
    "previewPriority": "String-value",
    "type": "String-value"
  }
}
```

// 例

```json
{
  "https%3A//contoso%2Esharepoint%2Ecom/teams/agile/documents/AnnualReport%2Epptx":
  {
    "@odata.type": "microsoft.graph.externalReference", // required in PATCH requests to edit the references on a task
    "alias": "Agile Team Annual Report",
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedDateTime": "2015-09-21T17:45:12.039Z",
    "previewPriority": "0009005756397228702",
    "type": "PowerPoint"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
