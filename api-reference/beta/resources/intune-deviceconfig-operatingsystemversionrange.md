---
title: operatingSystemVersionRange リソースの種類
description: オペレーティング システムのバージョンの範囲です。
author: tfitzmac
ms.openlocfilehash: b853e71b2d8f66d24122afb51cea97fc6a8f8d7e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331165"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="de488-103">operatingSystemVersionRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="de488-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="de488-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="de488-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de488-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de488-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de488-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="de488-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de488-107">オペレーティング システムのバージョンの範囲です。</span><span class="sxs-lookup"><span data-stu-id="de488-107">Operating System version range.</span></span>
## <a name="properties"></a><span data-ttu-id="de488-108">Properties</span><span class="sxs-lookup"><span data-stu-id="de488-108">Properties</span></span>
|<span data-ttu-id="de488-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de488-109">Property</span></span>|<span data-ttu-id="de488-110">種類</span><span class="sxs-lookup"><span data-stu-id="de488-110">Type</span></span>|<span data-ttu-id="de488-111">説明</span><span class="sxs-lookup"><span data-stu-id="de488-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de488-112">説明</span><span class="sxs-lookup"><span data-stu-id="de488-112">description</span></span>|<span data-ttu-id="de488-113">String</span><span class="sxs-lookup"><span data-stu-id="de488-113">String</span></span>|<span data-ttu-id="de488-114">この範囲 (有効 1702 のビルドなど) の説明</span><span class="sxs-lookup"><span data-stu-id="de488-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="de488-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="de488-115">lowestVersion</span></span>|<span data-ttu-id="de488-116">String</span><span class="sxs-lookup"><span data-stu-id="de488-116">String</span></span>|<span data-ttu-id="de488-117">最小包括的なバージョンをこの範囲に含まれています。</span><span class="sxs-lookup"><span data-stu-id="de488-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="de488-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="de488-118">highestVersion</span></span>|<span data-ttu-id="de488-119">String</span><span class="sxs-lookup"><span data-stu-id="de488-119">String</span></span>|<span data-ttu-id="de488-120">この範囲に含まれている最高の包括的なバージョンです。</span><span class="sxs-lookup"><span data-stu-id="de488-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de488-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="de488-121">Relationships</span></span>
<span data-ttu-id="de488-122">なし</span><span class="sxs-lookup"><span data-stu-id="de488-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="de488-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="de488-123">JSON Representation</span></span>
<span data-ttu-id="de488-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="de488-124">Here is a JSON representation of the resource.</span></span>
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





