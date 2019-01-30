---
title: insightIdentity
description: 共有アイテムのプロパティを格納する複合型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 45ac8874a30ebb4f3196f03a675229bf1fab750c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643889"
---
# <a name="insightidentity"></a><span data-ttu-id="8eb1f-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="8eb1f-103">insightIdentity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8eb1f-104">[共有](insights-shared.md)アイテムのプロパティを格納する複合型。</span><span class="sxs-lookup"><span data-stu-id="8eb1f-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="8eb1f-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8eb1f-105">JSON representation</span></span>
<span data-ttu-id="8eb1f-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="8eb1f-106">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="8eb1f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8eb1f-107">Properties</span></span>

| <span data-ttu-id="8eb1f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8eb1f-108">Property</span></span>              | <span data-ttu-id="8eb1f-109">型</span><span class="sxs-lookup"><span data-stu-id="8eb1f-109">Type</span></span>          | <span data-ttu-id="8eb1f-110">説明</span><span class="sxs-lookup"><span data-stu-id="8eb1f-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="8eb1f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8eb1f-111">displayName</span></span>       | <span data-ttu-id="8eb1f-112">String</span><span class="sxs-lookup"><span data-stu-id="8eb1f-112">String</span></span>          | <span data-ttu-id="8eb1f-113">アイテムを共有するユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="8eb1f-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="8eb1f-114">id</span><span class="sxs-lookup"><span data-stu-id="8eb1f-114">id</span></span>              | <span data-ttu-id="8eb1f-115">String</span><span class="sxs-lookup"><span data-stu-id="8eb1f-115">String</span></span>        | <span data-ttu-id="8eb1f-116">アイテムを共有するユーザーの id です。</span><span class="sxs-lookup"><span data-stu-id="8eb1f-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="8eb1f-117">address</span><span class="sxs-lookup"><span data-stu-id="8eb1f-117">address</span></span>             | <span data-ttu-id="8eb1f-118">String</span><span class="sxs-lookup"><span data-stu-id="8eb1f-118">String</span></span>      | <span data-ttu-id="8eb1f-119">アイテムを共有するユーザーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="8eb1f-119">The email address of the user who shared the item.</span></span>  |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-insightidentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
