---
title: operatingSystemVersionRange リソースの種類
description: オペレーティング システムのバージョンの範囲です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 56df6b53dc29247d3f718ad185152069a071a0f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875804"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="bd63f-103">operatingSystemVersionRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bd63f-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="bd63f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bd63f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd63f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd63f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd63f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bd63f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd63f-107">オペレーティング システムのバージョンの範囲です。</span><span class="sxs-lookup"><span data-stu-id="bd63f-107">Operating System version range.</span></span>
## <a name="properties"></a><span data-ttu-id="bd63f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd63f-108">Properties</span></span>
|<span data-ttu-id="bd63f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd63f-109">Property</span></span>|<span data-ttu-id="bd63f-110">種類</span><span class="sxs-lookup"><span data-stu-id="bd63f-110">Type</span></span>|<span data-ttu-id="bd63f-111">説明</span><span class="sxs-lookup"><span data-stu-id="bd63f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd63f-112">説明</span><span class="sxs-lookup"><span data-stu-id="bd63f-112">description</span></span>|<span data-ttu-id="bd63f-113">String</span><span class="sxs-lookup"><span data-stu-id="bd63f-113">String</span></span>|<span data-ttu-id="bd63f-114">この範囲 (有効 1702 のビルドなど) の説明</span><span class="sxs-lookup"><span data-stu-id="bd63f-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="bd63f-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="bd63f-115">lowestVersion</span></span>|<span data-ttu-id="bd63f-116">String</span><span class="sxs-lookup"><span data-stu-id="bd63f-116">String</span></span>|<span data-ttu-id="bd63f-117">最小包括的なバージョンをこの範囲に含まれています。</span><span class="sxs-lookup"><span data-stu-id="bd63f-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="bd63f-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="bd63f-118">highestVersion</span></span>|<span data-ttu-id="bd63f-119">String</span><span class="sxs-lookup"><span data-stu-id="bd63f-119">String</span></span>|<span data-ttu-id="bd63f-120">この範囲に含まれている最高の包括的なバージョンです。</span><span class="sxs-lookup"><span data-stu-id="bd63f-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd63f-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bd63f-121">Relationships</span></span>
<span data-ttu-id="bd63f-122">なし</span><span class="sxs-lookup"><span data-stu-id="bd63f-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bd63f-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bd63f-123">JSON Representation</span></span>
<span data-ttu-id="bd63f-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bd63f-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "lowestVersion": "String",
  "highestVersion": "String"
}
```





