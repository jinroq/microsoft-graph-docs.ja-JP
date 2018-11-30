---
title: mediaConfig リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: a04670d4c13299bde00c3812b9ecb996885330d3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066782"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="a2193-103">mediaConfig リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2193-103">mediaConfig resource type</span></span>

> <span data-ttu-id="a2193-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a2193-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2193-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2193-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="a2193-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2193-106">Properties</span></span>

| <span data-ttu-id="a2193-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2193-107">Property</span></span>       | <span data-ttu-id="a2193-108">型</span><span class="sxs-lookup"><span data-stu-id="a2193-108">Type</span></span>    | <span data-ttu-id="a2193-109">説明</span><span class="sxs-lookup"><span data-stu-id="a2193-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a2193-110">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="a2193-110">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="a2193-111">ブール値</span><span class="sxs-lookup"><span data-stu-id="a2193-111">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="a2193-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2193-112">JSON representation</span></span>

<span data-ttu-id="a2193-113">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a2193-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "removeFromDefaultAudioGroup"
  ],
  "@odata.type": "microsoft.graph.mediaConfig"
}-->
```json
{
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->