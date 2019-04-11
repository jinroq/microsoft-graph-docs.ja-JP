---
title: bulkmanageddeviceactionresult リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e0978367465fde92f9874e338a0de84da2a20403
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31770936"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="fb374-103">bulkmanageddeviceactionresult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fb374-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="fb374-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb374-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb374-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fb374-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb374-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fb374-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="fb374-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb374-107">Properties</span></span>
|<span data-ttu-id="fb374-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb374-108">Property</span></span>|<span data-ttu-id="fb374-109">型</span><span class="sxs-lookup"><span data-stu-id="fb374-109">Type</span></span>|<span data-ttu-id="fb374-110">説明</span><span class="sxs-lookup"><span data-stu-id="fb374-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb374-111">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="fb374-111">successfulDeviceIds</span></span>|<span data-ttu-id="fb374-112">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fb374-112">String collection</span></span>|<span data-ttu-id="fb374-113">成功したデバイス</span><span class="sxs-lookup"><span data-stu-id="fb374-113">Successful devices</span></span>|
|<span data-ttu-id="fb374-114">失敗 deviceid</span><span class="sxs-lookup"><span data-stu-id="fb374-114">failedDeviceIds</span></span>|<span data-ttu-id="fb374-115">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fb374-115">String collection</span></span>|<span data-ttu-id="fb374-116">失敗したデバイス</span><span class="sxs-lookup"><span data-stu-id="fb374-116">Failed devices</span></span>|
|<span data-ttu-id="fb374-117">not見つかり deviceid</span><span class="sxs-lookup"><span data-stu-id="fb374-117">notFoundDeviceIds</span></span>|<span data-ttu-id="fb374-118">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fb374-118">String collection</span></span>|<span data-ttu-id="fb374-119">見つからないデバイス</span><span class="sxs-lookup"><span data-stu-id="fb374-119">Not found devices</span></span>|
|<span data-ttu-id="fb374-120">notsupporteddeviceids</span><span class="sxs-lookup"><span data-stu-id="fb374-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="fb374-121">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fb374-121">String collection</span></span>|<span data-ttu-id="fb374-122">サポートされていないデバイス</span><span class="sxs-lookup"><span data-stu-id="fb374-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb374-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fb374-123">Relationships</span></span>
<span data-ttu-id="fb374-124">なし</span><span class="sxs-lookup"><span data-stu-id="fb374-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb374-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fb374-125">JSON Representation</span></span>
<span data-ttu-id="fb374-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fb374-126">Here is a JSON representation of the resource.</span></span>
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





