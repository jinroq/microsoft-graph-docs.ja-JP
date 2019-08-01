---
title: windowsMinimumOperatingSystem リソースの種類
description: Windows モバイル アプリに必要な最小オペレーティング システム。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a92d02f6994a7cd18ba44c7da5b43768e87fc61a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032075"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="023f5-103">windowsMinimumOperatingSystem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="023f5-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="023f5-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="023f5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="023f5-105">Windows モバイル アプリに必要な最小オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="023f5-105">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="023f5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="023f5-106">Properties</span></span>
|<span data-ttu-id="023f5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="023f5-107">Property</span></span>|<span data-ttu-id="023f5-108">型</span><span class="sxs-lookup"><span data-stu-id="023f5-108">Type</span></span>|<span data-ttu-id="023f5-109">説明</span><span class="sxs-lookup"><span data-stu-id="023f5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="023f5-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="023f5-110">v8_0</span></span>|<span data-ttu-id="023f5-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="023f5-111">Boolean</span></span>|<span data-ttu-id="023f5-112">Windows バージョン 8.0 以降。</span><span class="sxs-lookup"><span data-stu-id="023f5-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="023f5-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="023f5-113">v8_1</span></span>|<span data-ttu-id="023f5-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="023f5-114">Boolean</span></span>|<span data-ttu-id="023f5-115">Windows バージョン 8.1 以降。</span><span class="sxs-lookup"><span data-stu-id="023f5-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="023f5-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="023f5-116">v10_0</span></span>|<span data-ttu-id="023f5-117">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="023f5-117">Boolean</span></span>|<span data-ttu-id="023f5-118">Windows バージョン 10.0 以降。</span><span class="sxs-lookup"><span data-stu-id="023f5-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="023f5-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="023f5-119">Relationships</span></span>
<span data-ttu-id="023f5-120">なし</span><span class="sxs-lookup"><span data-stu-id="023f5-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="023f5-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="023f5-121">JSON Representation</span></span>
<span data-ttu-id="023f5-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="023f5-122">Here is a JSON representation of the resource.</span></span>
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



