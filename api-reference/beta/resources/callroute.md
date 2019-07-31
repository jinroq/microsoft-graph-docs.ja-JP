---
title: callRoute リソースの種類
description: CallRoute の種類。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9978bffd55f62f0646f84d2405df70eba6232d68
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974058"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="c1ada-103">callRoute リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1ada-103">callRoute resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1ada-104">CallRoute の種類。</span><span class="sxs-lookup"><span data-stu-id="c1ada-104">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="c1ada-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1ada-105">Properties</span></span>

| <span data-ttu-id="c1ada-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1ada-106">Property</span></span>            | <span data-ttu-id="c1ada-107">型</span><span class="sxs-lookup"><span data-stu-id="c1ada-107">Type</span></span>                          | <span data-ttu-id="c1ada-108">説明</span><span class="sxs-lookup"><span data-stu-id="c1ada-108">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="c1ada-109">最終的な</span><span class="sxs-lookup"><span data-stu-id="c1ada-109">final</span></span>               | [<span data-ttu-id="c1ada-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="c1ada-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="c1ada-111">呼び出しで解決された id。</span><span class="sxs-lookup"><span data-stu-id="c1ada-111">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="c1ada-112">翻訳元</span><span class="sxs-lookup"><span data-stu-id="c1ada-112">original</span></span>            | [<span data-ttu-id="c1ada-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="c1ada-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="c1ada-114">最初に呼び出しで使用された id。</span><span class="sxs-lookup"><span data-stu-id="c1ada-114">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="c1ada-115">routingType</span><span class="sxs-lookup"><span data-stu-id="c1ada-115">routingType</span></span>         | <span data-ttu-id="c1ada-116">String</span><span class="sxs-lookup"><span data-stu-id="c1ada-116">String</span></span>                        | <span data-ttu-id="c1ada-117">可能な値は、`forwarded`、`lookup`、`selfFork` です。</span><span class="sxs-lookup"><span data-stu-id="c1ada-117">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="c1ada-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1ada-118">JSON representation</span></span>

<span data-ttu-id="c1ada-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c1ada-119">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
