---
title: iosMinimumOperatingSystem リソースの種類
description: iOS モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。
ms.openlocfilehash: 1b39890faf574ab952635c11f113c90479c3ba1a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021065"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="1f884-103">iosMinimumOperatingSystem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1f884-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="1f884-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1f884-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f884-105">iOS モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="1f884-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="1f884-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f884-106">Properties</span></span>
|<span data-ttu-id="1f884-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f884-107">Property</span></span>|<span data-ttu-id="1f884-108">型</span><span class="sxs-lookup"><span data-stu-id="1f884-108">Type</span></span>|<span data-ttu-id="1f884-109">説明</span><span class="sxs-lookup"><span data-stu-id="1f884-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f884-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="1f884-110">v8_0</span></span>|<span data-ttu-id="1f884-111">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1f884-111">Boolean</span></span>|<span data-ttu-id="1f884-112">バージョン 8.0 以降。</span><span class="sxs-lookup"><span data-stu-id="1f884-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="1f884-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="1f884-113">v9_0</span></span>|<span data-ttu-id="1f884-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1f884-114">Boolean</span></span>|<span data-ttu-id="1f884-115">バージョン 9.0 以降。</span><span class="sxs-lookup"><span data-stu-id="1f884-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="1f884-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="1f884-116">v10_0</span></span>|<span data-ttu-id="1f884-117">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1f884-117">Boolean</span></span>|<span data-ttu-id="1f884-118">バージョン 10.0 以降。</span><span class="sxs-lookup"><span data-stu-id="1f884-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="1f884-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="1f884-119">v11_0</span></span>|<span data-ttu-id="1f884-120">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1f884-120">Boolean</span></span>|<span data-ttu-id="1f884-121">バージョン 11.0 以降。</span><span class="sxs-lookup"><span data-stu-id="1f884-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="1f884-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="1f884-122">v12_0</span></span>|<span data-ttu-id="1f884-123">ブール値</span><span class="sxs-lookup"><span data-stu-id="1f884-123">Boolean</span></span>|<span data-ttu-id="1f884-124">12.0 またはそれ以降のバージョンです。</span><span class="sxs-lookup"><span data-stu-id="1f884-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f884-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1f884-125">Relationships</span></span>
<span data-ttu-id="1f884-126">なし</span><span class="sxs-lookup"><span data-stu-id="1f884-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1f884-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1f884-127">JSON Representation</span></span>
<span data-ttu-id="1f884-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1f884-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true,
  "v12_0": true
}
```



