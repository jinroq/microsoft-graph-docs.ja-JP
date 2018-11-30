---
title: plannerChecklistItems リソースの種類
description: '**plannerChecklistItemCollection** リソースは、タスクのチェックリスト項目のコレクションを表します。これは、オープン型です。タスクの詳細オブジェクトの一部です。プロパティ/値の組の値は、checklistItem オブジェクトです。'
ms.openlocfilehash: 3a08fe5bea1c7aaf493500b503e9ff85dc460acc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023196"
---
# <a name="plannerchecklistitems-resource-type"></a><span data-ttu-id="538c4-106">plannerChecklistItems リソースの種類</span><span class="sxs-lookup"><span data-stu-id="538c4-106">plannerChecklistItems resource type</span></span>

<span data-ttu-id="538c4-p102">**plannerChecklistItemCollection** リソースは、タスクのチェックリスト項目のコレクションを表します。これは、オープン型です。[タスクの詳細](plannertaskdetails.md)オブジェクトの一部です。プロパティ/値の組の値は、[checklistItem](plannerchecklistitem.md) オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="538c4-p102">The **plannerChecklistItemCollection** resource represents the collection of checklist items on a task. It is an Open Type. It is part of the [task details](plannertaskdetails.md) object. The value in the property-value pair is the [checklistItem](plannerchecklistitem.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="538c4-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="538c4-111">Properties</span></span>
<span data-ttu-id="538c4-p103">クライアントは、オープン型のプロパティを定義できます。この場合、クライアントは **GUID** をプロパティとして指定し、その値は [checklistItem](plannerchecklistitem.md) オブジェクトでなければなりません。以下に例を示します。チェックリストの項目を削除するには、プロパティの値を `null` に設定します。</span><span class="sxs-lookup"><span data-stu-id="538c4-p103">Properties of an Open Type can be defined by the client. In this case, the client should provide **GUIDs** as properties and their values must be [checklistItem](plannerchecklistitem.md) objects. Example is shown below. To remove an item in the checklist, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="538c4-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="538c4-116">JSON representation</span></span>

<span data-ttu-id="538c4-117">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="538c4-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
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
<span data-ttu-id="538c4-118">// 例</span><span class="sxs-lookup"><span data-stu-id="538c4-118">// Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItems resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->