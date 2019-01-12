---
title: plannerExternalReferences リソースの種類
description: '**PlannerExternalReferences** リソースは、タスク上での参照のコレクションを表します。これはオープン型です。タスクの詳細オブジェクトの一部です。プロパティ/値の組の値は、externalReference オブジェクトです。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 8048a8a412935cc69e805a1d7c77ff8b1fbf5f7c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974659"
---
# <a name="plannerexternalreferences-resource-type"></a><span data-ttu-id="b1dfa-106">plannerExternalReferences リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b1dfa-106">plannerExternalReferences resource type</span></span>

<span data-ttu-id="b1dfa-p102">**PlannerExternalReferences** リソースは、タスク上での参照のコレクションを表します。これはオープン型です。[タスクの詳細](plannertaskdetails.md)オブジェクトの一部です。プロパティ/値の組の値は、[externalReference](plannerexternalreference.md) オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b1dfa-p102">The **plannerExternalReferences** resource represents the collection of references on a task. This is an Open Type. It is part of the [task details](plannertaskdetails.md) object. The value in the property-value pair is the [externalReference](plannerexternalreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="b1dfa-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1dfa-111">Properties</span></span>
<span data-ttu-id="b1dfa-p103">クライアントは、オープン型のプロパティを定義できます。この例では、プロパティとその値を [externalReference](plannerexternalreference.md) オブジェクトにする必要があるため、クライアントは **HTTP/HTTPS** プロトコルに基づいて **有効な URL** を指定する必要があります。OData に基づき、オープン型のプロパティ名には、`.`、`:`、`%` の文字を含めることができないため、エンコードする必要があります。以下に例を示します。参照を削除するには、プロパティの値を `null` に設定します。</span><span class="sxs-lookup"><span data-stu-id="b1dfa-p103">Properties of an Open Type can be defined by the client. In this case, the client must provide **valid URLs** based on the **HTTP/HTTPS** protocols as properties and their values must be the [externalReference](plannerexternalreference.md) objects. Based on OData, property names in Open Types cannot contain the following characters: `.`, `:`, `%`  so they need to be encoded. Example is shown below. To remove a reference, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1dfa-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b1dfa-117">JSON representation</span></span>

<span data-ttu-id="b1dfa-118">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b1dfa-118">Here is a JSON representation of the resource</span></span>

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

<span data-ttu-id="b1dfa-119">// 例</span><span class="sxs-lookup"><span data-stu-id="b1dfa-119">// Example</span></span>

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
