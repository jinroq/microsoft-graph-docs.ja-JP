---
title: plannerChecklistItems リソースの種類
description: '**plan? checklistitemcollection**リソースは、タスクのチェックリストアイテムのコレクションを表します。 オープンな種類です。 タスクの詳細オブジェクトの一部です。 プロパティと値のペアの値は、checklistitem オブジェクトです。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 17c1d8c0529e0d85ebc784d25c2dc284f1775c0f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462285"
---
# <a name="plannerchecklistitems-resource-type"></a><span data-ttu-id="0ed1f-106">plannerChecklistItems リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0ed1f-106">plannerChecklistItems resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ed1f-107">**plan? checklistitemcollection**リソースは、タスクのチェックリストアイテムのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="0ed1f-107">The **plannerChecklistItemCollection** resource represents the collection of checklist items on a task.</span></span> <span data-ttu-id="0ed1f-108">オープンな種類です。</span><span class="sxs-lookup"><span data-stu-id="0ed1f-108">It is an Open Type.</span></span> <span data-ttu-id="0ed1f-109">[タスクの詳細](plannertaskdetails.md)オブジェクトの一部です。</span><span class="sxs-lookup"><span data-stu-id="0ed1f-109">It is part of the [task details](plannertaskdetails.md) object.</span></span> <span data-ttu-id="0ed1f-110">プロパティと値のペアの値は、 [checklistitem](plannerchecklistitem.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0ed1f-110">The value in the property-value pair is the [checklistItem](plannerchecklistitem.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="0ed1f-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ed1f-111">Properties</span></span>
<span data-ttu-id="0ed1f-112">オープン型のプロパティは、クライアントで定義できます。</span><span class="sxs-lookup"><span data-stu-id="0ed1f-112">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="0ed1f-113">この場合、クライアントは**guid**をプロパティとして提供し、それらの値は[checklistitem](plannerchecklistitem.md)オブジェクトである必要があります。</span><span class="sxs-lookup"><span data-stu-id="0ed1f-113">In this case, the client should provide **GUIDs** as properties and their values must be [checklistItem](plannerchecklistitem.md) objects.</span></span> <span data-ttu-id="0ed1f-114">例を以下に示します。</span><span class="sxs-lookup"><span data-stu-id="0ed1f-114">Example is shown below.</span></span> <span data-ttu-id="0ed1f-115">チェックリストの項目を削除するには、プロパティの値をに`null`設定します。</span><span class="sxs-lookup"><span data-stu-id="0ed1f-115">To remove an item in the checklist, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ed1f-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0ed1f-116">JSON representation</span></span>

<span data-ttu-id="0ed1f-117">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="0ed1f-117">Here is a JSON representation of the resource</span></span>

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
<span data-ttu-id="0ed1f-118">例</span><span class="sxs-lookup"><span data-stu-id="0ed1f-118">// Example</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerchecklistitems.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
