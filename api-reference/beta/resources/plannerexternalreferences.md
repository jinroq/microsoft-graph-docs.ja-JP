---
title: プランリソースの種類
description: "\" **plan/外部参照**\" リソースは、タスクに対する参照のコレクションを表します。 これはオープン型です。 タスクの詳細オブジェクトの一部です。 プロパティと値のペアの値は、externalreference オブジェクトです。"
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 6684757b9eb8b1d05a738b5aed887a05e8f32cb3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344514"
---
# <a name="plannerexternalreferences-resource-type"></a>プランリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

" **plan/外部参照**" リソースは、タスクに対する参照のコレクションを表します。 これはオープン型です。 [タスクの詳細](plannertaskdetails.md)オブジェクトの一部です。 プロパティと値のペアの値は、 [externalreference](plannerexternalreference.md)オブジェクトです。


## <a name="properties"></a>プロパティ
オープン型のプロパティは、クライアントで定義できます。 この場合、クライアントは**HTTP/HTTPS**プロトコルに基づいた**有効な url**をプロパティとして提供する必要があり、それらの値は[externalreference](plannerexternalreference.md)オブジェクトである必要があります。 OData に基づいて、オープン型のプロパティ名に次の文字を`.`含める`:`こと`%`はできません。つまり、をエンコードする必要があります。 例を以下に示します。 参照を削除するには、プロパティの値をに`null`設定します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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

例

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerExternalReferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
