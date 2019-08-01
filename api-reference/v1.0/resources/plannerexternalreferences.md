---
title: プランリソースの種類
description: "\" **Plan/外部参照**\" リソースは、タスクに対する参照のコレクションを表します。 これはオープン型です。 タスクの詳細オブジェクトの一部です。 プロパティと値のペアの値は、externalReference オブジェクトです。"
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 35e26aaf13686a030d35d5d75ec3c99c8df93a6a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035225"
---
# <a name="plannerexternalreferences-resource-type"></a><span data-ttu-id="0242e-106">プランリソースの種類</span><span class="sxs-lookup"><span data-stu-id="0242e-106">plannerExternalReferences resource type</span></span>

<span data-ttu-id="0242e-107">" **Plan/外部参照**" リソースは、タスクに対する参照のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="0242e-107">The **plannerExternalReferences** resource represents the collection of references on a task.</span></span> <span data-ttu-id="0242e-108">これはオープン型です。</span><span class="sxs-lookup"><span data-stu-id="0242e-108">This is an Open Type.</span></span> <span data-ttu-id="0242e-109">[タスクの詳細](plannertaskdetails.md)オブジェクトの一部です。</span><span class="sxs-lookup"><span data-stu-id="0242e-109">It is part of the [task details](plannertaskdetails.md) object.</span></span> <span data-ttu-id="0242e-110">プロパティと値のペアの値は、 [Externalreference](plannerexternalreference.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0242e-110">The value in the property-value pair is the [externalReference](plannerexternalreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="0242e-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0242e-111">Properties</span></span>
<span data-ttu-id="0242e-112">オープン型のプロパティは、クライアントで定義できます。</span><span class="sxs-lookup"><span data-stu-id="0242e-112">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="0242e-113">この場合、クライアントは**HTTP/HTTPS**プロトコルに基づいた**有効な url**をプロパティとして提供する必要があり、それらの値は[externalreference](plannerexternalreference.md)オブジェクトである必要があります。</span><span class="sxs-lookup"><span data-stu-id="0242e-113">In this case, the client must provide **valid URLs** based on the **HTTP/HTTPS** protocols as properties and their values must be the [externalReference](plannerexternalreference.md) objects.</span></span> <span data-ttu-id="0242e-114">OData に基づいて、オープン型のプロパティ名に次の文字を`.`含める`:`こと`%`はできません。つまり、をエンコードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0242e-114">Based on OData, property names in Open Types cannot contain the following characters: `.`, `:`, `%`  so they need to be encoded.</span></span> <span data-ttu-id="0242e-115">例を以下に示します。</span><span class="sxs-lookup"><span data-stu-id="0242e-115">Example is shown below.</span></span> <span data-ttu-id="0242e-116">参照を削除するには、プロパティの値をに`null`設定します。</span><span class="sxs-lookup"><span data-stu-id="0242e-116">To remove a reference, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0242e-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0242e-117">JSON representation</span></span>

<span data-ttu-id="0242e-118">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="0242e-118">Here is a JSON representation of the resource</span></span>

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

<span data-ttu-id="0242e-119">例</span><span class="sxs-lookup"><span data-stu-id="0242e-119">// Example</span></span>

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
