---
title: operatingSystemVersionRange リソースの種類
description: オペレーティング システムのバージョンの範囲です。
ms.openlocfilehash: af140bf2a5d889b66d45460465e47c466bb2160b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068533"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="6e612-103">operatingSystemVersionRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6e612-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="6e612-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6e612-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e612-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e612-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e612-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6e612-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6e612-107">オペレーティング システムのバージョンの範囲です。</span><span class="sxs-lookup"><span data-stu-id="6e612-107">Operating System version range.</span></span>
## <a name="properties"></a><span data-ttu-id="6e612-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e612-108">Properties</span></span>
|<span data-ttu-id="6e612-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e612-109">Property</span></span>|<span data-ttu-id="6e612-110">型</span><span class="sxs-lookup"><span data-stu-id="6e612-110">Type</span></span>|<span data-ttu-id="6e612-111">説明</span><span class="sxs-lookup"><span data-stu-id="6e612-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e612-112">説明</span><span class="sxs-lookup"><span data-stu-id="6e612-112">description</span></span>|<span data-ttu-id="6e612-113">String</span><span class="sxs-lookup"><span data-stu-id="6e612-113">String</span></span>|<span data-ttu-id="6e612-114">この範囲 (有効 1702 のビルドなど) の説明</span><span class="sxs-lookup"><span data-stu-id="6e612-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="6e612-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="6e612-115">lowestVersion</span></span>|<span data-ttu-id="6e612-116">String</span><span class="sxs-lookup"><span data-stu-id="6e612-116">String</span></span>|<span data-ttu-id="6e612-117">最小包括的なバージョンをこの範囲に含まれています。</span><span class="sxs-lookup"><span data-stu-id="6e612-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="6e612-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="6e612-118">highestVersion</span></span>|<span data-ttu-id="6e612-119">String</span><span class="sxs-lookup"><span data-stu-id="6e612-119">String</span></span>|<span data-ttu-id="6e612-120">この範囲に含まれている最高の包括的なバージョンです。</span><span class="sxs-lookup"><span data-stu-id="6e612-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e612-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6e612-121">Relationships</span></span>
<span data-ttu-id="6e612-122">なし</span><span class="sxs-lookup"><span data-stu-id="6e612-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6e612-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6e612-123">JSON Representation</span></span>
<span data-ttu-id="6e612-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6e612-124">Here is a JSON representation of the resource.</span></span>
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





