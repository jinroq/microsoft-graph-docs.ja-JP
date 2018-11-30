---
title: mediaInfo リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 961ce2375b742b2a657db28ec11d5439985583d3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073017"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="2385b-103">mediaInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2385b-103">mediaInfo resource type</span></span>

> <span data-ttu-id="2385b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2385b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2385b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2385b-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="2385b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2385b-106">Properties</span></span>
| <span data-ttu-id="2385b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2385b-107">Property</span></span>   | <span data-ttu-id="2385b-108">型</span><span class="sxs-lookup"><span data-stu-id="2385b-108">Type</span></span>    |<span data-ttu-id="2385b-109">説明</span><span class="sxs-lookup"><span data-stu-id="2385b-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2385b-110">resourceId</span><span class="sxs-lookup"><span data-stu-id="2385b-110">resourceId</span></span>     | <span data-ttu-id="2385b-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2385b-111">String</span></span>  |           |
| <span data-ttu-id="2385b-112">uri</span><span class="sxs-lookup"><span data-stu-id="2385b-112">uri</span></span>            | <span data-ttu-id="2385b-113">String</span><span class="sxs-lookup"><span data-stu-id="2385b-113">String</span></span>  |           |

## <a name="json-representation"></a><span data-ttu-id="2385b-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2385b-114">JSON representation</span></span>

<span data-ttu-id="2385b-115">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2385b-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->