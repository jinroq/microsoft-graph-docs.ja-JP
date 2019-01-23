---
title: bulkManagedDeviceActionResult リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5d1b23efdb5b8eed16c6c66d72a13efaef9e38d9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425842"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="fa221-103">bulkManagedDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fa221-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="fa221-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fa221-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fa221-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa221-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa221-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fa221-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa221-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fa221-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="fa221-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa221-108">Properties</span></span>
|<span data-ttu-id="fa221-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa221-109">Property</span></span>|<span data-ttu-id="fa221-110">型</span><span class="sxs-lookup"><span data-stu-id="fa221-110">Type</span></span>|<span data-ttu-id="fa221-111">説明</span><span class="sxs-lookup"><span data-stu-id="fa221-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa221-112">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="fa221-112">successfulDeviceIds</span></span>|<span data-ttu-id="fa221-113">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fa221-113">String collection</span></span>|<span data-ttu-id="fa221-114">正常なデバイス</span><span class="sxs-lookup"><span data-stu-id="fa221-114">Successful devices</span></span>|
|<span data-ttu-id="fa221-115">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="fa221-115">failedDeviceIds</span></span>|<span data-ttu-id="fa221-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fa221-116">String collection</span></span>|<span data-ttu-id="fa221-117">障害が発生したデバイス</span><span class="sxs-lookup"><span data-stu-id="fa221-117">Failed devices</span></span>|
|<span data-ttu-id="fa221-118">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="fa221-118">notFoundDeviceIds</span></span>|<span data-ttu-id="fa221-119">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fa221-119">String collection</span></span>|<span data-ttu-id="fa221-120">デバイスが見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="fa221-120">Not found devices</span></span>|
|<span data-ttu-id="fa221-121">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="fa221-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="fa221-122">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fa221-122">String collection</span></span>|<span data-ttu-id="fa221-123">デバイスがサポートされていません</span><span class="sxs-lookup"><span data-stu-id="fa221-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa221-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fa221-124">Relationships</span></span>
<span data-ttu-id="fa221-125">なし</span><span class="sxs-lookup"><span data-stu-id="fa221-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa221-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fa221-126">JSON Representation</span></span>
<span data-ttu-id="fa221-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fa221-127">Here is a JSON representation of the resource.</span></span>
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




