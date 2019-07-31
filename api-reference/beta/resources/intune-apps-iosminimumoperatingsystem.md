---
title: iosMinimumOperatingSystem リソースの種類
description: iOS モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 43409d7c4f4eb7bedd4a169c5f56d969e2b9d03d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005941"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="9f056-103">iosMinimumOperatingSystem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9f056-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="9f056-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f056-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f056-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9f056-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f056-106">iOS モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="9f056-106">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="9f056-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f056-107">Properties</span></span>
|<span data-ttu-id="9f056-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f056-108">Property</span></span>|<span data-ttu-id="9f056-109">型</span><span class="sxs-lookup"><span data-stu-id="9f056-109">Type</span></span>|<span data-ttu-id="9f056-110">説明</span><span class="sxs-lookup"><span data-stu-id="9f056-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f056-111">v8_0</span><span class="sxs-lookup"><span data-stu-id="9f056-111">v8_0</span></span>|<span data-ttu-id="9f056-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f056-112">Boolean</span></span>|<span data-ttu-id="9f056-113">バージョン 8.0 以降。</span><span class="sxs-lookup"><span data-stu-id="9f056-113">Version 8.0 or later.</span></span>|
|<span data-ttu-id="9f056-114">v9_0</span><span class="sxs-lookup"><span data-stu-id="9f056-114">v9_0</span></span>|<span data-ttu-id="9f056-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f056-115">Boolean</span></span>|<span data-ttu-id="9f056-116">バージョン 9.0 以降。</span><span class="sxs-lookup"><span data-stu-id="9f056-116">Version 9.0 or later.</span></span>|
|<span data-ttu-id="9f056-117">v10_0</span><span class="sxs-lookup"><span data-stu-id="9f056-117">v10_0</span></span>|<span data-ttu-id="9f056-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f056-118">Boolean</span></span>|<span data-ttu-id="9f056-119">バージョン 10.0 以降。</span><span class="sxs-lookup"><span data-stu-id="9f056-119">Version 10.0 or later.</span></span>|
|<span data-ttu-id="9f056-120">v11_0</span><span class="sxs-lookup"><span data-stu-id="9f056-120">v11_0</span></span>|<span data-ttu-id="9f056-121">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="9f056-121">Boolean</span></span>|<span data-ttu-id="9f056-122">バージョン 11.0 以降。</span><span class="sxs-lookup"><span data-stu-id="9f056-122">Version 11.0 or later.</span></span>|
|<span data-ttu-id="9f056-123">v12_0</span><span class="sxs-lookup"><span data-stu-id="9f056-123">v12_0</span></span>|<span data-ttu-id="9f056-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f056-124">Boolean</span></span>|<span data-ttu-id="9f056-125">バージョン12.0 以降。</span><span class="sxs-lookup"><span data-stu-id="9f056-125">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f056-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9f056-126">Relationships</span></span>
<span data-ttu-id="9f056-127">なし</span><span class="sxs-lookup"><span data-stu-id="9f056-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f056-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f056-128">JSON Representation</span></span>
<span data-ttu-id="9f056-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9f056-129">Here is a JSON representation of the resource.</span></span>
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





