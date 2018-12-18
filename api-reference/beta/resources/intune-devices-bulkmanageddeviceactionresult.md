---
title: bulkManagedDeviceActionResult リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 0a80a05b1caba7cd5ac1e672c9e39366ca29048c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339516"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="564bb-103">bulkManagedDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="564bb-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="564bb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="564bb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="564bb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="564bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="564bb-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="564bb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="564bb-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="564bb-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="564bb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="564bb-108">Properties</span></span>
|<span data-ttu-id="564bb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="564bb-109">Property</span></span>|<span data-ttu-id="564bb-110">種類</span><span class="sxs-lookup"><span data-stu-id="564bb-110">Type</span></span>|<span data-ttu-id="564bb-111">説明</span><span class="sxs-lookup"><span data-stu-id="564bb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="564bb-112">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="564bb-112">successfulDeviceIds</span></span>|<span data-ttu-id="564bb-113">String コレクション</span><span class="sxs-lookup"><span data-stu-id="564bb-113">String collection</span></span>|<span data-ttu-id="564bb-114">正常なデバイス</span><span class="sxs-lookup"><span data-stu-id="564bb-114">Successful devices</span></span>|
|<span data-ttu-id="564bb-115">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="564bb-115">failedDeviceIds</span></span>|<span data-ttu-id="564bb-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="564bb-116">String collection</span></span>|<span data-ttu-id="564bb-117">障害が発生したデバイス</span><span class="sxs-lookup"><span data-stu-id="564bb-117">Failed devices</span></span>|
|<span data-ttu-id="564bb-118">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="564bb-118">notFoundDeviceIds</span></span>|<span data-ttu-id="564bb-119">String コレクション</span><span class="sxs-lookup"><span data-stu-id="564bb-119">String collection</span></span>|<span data-ttu-id="564bb-120">デバイスが見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="564bb-120">Not found devices</span></span>|
|<span data-ttu-id="564bb-121">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="564bb-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="564bb-122">String コレクション</span><span class="sxs-lookup"><span data-stu-id="564bb-122">String collection</span></span>|<span data-ttu-id="564bb-123">デバイスがサポートされていません</span><span class="sxs-lookup"><span data-stu-id="564bb-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="564bb-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="564bb-124">Relationships</span></span>
<span data-ttu-id="564bb-125">なし</span><span class="sxs-lookup"><span data-stu-id="564bb-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="564bb-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="564bb-126">JSON Representation</span></span>
<span data-ttu-id="564bb-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="564bb-127">Here is a JSON representation of the resource.</span></span>
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





