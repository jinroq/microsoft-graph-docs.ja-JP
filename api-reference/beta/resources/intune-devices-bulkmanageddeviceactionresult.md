---
title: bulkManagedDeviceActionResult リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5a7b5e719e837dbd175fa634aea2082f5b0b142b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999991"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="8d94e-103">bulkManagedDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8d94e-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="8d94e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d94e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d94e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8d94e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d94e-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8d94e-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8d94e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d94e-107">Properties</span></span>
|<span data-ttu-id="8d94e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d94e-108">Property</span></span>|<span data-ttu-id="8d94e-109">型</span><span class="sxs-lookup"><span data-stu-id="8d94e-109">Type</span></span>|<span data-ttu-id="8d94e-110">説明</span><span class="sxs-lookup"><span data-stu-id="8d94e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d94e-111">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="8d94e-111">successfulDeviceIds</span></span>|<span data-ttu-id="8d94e-112">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="8d94e-112">String collection</span></span>|<span data-ttu-id="8d94e-113">成功したデバイス</span><span class="sxs-lookup"><span data-stu-id="8d94e-113">Successful devices</span></span>|
|<span data-ttu-id="8d94e-114">失敗 Deviceid</span><span class="sxs-lookup"><span data-stu-id="8d94e-114">failedDeviceIds</span></span>|<span data-ttu-id="8d94e-115">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="8d94e-115">String collection</span></span>|<span data-ttu-id="8d94e-116">失敗したデバイス</span><span class="sxs-lookup"><span data-stu-id="8d94e-116">Failed devices</span></span>|
|<span data-ttu-id="8d94e-117">Not見つかり Deviceid</span><span class="sxs-lookup"><span data-stu-id="8d94e-117">notFoundDeviceIds</span></span>|<span data-ttu-id="8d94e-118">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="8d94e-118">String collection</span></span>|<span data-ttu-id="8d94e-119">見つからないデバイス</span><span class="sxs-lookup"><span data-stu-id="8d94e-119">Not found devices</span></span>|
|<span data-ttu-id="8d94e-120">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="8d94e-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="8d94e-121">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="8d94e-121">String collection</span></span>|<span data-ttu-id="8d94e-122">サポートされていないデバイス</span><span class="sxs-lookup"><span data-stu-id="8d94e-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d94e-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8d94e-123">Relationships</span></span>
<span data-ttu-id="8d94e-124">なし</span><span class="sxs-lookup"><span data-stu-id="8d94e-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d94e-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8d94e-125">JSON Representation</span></span>
<span data-ttu-id="8d94e-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8d94e-126">Here is a JSON representation of the resource.</span></span>
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





