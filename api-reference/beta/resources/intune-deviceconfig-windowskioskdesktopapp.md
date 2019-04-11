---
title: windowskioskdesktopapp リソースの種類
description: アプリの種類の基本クラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 89f309b53e44b0f2843145dd7c0f4d3ffa6d7f98
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805216"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="eb865-103">windowskioskdesktopapp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eb865-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="eb865-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb865-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb865-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eb865-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb865-106">アプリの種類の基本クラス</span><span class="sxs-lookup"><span data-stu-id="eb865-106">The base class for a type of apps</span></span>


<span data-ttu-id="eb865-107">[windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="eb865-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eb865-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb865-108">Properties</span></span>
|<span data-ttu-id="eb865-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb865-109">Property</span></span>|<span data-ttu-id="eb865-110">型</span><span class="sxs-lookup"><span data-stu-id="eb865-110">Type</span></span>|<span data-ttu-id="eb865-111">説明</span><span class="sxs-lookup"><span data-stu-id="eb865-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb865-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="eb865-112">startLayoutTileSize</span></span>|[<span data-ttu-id="eb865-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="eb865-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="eb865-114">[windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承された開始レイアウトのアプリタイルサイズ。</span><span class="sxs-lookup"><span data-stu-id="eb865-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="eb865-115">可能な値は、`hidden`、`small`、`medium`、`wide`、`large` です。</span><span class="sxs-lookup"><span data-stu-id="eb865-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="eb865-116">name</span><span class="sxs-lookup"><span data-stu-id="eb865-116">name</span></span>|<span data-ttu-id="eb865-117">String</span><span class="sxs-lookup"><span data-stu-id="eb865-117">String</span></span>|<span data-ttu-id="eb865-118">[windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承されたアプリのフレンドリ名を表します。</span><span class="sxs-lookup"><span data-stu-id="eb865-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="eb865-119">appType</span><span class="sxs-lookup"><span data-stu-id="eb865-119">appType</span></span>|[<span data-ttu-id="eb865-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="eb865-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="eb865-121">[windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承されるアプリの種類。</span><span class="sxs-lookup"><span data-stu-id="eb865-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="eb865-122">可能な値は、`unknown`、`store`、`desktop`、`aumId` です。</span><span class="sxs-lookup"><span data-stu-id="eb865-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="eb865-123">autoLaunch</span><span class="sxs-lookup"><span data-stu-id="eb865-123">autoLaunch</span></span>|<span data-ttu-id="eb865-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb865-124">Boolean</span></span>|<span data-ttu-id="eb865-125">[windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承されたマルチアプリキオスクモードでアプリを自動起動することを許可します。</span><span class="sxs-lookup"><span data-stu-id="eb865-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="eb865-126">path</span><span class="sxs-lookup"><span data-stu-id="eb865-126">path</span></span>|<span data-ttu-id="eb865-127">String</span><span class="sxs-lookup"><span data-stu-id="eb865-127">String</span></span>|<span data-ttu-id="eb865-128">デスクトップアプリのパスの定義</span><span class="sxs-lookup"><span data-stu-id="eb865-128">Define the path of a desktop app</span></span>|
|<span data-ttu-id="eb865-129">desktopapplicationid</span><span class="sxs-lookup"><span data-stu-id="eb865-129">desktopApplicationId</span></span>|<span data-ttu-id="eb865-130">文字列</span><span class="sxs-lookup"><span data-stu-id="eb865-130">String</span></span>|<span data-ttu-id="eb865-131">アプリの desktopapplicationid を定義する</span><span class="sxs-lookup"><span data-stu-id="eb865-131">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="eb865-132">desktopapplicationlinkpath</span><span class="sxs-lookup"><span data-stu-id="eb865-132">desktopApplicationLinkPath</span></span>|<span data-ttu-id="eb865-133">文字列</span><span class="sxs-lookup"><span data-stu-id="eb865-133">String</span></span>|<span data-ttu-id="eb865-134">アプリの desktopapplicationlinkpath を定義する</span><span class="sxs-lookup"><span data-stu-id="eb865-134">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb865-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="eb865-135">Relationships</span></span>
<span data-ttu-id="eb865-136">なし</span><span class="sxs-lookup"><span data-stu-id="eb865-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb865-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eb865-137">JSON Representation</span></span>
<span data-ttu-id="eb865-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eb865-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskDesktopApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```





