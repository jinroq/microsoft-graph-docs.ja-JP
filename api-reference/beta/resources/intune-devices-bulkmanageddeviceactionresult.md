---
title: bulkManagedDeviceActionResult リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: 856054f293dca0ae86681246d4783aae6a0373c0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070102"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="c1f37-103">bulkManagedDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1f37-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="c1f37-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c1f37-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1f37-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1f37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1f37-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c1f37-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1f37-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c1f37-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c1f37-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1f37-108">Properties</span></span>
|<span data-ttu-id="c1f37-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1f37-109">Property</span></span>|<span data-ttu-id="c1f37-110">型</span><span class="sxs-lookup"><span data-stu-id="c1f37-110">Type</span></span>|<span data-ttu-id="c1f37-111">説明</span><span class="sxs-lookup"><span data-stu-id="c1f37-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1f37-112">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="c1f37-112">successfulDeviceIds</span></span>|<span data-ttu-id="c1f37-113">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c1f37-113">String collection</span></span>|<span data-ttu-id="c1f37-114">正常なデバイス</span><span class="sxs-lookup"><span data-stu-id="c1f37-114">Successful devices</span></span>|
|<span data-ttu-id="c1f37-115">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="c1f37-115">failedDeviceIds</span></span>|<span data-ttu-id="c1f37-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c1f37-116">String collection</span></span>|<span data-ttu-id="c1f37-117">障害が発生したデバイス</span><span class="sxs-lookup"><span data-stu-id="c1f37-117">Failed devices</span></span>|
|<span data-ttu-id="c1f37-118">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="c1f37-118">notFoundDeviceIds</span></span>|<span data-ttu-id="c1f37-119">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c1f37-119">String collection</span></span>|<span data-ttu-id="c1f37-120">デバイスが見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="c1f37-120">Not found devices</span></span>|
|<span data-ttu-id="c1f37-121">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="c1f37-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="c1f37-122">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c1f37-122">String collection</span></span>|<span data-ttu-id="c1f37-123">デバイスがサポートされていません</span><span class="sxs-lookup"><span data-stu-id="c1f37-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1f37-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c1f37-124">Relationships</span></span>
<span data-ttu-id="c1f37-125">なし</span><span class="sxs-lookup"><span data-stu-id="c1f37-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c1f37-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1f37-126">JSON Representation</span></span>
<span data-ttu-id="c1f37-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c1f37-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bulkManagedDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bulkManagedDeviceActionResult",
  "successfulDeviceIds": [
    "String"
  ],
  "failedDeviceIds": [
    "String"
  ],
  "notFoundDeviceIds": [
    "String"
  ],
  "notSupportedDeviceIds": [
    "String"
  ]
}
```





