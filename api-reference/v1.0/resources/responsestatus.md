---
title: responseStatus リソースの種類
description: 会議出席依頼の応答状態です。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 03deeabfd789fe3e8912d5a431af21bc2c8e5256
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034665"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="33b21-103">responseStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="33b21-103">responseStatus resource type</span></span>

<span data-ttu-id="33b21-104">会議出席依頼の応答状態です。</span><span class="sxs-lookup"><span data-stu-id="33b21-104">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="33b21-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33b21-105">Properties</span></span>

| <span data-ttu-id="33b21-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33b21-106">Property</span></span> | <span data-ttu-id="33b21-107">型</span><span class="sxs-lookup"><span data-stu-id="33b21-107">Type</span></span>           | <span data-ttu-id="33b21-108">説明</span><span class="sxs-lookup"><span data-stu-id="33b21-108">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="33b21-109">response</span><span class="sxs-lookup"><span data-stu-id="33b21-109">response</span></span> | <span data-ttu-id="33b21-110">responseType</span><span class="sxs-lookup"><span data-stu-id="33b21-110">responseType</span></span>   | <span data-ttu-id="33b21-111">応答の種類。</span><span class="sxs-lookup"><span data-stu-id="33b21-111">The response type.</span></span> <span data-ttu-id="33b21-112">使用可能な値: `None`、`Organizer`、`TentativelyAccepted`、`Accepted`、`Declined`、`NotResponded`。</span><span class="sxs-lookup"><span data-stu-id="33b21-112">The possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="33b21-113">time</span><span class="sxs-lookup"><span data-stu-id="33b21-113">time</span></span>     | <span data-ttu-id="33b21-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33b21-114">DateTimeOffset</span></span> | <span data-ttu-id="33b21-p102">応答が返された日時。ISO 8601 形式を使って表され、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="33b21-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="33b21-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="33b21-118">JSON representation</span></span>

<span data-ttu-id="33b21-119">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="33b21-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.responseStatus"
}-->

```json
{
  "response": "String",
  "time": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
