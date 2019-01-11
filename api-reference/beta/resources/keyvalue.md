---
title: keyValue リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: 6f81d5aaef6e045abec02ebb5a55c4eb19db2665
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833846"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="5a59f-103">keyValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5a59f-103">keyValue resource type</span></span>

> <span data-ttu-id="5a59f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5a59f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a59f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a59f-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a59f-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5a59f-106">JSON representation</span></span>

<span data-ttu-id="5a59f-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5a59f-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyvalue"
}-->

```json
{
  "key": "string",
  "value": "string"
}

```
## <a name="properties"></a><span data-ttu-id="5a59f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a59f-108">Properties</span></span>
| <span data-ttu-id="5a59f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a59f-109">Property</span></span>     | <span data-ttu-id="5a59f-110">種類</span><span class="sxs-lookup"><span data-stu-id="5a59f-110">Type</span></span>   |<span data-ttu-id="5a59f-111">説明</span><span class="sxs-lookup"><span data-stu-id="5a59f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a59f-112">Key</span><span class="sxs-lookup"><span data-stu-id="5a59f-112">key</span></span>|<span data-ttu-id="5a59f-113">文字列</span><span class="sxs-lookup"><span data-stu-id="5a59f-113">string</span></span>||
|<span data-ttu-id="5a59f-114">value</span><span class="sxs-lookup"><span data-stu-id="5a59f-114">value</span></span>|<span data-ttu-id="5a59f-115">文字列</span><span class="sxs-lookup"><span data-stu-id="5a59f-115">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
