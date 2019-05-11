---
title: windowsKioskDesktopApp リソースの種類
description: アプリの種類の基本クラス
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a1541b12754307844e89a06c02ab78081856ee4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943887"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="88f61-103">windowsKioskDesktopApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="88f61-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="88f61-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88f61-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88f61-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="88f61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88f61-106">アプリの種類の基本クラス</span><span class="sxs-lookup"><span data-stu-id="88f61-106">The base class for a type of apps</span></span>


<span data-ttu-id="88f61-107">[Windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="88f61-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="88f61-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88f61-108">Properties</span></span>
|<span data-ttu-id="88f61-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88f61-109">Property</span></span>|<span data-ttu-id="88f61-110">型</span><span class="sxs-lookup"><span data-stu-id="88f61-110">Type</span></span>|<span data-ttu-id="88f61-111">説明</span><span class="sxs-lookup"><span data-stu-id="88f61-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88f61-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="88f61-112">startLayoutTileSize</span></span>|[<span data-ttu-id="88f61-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="88f61-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="88f61-114">[Windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承された開始レイアウトのアプリタイルサイズ。</span><span class="sxs-lookup"><span data-stu-id="88f61-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="88f61-115">可能な値は、`hidden`、`small`、`medium`、`wide`、`large` です。</span><span class="sxs-lookup"><span data-stu-id="88f61-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="88f61-116">name</span><span class="sxs-lookup"><span data-stu-id="88f61-116">name</span></span>|<span data-ttu-id="88f61-117">String</span><span class="sxs-lookup"><span data-stu-id="88f61-117">String</span></span>|<span data-ttu-id="88f61-118">[Windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承されたアプリのフレンドリ名を表します。</span><span class="sxs-lookup"><span data-stu-id="88f61-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="88f61-119">appType</span><span class="sxs-lookup"><span data-stu-id="88f61-119">appType</span></span>|[<span data-ttu-id="88f61-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="88f61-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="88f61-121">[Windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承されるアプリの種類。</span><span class="sxs-lookup"><span data-stu-id="88f61-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="88f61-122">使用可能な値は、`unknown`、`store`、`desktop`、`aumId` です。</span><span class="sxs-lookup"><span data-stu-id="88f61-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="88f61-123">autoLaunch</span><span class="sxs-lookup"><span data-stu-id="88f61-123">autoLaunch</span></span>|<span data-ttu-id="88f61-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="88f61-124">Boolean</span></span>|<span data-ttu-id="88f61-125">[Windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承されたマルチアプリキオスクモードでアプリを自動起動することを許可します。</span><span class="sxs-lookup"><span data-stu-id="88f61-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="88f61-126">path</span><span class="sxs-lookup"><span data-stu-id="88f61-126">path</span></span>|<span data-ttu-id="88f61-127">String</span><span class="sxs-lookup"><span data-stu-id="88f61-127">String</span></span>|<span data-ttu-id="88f61-128">デスクトップアプリのパスの定義</span><span class="sxs-lookup"><span data-stu-id="88f61-128">Define the path of a desktop app</span></span>|
|<span data-ttu-id="88f61-129">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="88f61-129">desktopApplicationId</span></span>|<span data-ttu-id="88f61-130">String</span><span class="sxs-lookup"><span data-stu-id="88f61-130">String</span></span>|<span data-ttu-id="88f61-131">アプリの DesktopApplicationID を定義する</span><span class="sxs-lookup"><span data-stu-id="88f61-131">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="88f61-132">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="88f61-132">desktopApplicationLinkPath</span></span>|<span data-ttu-id="88f61-133">String</span><span class="sxs-lookup"><span data-stu-id="88f61-133">String</span></span>|<span data-ttu-id="88f61-134">アプリの DesktopApplicationLinkPath を定義する</span><span class="sxs-lookup"><span data-stu-id="88f61-134">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="88f61-135">関係</span><span class="sxs-lookup"><span data-stu-id="88f61-135">Relationships</span></span>
<span data-ttu-id="88f61-136">なし</span><span class="sxs-lookup"><span data-stu-id="88f61-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88f61-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="88f61-137">JSON Representation</span></span>
<span data-ttu-id="88f61-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="88f61-138">Here is a JSON representation of the resource.</span></span>
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




