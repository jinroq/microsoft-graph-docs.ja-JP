---
title: windowsMinimumOperatingSystem リソースの種類
description: Windows モバイル アプリに必要な最小オペレーティング システム。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d80a7c957b4a03132b349ebd609e21481322021a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863792"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="ce217-103">windowsMinimumOperatingSystem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ce217-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="ce217-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce217-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce217-105">Windows モバイル アプリに必要な最小オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="ce217-105">The minimum operating system required for a Windows mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="ce217-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce217-106">Properties</span></span>
|<span data-ttu-id="ce217-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce217-107">Property</span></span>|<span data-ttu-id="ce217-108">種類</span><span class="sxs-lookup"><span data-stu-id="ce217-108">Type</span></span>|<span data-ttu-id="ce217-109">説明</span><span class="sxs-lookup"><span data-stu-id="ce217-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce217-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="ce217-110">v8_0</span></span>|<span data-ttu-id="ce217-111">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="ce217-111">Boolean</span></span>|<span data-ttu-id="ce217-112">Windows バージョン 8.0 以降。</span><span class="sxs-lookup"><span data-stu-id="ce217-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="ce217-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="ce217-113">v8_1</span></span>|<span data-ttu-id="ce217-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="ce217-114">Boolean</span></span>|<span data-ttu-id="ce217-115">Windows バージョン 8.1 以降。</span><span class="sxs-lookup"><span data-stu-id="ce217-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="ce217-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="ce217-116">v10_0</span></span>|<span data-ttu-id="ce217-117">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="ce217-117">Boolean</span></span>|<span data-ttu-id="ce217-118">Windows バージョン 10.0 以降。</span><span class="sxs-lookup"><span data-stu-id="ce217-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce217-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ce217-119">Relationships</span></span>
<span data-ttu-id="ce217-120">なし</span><span class="sxs-lookup"><span data-stu-id="ce217-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ce217-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ce217-121">JSON Representation</span></span>
<span data-ttu-id="ce217-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ce217-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true
}
```



