---
title: bulkManagedDeviceActionResult リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d1f260b032078bdcd60000ecbde315a91cfcf492
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337595"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="12226-103">bulkManagedDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="12226-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="12226-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12226-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12226-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="12226-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12226-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="12226-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="12226-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12226-107">Properties</span></span>
|<span data-ttu-id="12226-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12226-108">Property</span></span>|<span data-ttu-id="12226-109">型</span><span class="sxs-lookup"><span data-stu-id="12226-109">Type</span></span>|<span data-ttu-id="12226-110">説明</span><span class="sxs-lookup"><span data-stu-id="12226-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12226-111">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="12226-111">successfulDeviceIds</span></span>|<span data-ttu-id="12226-112">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="12226-112">String collection</span></span>|<span data-ttu-id="12226-113">成功したデバイス</span><span class="sxs-lookup"><span data-stu-id="12226-113">Successful devices</span></span>|
|<span data-ttu-id="12226-114">失敗 Deviceid</span><span class="sxs-lookup"><span data-stu-id="12226-114">failedDeviceIds</span></span>|<span data-ttu-id="12226-115">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="12226-115">String collection</span></span>|<span data-ttu-id="12226-116">失敗したデバイス</span><span class="sxs-lookup"><span data-stu-id="12226-116">Failed devices</span></span>|
|<span data-ttu-id="12226-117">Not見つかり Deviceid</span><span class="sxs-lookup"><span data-stu-id="12226-117">notFoundDeviceIds</span></span>|<span data-ttu-id="12226-118">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="12226-118">String collection</span></span>|<span data-ttu-id="12226-119">見つからないデバイス</span><span class="sxs-lookup"><span data-stu-id="12226-119">Not found devices</span></span>|
|<span data-ttu-id="12226-120">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="12226-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="12226-121">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="12226-121">String collection</span></span>|<span data-ttu-id="12226-122">サポートされていないデバイス</span><span class="sxs-lookup"><span data-stu-id="12226-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="12226-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="12226-123">Relationships</span></span>
<span data-ttu-id="12226-124">なし</span><span class="sxs-lookup"><span data-stu-id="12226-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="12226-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="12226-125">JSON Representation</span></span>
<span data-ttu-id="12226-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="12226-126">Here is a JSON representation of the resource.</span></span>
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



