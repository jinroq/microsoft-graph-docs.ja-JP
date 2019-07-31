---
title: Audioアヒルの構成リソースの種類
description: 他のソースの ducking のパラメーター (他のソースの段階的なインおよび out)。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cfff0ca240a13c9c4396d605def05a52e1916778
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013221"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="d5279-103">Audioアヒルの構成リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d5279-103">audioDuckingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5279-104">他のソースの ducking のパラメーター (他のソースの段階的なインおよび out)。</span><span class="sxs-lookup"><span data-stu-id="d5279-104">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="d5279-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5279-105">Properties</span></span>

| <span data-ttu-id="d5279-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5279-106">Property</span></span>      | <span data-ttu-id="d5279-107">型</span><span class="sxs-lookup"><span data-stu-id="d5279-107">Type</span></span>     | <span data-ttu-id="d5279-108">説明</span><span class="sxs-lookup"><span data-stu-id="d5279-108">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="d5279-109">下位レベル</span><span class="sxs-lookup"><span data-stu-id="d5279-109">lowerLevel</span></span>    | <span data-ttu-id="d5279-110">Int64</span><span class="sxs-lookup"><span data-stu-id="d5279-110">Int64</span></span>    | <span data-ttu-id="d5279-111">ソースが処理されるときのソースの量 (パーセント)。</span><span class="sxs-lookup"><span data-stu-id="d5279-111">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="d5279-112">rampActive</span><span class="sxs-lookup"><span data-stu-id="d5279-112">rampActive</span></span>    | <span data-ttu-id="d5279-113">Int64</span><span class="sxs-lookup"><span data-stu-id="d5279-113">Int64</span></span>    | <span data-ttu-id="d5279-114">発行元が "フェードアウト" するまでにかかる時間 (ミリ秒)。</span><span class="sxs-lookup"><span data-stu-id="d5279-114">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="d5279-115">rampInactive</span><span class="sxs-lookup"><span data-stu-id="d5279-115">rampInactive</span></span>  | <span data-ttu-id="d5279-116">Int64</span><span class="sxs-lookup"><span data-stu-id="d5279-116">Int64</span></span>    | <span data-ttu-id="d5279-117">発行元が "フェードイン" になるまでにかかる時間 (ミリ秒)。</span><span class="sxs-lookup"><span data-stu-id="d5279-117">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="d5279-118">upperLevel</span><span class="sxs-lookup"><span data-stu-id="d5279-118">upperLevel</span></span>    | <span data-ttu-id="d5279-119">Int64</span><span class="sxs-lookup"><span data-stu-id="d5279-119">Int64</span></span>    | <span data-ttu-id="d5279-120">ソースが発行されていない場合のソースの量 (パーセント)。</span><span class="sxs-lookup"><span data-stu-id="d5279-120">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="d5279-121">**注:** 傾斜時間は5000ミリ秒を超えることはできません。</span><span class="sxs-lookup"><span data-stu-id="d5279-121">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5279-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d5279-122">JSON representation</span></span>

<span data-ttu-id="d5279-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d5279-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioDuckingConfiguration"
}-->
```json
{
  "lowerLevel": 20,
  "rampActive": 1000,
  "rampInactive": 1000,
  "upperLevel": 100
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
