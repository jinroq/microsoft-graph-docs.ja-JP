---
title: operatingSystemVersionRange リソースの種類
description: オペレーティング システムのバージョンの範囲です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c0b81482ad4b48ad5fe59b1ec0109fcd3bf03f83
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918547"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="62d64-103">operatingSystemVersionRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="62d64-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="62d64-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="62d64-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62d64-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62d64-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62d64-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="62d64-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62d64-107">オペレーティング システムのバージョンの範囲です。</span><span class="sxs-lookup"><span data-stu-id="62d64-107">Operating System version range.</span></span>
## <a name="properties"></a><span data-ttu-id="62d64-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62d64-108">Properties</span></span>
|<span data-ttu-id="62d64-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62d64-109">Property</span></span>|<span data-ttu-id="62d64-110">種類</span><span class="sxs-lookup"><span data-stu-id="62d64-110">Type</span></span>|<span data-ttu-id="62d64-111">説明</span><span class="sxs-lookup"><span data-stu-id="62d64-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62d64-112">説明</span><span class="sxs-lookup"><span data-stu-id="62d64-112">description</span></span>|<span data-ttu-id="62d64-113">String</span><span class="sxs-lookup"><span data-stu-id="62d64-113">String</span></span>|<span data-ttu-id="62d64-114">この範囲 (有効 1702 のビルドなど) の説明</span><span class="sxs-lookup"><span data-stu-id="62d64-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="62d64-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="62d64-115">lowestVersion</span></span>|<span data-ttu-id="62d64-116">String</span><span class="sxs-lookup"><span data-stu-id="62d64-116">String</span></span>|<span data-ttu-id="62d64-117">最小包括的なバージョンをこの範囲に含まれています。</span><span class="sxs-lookup"><span data-stu-id="62d64-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="62d64-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="62d64-118">highestVersion</span></span>|<span data-ttu-id="62d64-119">String</span><span class="sxs-lookup"><span data-stu-id="62d64-119">String</span></span>|<span data-ttu-id="62d64-120">この範囲に含まれている最高の包括的なバージョンです。</span><span class="sxs-lookup"><span data-stu-id="62d64-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62d64-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="62d64-121">Relationships</span></span>
<span data-ttu-id="62d64-122">なし</span><span class="sxs-lookup"><span data-stu-id="62d64-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="62d64-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="62d64-123">JSON Representation</span></span>
<span data-ttu-id="62d64-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="62d64-124">Here is a JSON representation of the resource.</span></span>
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





