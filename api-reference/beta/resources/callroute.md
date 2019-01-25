---
title: callRoute リソースの種類
description: CallRoute 型です。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cfa470c4d3a03655221cab1f29baa60d00a8cf6c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512802"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="afd65-103">callRoute リソースの種類</span><span class="sxs-lookup"><span data-stu-id="afd65-103">callRoute resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afd65-104">CallRoute 型です。</span><span class="sxs-lookup"><span data-stu-id="afd65-104">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="afd65-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="afd65-105">Properties</span></span>

| <span data-ttu-id="afd65-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="afd65-106">Property</span></span>            | <span data-ttu-id="afd65-107">型</span><span class="sxs-lookup"><span data-stu-id="afd65-107">Type</span></span>                          | <span data-ttu-id="afd65-108">説明</span><span class="sxs-lookup"><span data-stu-id="afd65-108">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="afd65-109">Final</span><span class="sxs-lookup"><span data-stu-id="afd65-109">final</span></span>               | [<span data-ttu-id="afd65-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="afd65-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="afd65-111">この id は、呼び出しを解決しました。</span><span class="sxs-lookup"><span data-stu-id="afd65-111">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="afd65-112">Original</span><span class="sxs-lookup"><span data-stu-id="afd65-112">original</span></span>            | [<span data-ttu-id="afd65-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="afd65-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="afd65-114">呼び出しで使用されていた id です。</span><span class="sxs-lookup"><span data-stu-id="afd65-114">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="afd65-115">routingType</span><span class="sxs-lookup"><span data-stu-id="afd65-115">routingType</span></span>         | <span data-ttu-id="afd65-116">String</span><span class="sxs-lookup"><span data-stu-id="afd65-116">String</span></span>                        | <span data-ttu-id="afd65-117">可能な値は、`forwarded`、`lookup`、`selfFork` です。</span><span class="sxs-lookup"><span data-stu-id="afd65-117">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="afd65-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="afd65-118">JSON representation</span></span>

<span data-ttu-id="afd65-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="afd65-119">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/callroute.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
