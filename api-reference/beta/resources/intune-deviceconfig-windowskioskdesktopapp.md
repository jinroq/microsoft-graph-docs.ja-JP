---
title: windowskioskdesktopapp リソースの種類
description: アプリの種類の基本クラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0487fa24ecd2d27817349b68063cf606a2401944
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170477"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="4497f-103">windowskioskdesktopapp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4497f-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="4497f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4497f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4497f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4497f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4497f-106">アプリの種類の基本クラス</span><span class="sxs-lookup"><span data-stu-id="4497f-106">The base class for a type of apps</span></span>


<span data-ttu-id="4497f-107">[windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="4497f-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4497f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4497f-108">Properties</span></span>
|<span data-ttu-id="4497f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4497f-109">Property</span></span>|<span data-ttu-id="4497f-110">型</span><span class="sxs-lookup"><span data-stu-id="4497f-110">Type</span></span>|<span data-ttu-id="4497f-111">説明</span><span class="sxs-lookup"><span data-stu-id="4497f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4497f-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="4497f-112">startLayoutTileSize</span></span>|[<span data-ttu-id="4497f-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="4497f-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="4497f-114">[windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承された開始レイアウトのアプリタイルサイズ。</span><span class="sxs-lookup"><span data-stu-id="4497f-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="4497f-115">可能な値は、`hidden`、`small`、`medium`、`wide`、`large` です。</span><span class="sxs-lookup"><span data-stu-id="4497f-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="4497f-116">name</span><span class="sxs-lookup"><span data-stu-id="4497f-116">name</span></span>|<span data-ttu-id="4497f-117">String</span><span class="sxs-lookup"><span data-stu-id="4497f-117">String</span></span>|<span data-ttu-id="4497f-118">[windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承されたアプリのフレンドリ名を表します。</span><span class="sxs-lookup"><span data-stu-id="4497f-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="4497f-119">appType</span><span class="sxs-lookup"><span data-stu-id="4497f-119">appType</span></span>|[<span data-ttu-id="4497f-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="4497f-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="4497f-121">[windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承されるアプリの種類。</span><span class="sxs-lookup"><span data-stu-id="4497f-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="4497f-122">使用可能な値は、`unknown`、`store`、`desktop`、`aumId` です。</span><span class="sxs-lookup"><span data-stu-id="4497f-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="4497f-123">path</span><span class="sxs-lookup"><span data-stu-id="4497f-123">path</span></span>|<span data-ttu-id="4497f-124">String</span><span class="sxs-lookup"><span data-stu-id="4497f-124">String</span></span>|<span data-ttu-id="4497f-125">デスクトップアプリのパスの定義</span><span class="sxs-lookup"><span data-stu-id="4497f-125">Define the path of a desktop app</span></span>|
|<span data-ttu-id="4497f-126">desktopapplicationid</span><span class="sxs-lookup"><span data-stu-id="4497f-126">desktopApplicationId</span></span>|<span data-ttu-id="4497f-127">String</span><span class="sxs-lookup"><span data-stu-id="4497f-127">String</span></span>|<span data-ttu-id="4497f-128">アプリの desktopapplicationid を定義する</span><span class="sxs-lookup"><span data-stu-id="4497f-128">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="4497f-129">desktopapplicationlinkpath</span><span class="sxs-lookup"><span data-stu-id="4497f-129">desktopApplicationLinkPath</span></span>|<span data-ttu-id="4497f-130">String</span><span class="sxs-lookup"><span data-stu-id="4497f-130">String</span></span>|<span data-ttu-id="4497f-131">アプリの desktopapplicationlinkpath を定義する</span><span class="sxs-lookup"><span data-stu-id="4497f-131">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="4497f-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4497f-132">Relationships</span></span>
<span data-ttu-id="4497f-133">なし</span><span class="sxs-lookup"><span data-stu-id="4497f-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4497f-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4497f-134">JSON Representation</span></span>
<span data-ttu-id="4497f-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4497f-135">Here is a JSON representation of the resource.</span></span>
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
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```




