---
title: responseStatus リソースの種類
description: 会議出席依頼の応答状態です。
ms.openlocfilehash: 9a6ddb26f018535682611152a69c2039f1c7f016
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069545"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="6f387-103">responseStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6f387-103">responseStatus resource type</span></span>

> <span data-ttu-id="6f387-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6f387-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f387-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f387-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6f387-106">会議出席依頼の応答状態です。</span><span class="sxs-lookup"><span data-stu-id="6f387-106">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="6f387-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6f387-107">Properties</span></span>

| <span data-ttu-id="6f387-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6f387-108">Property</span></span> | <span data-ttu-id="6f387-109">型</span><span class="sxs-lookup"><span data-stu-id="6f387-109">Type</span></span>           | <span data-ttu-id="6f387-110">説明</span><span class="sxs-lookup"><span data-stu-id="6f387-110">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="6f387-111">response</span><span class="sxs-lookup"><span data-stu-id="6f387-111">response</span></span> | <span data-ttu-id="6f387-112">String</span><span class="sxs-lookup"><span data-stu-id="6f387-112">String</span></span>         | <span data-ttu-id="6f387-113">応答の種類。</span><span class="sxs-lookup"><span data-stu-id="6f387-113">The response type.</span></span> <span data-ttu-id="6f387-114">可能な値は `None`、`Organizer`、`TentativelyAccepted`、`Accepted`、`Declined`、`NotResponded` です。</span><span class="sxs-lookup"><span data-stu-id="6f387-114">Possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="6f387-115">time</span><span class="sxs-lookup"><span data-stu-id="6f387-115">time</span></span>     | <span data-ttu-id="6f387-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f387-116">DateTimeOffset</span></span> | <span data-ttu-id="6f387-p103">応答が返された日時。ISO 8601 形式を使って表され、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6f387-p103">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f387-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6f387-120">JSON representation</span></span>

<span data-ttu-id="6f387-121">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="6f387-121">Here is a JSON representation of the resource</span></span>

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
