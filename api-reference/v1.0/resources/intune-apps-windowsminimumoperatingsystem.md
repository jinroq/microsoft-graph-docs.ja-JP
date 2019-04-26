---
title: windowsMinimumOperatingSystem リソースの種類
description: Windows モバイル アプリに必要な最小オペレーティング システム。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f337a61f3a0cfd52e042e65bb3d8de57dcf9f283
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571710"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="97d97-103">windowsMinimumOperatingSystem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="97d97-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="97d97-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="97d97-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97d97-105">Windows モバイル アプリに必要な最小オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="97d97-105">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="97d97-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97d97-106">Properties</span></span>
|<span data-ttu-id="97d97-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97d97-107">Property</span></span>|<span data-ttu-id="97d97-108">型</span><span class="sxs-lookup"><span data-stu-id="97d97-108">Type</span></span>|<span data-ttu-id="97d97-109">説明</span><span class="sxs-lookup"><span data-stu-id="97d97-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97d97-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="97d97-110">v8_0</span></span>|<span data-ttu-id="97d97-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="97d97-111">Boolean</span></span>|<span data-ttu-id="97d97-112">Windows バージョン 8.0 以降。</span><span class="sxs-lookup"><span data-stu-id="97d97-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="97d97-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="97d97-113">v8_1</span></span>|<span data-ttu-id="97d97-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="97d97-114">Boolean</span></span>|<span data-ttu-id="97d97-115">Windows バージョン 8.1 以降。</span><span class="sxs-lookup"><span data-stu-id="97d97-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="97d97-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="97d97-116">v10_0</span></span>|<span data-ttu-id="97d97-117">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="97d97-117">Boolean</span></span>|<span data-ttu-id="97d97-118">Windows バージョン 10.0 以降。</span><span class="sxs-lookup"><span data-stu-id="97d97-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97d97-119">関係</span><span class="sxs-lookup"><span data-stu-id="97d97-119">Relationships</span></span>
<span data-ttu-id="97d97-120">なし</span><span class="sxs-lookup"><span data-stu-id="97d97-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97d97-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="97d97-121">JSON Representation</span></span>
<span data-ttu-id="97d97-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="97d97-122">Here is a JSON representation of the resource.</span></span>
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



