---
title: plannerChecklistItems リソースの種類
description: '**Plan? Checklistitemcollection**リソースは、タスクのチェックリストアイテムのコレクションを表します。 オープンな種類です。 タスクの詳細オブジェクトの一部です。 プロパティと値のペアの値は、checklistItem オブジェクトです。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: bebec56f57f546dcfc0b16eedb1fb9635d0fb16f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966009"
---
# <a name="plannerchecklistitems-resource-type"></a><span data-ttu-id="185b1-106">plannerChecklistItems リソースの種類</span><span class="sxs-lookup"><span data-stu-id="185b1-106">plannerChecklistItems resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="185b1-107">**Plan? Checklistitemcollection**リソースは、タスクのチェックリストアイテムのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="185b1-107">The **plannerChecklistItemCollection** resource represents the collection of checklist items on a task.</span></span> <span data-ttu-id="185b1-108">オープンな種類です。</span><span class="sxs-lookup"><span data-stu-id="185b1-108">It is an Open Type.</span></span> <span data-ttu-id="185b1-109">[タスクの詳細](plannertaskdetails.md)オブジェクトの一部です。</span><span class="sxs-lookup"><span data-stu-id="185b1-109">It is part of the [task details](plannertaskdetails.md) object.</span></span> <span data-ttu-id="185b1-110">プロパティと値のペアの値は、 [Checklistitem](plannerchecklistitem.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="185b1-110">The value in the property-value pair is the [checklistItem](plannerchecklistitem.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="185b1-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="185b1-111">Properties</span></span>
<span data-ttu-id="185b1-112">オープン型のプロパティは、クライアントで定義できます。</span><span class="sxs-lookup"><span data-stu-id="185b1-112">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="185b1-113">この場合、クライアントは**guid**をプロパティとして提供し、それらの値は[checklistitem](plannerchecklistitem.md)オブジェクトである必要があります。</span><span class="sxs-lookup"><span data-stu-id="185b1-113">In this case, the client should provide **GUIDs** as properties and their values must be [checklistItem](plannerchecklistitem.md) objects.</span></span> <span data-ttu-id="185b1-114">例を以下に示します。</span><span class="sxs-lookup"><span data-stu-id="185b1-114">Example is shown below.</span></span> <span data-ttu-id="185b1-115">チェックリストの項目を削除するには、プロパティの値をに`null`設定します。</span><span class="sxs-lookup"><span data-stu-id="185b1-115">To remove an item in the checklist, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="185b1-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="185b1-116">JSON representation</span></span>

<span data-ttu-id="185b1-117">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="185b1-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItems"
}-->

```json
{
  "String-value":
  {
    "isChecked": true,
    "lastModifiedBy": "String-value",
    "lastModifiedByDateTime": "String(timestamp)",
    "orderHint": "String-value",
    "title": "String-value"
  }
}
```
<span data-ttu-id="185b1-118">例</span><span class="sxs-lookup"><span data-stu-id="185b1-118">// Example</span></span>

```json
{
  "3a73c9dd-fb47-4230-9c0f-b80788fb0f9b": // client-generated GUID
  {
    "@odata.type": "microsoft.graph.checklistItem", // required in PATCH requests to edit the checklist on a task
    "isChecked": true,
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedByDateTime": "2015-09-21T17:45:12.039Z",
    "orderHint": "0009005756397228702",
    "title": "Get stamps"
  },
  "5f36f5b2-1ec0-4c48-9c75-ed59429516c5":
  {
     "@odata.type": "microsoft.graph.checklistItem",
    "isChecked": false,
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedByDateTime": "2015-09-21T17:45:12.039Z",
    "orderHint": "0004105723397228784",
    "title": "Mail card at UPS"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerChecklistItems resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
