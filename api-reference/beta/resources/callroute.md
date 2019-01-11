---
title: callRoute リソースの種類
description: CallRoute 型です。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: e417a7e814b5a2a80da1fa9cd7a551f82e0c37db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815086"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="ba8d6-103">callRoute リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ba8d6-103">callRoute resource type</span></span>

> <span data-ttu-id="ba8d6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ba8d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba8d6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba8d6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ba8d6-106">CallRoute 型です。</span><span class="sxs-lookup"><span data-stu-id="ba8d6-106">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="ba8d6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba8d6-107">Properties</span></span>

| <span data-ttu-id="ba8d6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba8d6-108">Property</span></span>            | <span data-ttu-id="ba8d6-109">種類</span><span class="sxs-lookup"><span data-stu-id="ba8d6-109">Type</span></span>                          | <span data-ttu-id="ba8d6-110">説明</span><span class="sxs-lookup"><span data-stu-id="ba8d6-110">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="ba8d6-111">最終的な</span><span class="sxs-lookup"><span data-stu-id="ba8d6-111">final</span></span>               | [<span data-ttu-id="ba8d6-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="ba8d6-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="ba8d6-113">この id は、呼び出しを解決しました。</span><span class="sxs-lookup"><span data-stu-id="ba8d6-113">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="ba8d6-114">翻訳元</span><span class="sxs-lookup"><span data-stu-id="ba8d6-114">original</span></span>            | [<span data-ttu-id="ba8d6-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="ba8d6-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="ba8d6-116">呼び出しで使用されていた id です。</span><span class="sxs-lookup"><span data-stu-id="ba8d6-116">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="ba8d6-117">routingType</span><span class="sxs-lookup"><span data-stu-id="ba8d6-117">routingType</span></span>         | <span data-ttu-id="ba8d6-118">String</span><span class="sxs-lookup"><span data-stu-id="ba8d6-118">String</span></span>                        | <span data-ttu-id="ba8d6-119">可能な値は、`forwarded`、`lookup`、`selfFork` です。</span><span class="sxs-lookup"><span data-stu-id="ba8d6-119">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="ba8d6-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ba8d6-120">JSON representation</span></span>

<span data-ttu-id="ba8d6-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ba8d6-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRoute"
}-->
```json
{
  "final": {"@odata.type": "#microsoft.graph.identitySet"},
  "original": {"@odata.type": "#microsoft.graph.identitySet"},
  "routingType": "forwarded | lookup | selfFork"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
