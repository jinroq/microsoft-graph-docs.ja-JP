---
title: plannerChecklistItems リソースの種類
description: '**plannerChecklistItemCollection** リソースは、タスクのチェックリスト項目のコレクションを表します。これは、オープン型です。タスクの詳細オブジェクトの一部です。プロパティ/値の組の値は、checklistItem オブジェクトです。'
localization_priority: Normal
ms.openlocfilehash: f958289e22ccc7515fe0e79145bba5fb5188e660
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858626"
---
# <a name="plannerchecklistitems-resource-type"></a><span data-ttu-id="56500-106">plannerChecklistItems リソースの種類</span><span class="sxs-lookup"><span data-stu-id="56500-106">plannerChecklistItems resource type</span></span>

> <span data-ttu-id="56500-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="56500-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56500-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56500-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="56500-p103">**plannerChecklistItemCollection** リソースは、タスクのチェックリスト項目のコレクションを表します。これは、オープン型です。[タスクの詳細](plannertaskdetails.md)オブジェクトの一部です。プロパティ/値の組の値は、[checklistItem](plannerchecklistitem.md) オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="56500-p103">The **plannerChecklistItemCollection** resource represents the collection of checklist items on a task. It is an Open Type. It is part of the [task details](plannertaskdetails.md) object. The value in the property-value pair is the [checklistItem](plannerchecklistitem.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="56500-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56500-113">Properties</span></span>
<span data-ttu-id="56500-p104">クライアントは、オープン型のプロパティを定義できます。この場合、クライアントは **GUID** をプロパティとして指定し、その値は [checklistItem](plannerchecklistitem.md) オブジェクトでなければなりません。以下に例を示します。チェックリストの項目を削除するには、プロパティの値を `null` に設定します。</span><span class="sxs-lookup"><span data-stu-id="56500-p104">Properties of an Open Type can be defined by the client. In this case, the client should provide **GUIDs** as properties and their values must be [checklistItem](plannerchecklistitem.md) objects. Example is shown below. To remove an item in the checklist, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="56500-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="56500-118">JSON representation</span></span>

<span data-ttu-id="56500-119">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="56500-119">Here is a JSON representation of the resource</span></span>

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
<span data-ttu-id="56500-120">// 例</span><span class="sxs-lookup"><span data-stu-id="56500-120">// Example</span></span>

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
