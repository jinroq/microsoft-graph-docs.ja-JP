---
title: メール リソースの種類
description: 以下は、リソースの JSON 表記です
localization_priority: Normal
ms.openlocfilehash: 02eb37c065cc8d664caf97f1f86da0efeaac09e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830059"
---
# <a name="email-resource-type"></a><span data-ttu-id="a520f-103">メール リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a520f-103">email resource type</span></span>

> <span data-ttu-id="a520f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a520f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a520f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a520f-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a520f-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a520f-106">JSON representation</span></span>

<span data-ttu-id="a520f-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a520f-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.email"
}-->

```json
{
  "address": "string"
}

```
## <a name="properties"></a><span data-ttu-id="a520f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a520f-108">Properties</span></span>
| <span data-ttu-id="a520f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a520f-109">Property</span></span>     | <span data-ttu-id="a520f-110">種類</span><span class="sxs-lookup"><span data-stu-id="a520f-110">Type</span></span>   |<span data-ttu-id="a520f-111">説明</span><span class="sxs-lookup"><span data-stu-id="a520f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a520f-112">address</span><span class="sxs-lookup"><span data-stu-id="a520f-112">address</span></span>|<span data-ttu-id="a520f-113">String</span><span class="sxs-lookup"><span data-stu-id="a520f-113">String</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "email resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
