---
title: windowsKioskDesktopApp リソースの種類
description: アプリケーションの型の基本クラス
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 831ed86da24791cde549687ecaff42cabc29a99e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415307"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="0fa27-103">windowsKioskDesktopApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0fa27-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="0fa27-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0fa27-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0fa27-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0fa27-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0fa27-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0fa27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fa27-107">アプリケーションの型の基本クラス</span><span class="sxs-lookup"><span data-stu-id="0fa27-107">The base class for a type of apps</span></span>


<span data-ttu-id="0fa27-108">[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0fa27-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0fa27-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0fa27-109">Properties</span></span>
|<span data-ttu-id="0fa27-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0fa27-110">Property</span></span>|<span data-ttu-id="0fa27-111">型</span><span class="sxs-lookup"><span data-stu-id="0fa27-111">Type</span></span>|<span data-ttu-id="0fa27-112">説明</span><span class="sxs-lookup"><span data-stu-id="0fa27-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fa27-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="0fa27-113">startLayoutTileSize</span></span>|[<span data-ttu-id="0fa27-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="0fa27-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="0fa27-115">[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承される開始レイアウトのアプリケーションのタイルのサイズです。</span><span class="sxs-lookup"><span data-stu-id="0fa27-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="0fa27-116">可能な値は、`hidden`、`small`、`medium`、`wide`、`large` です。</span><span class="sxs-lookup"><span data-stu-id="0fa27-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="0fa27-117">name</span><span class="sxs-lookup"><span data-stu-id="0fa27-117">name</span></span>|<span data-ttu-id="0fa27-118">String</span><span class="sxs-lookup"><span data-stu-id="0fa27-118">String</span></span>|<span data-ttu-id="0fa27-119">[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承される、アプリケーションのフレンドリ名を表す</span><span class="sxs-lookup"><span data-stu-id="0fa27-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="0fa27-120">appType</span><span class="sxs-lookup"><span data-stu-id="0fa27-120">appType</span></span>|[<span data-ttu-id="0fa27-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="0fa27-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="0fa27-122">[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)からアプリケーション型継承します。</span><span class="sxs-lookup"><span data-stu-id="0fa27-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="0fa27-123">可能な値は、`unknown`、`store`、`desktop`、`aumId` です。</span><span class="sxs-lookup"><span data-stu-id="0fa27-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="0fa27-124">path</span><span class="sxs-lookup"><span data-stu-id="0fa27-124">path</span></span>|<span data-ttu-id="0fa27-125">String</span><span class="sxs-lookup"><span data-stu-id="0fa27-125">String</span></span>|<span data-ttu-id="0fa27-126">デスクトップ アプリケーションのパスを定義します。</span><span class="sxs-lookup"><span data-stu-id="0fa27-126">Define the path of a desktop app</span></span>|
|<span data-ttu-id="0fa27-127">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="0fa27-127">desktopApplicationId</span></span>|<span data-ttu-id="0fa27-128">String</span><span class="sxs-lookup"><span data-stu-id="0fa27-128">String</span></span>|<span data-ttu-id="0fa27-129">アプリケーションの DesktopApplicationID を定義します。</span><span class="sxs-lookup"><span data-stu-id="0fa27-129">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="0fa27-130">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="0fa27-130">desktopApplicationLinkPath</span></span>|<span data-ttu-id="0fa27-131">String</span><span class="sxs-lookup"><span data-stu-id="0fa27-131">String</span></span>|<span data-ttu-id="0fa27-132">アプリケーションの DesktopApplicationLinkPath を定義します。</span><span class="sxs-lookup"><span data-stu-id="0fa27-132">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fa27-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0fa27-133">Relationships</span></span>
<span data-ttu-id="0fa27-134">なし</span><span class="sxs-lookup"><span data-stu-id="0fa27-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0fa27-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0fa27-135">JSON Representation</span></span>
<span data-ttu-id="0fa27-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0fa27-136">Here is a JSON representation of the resource.</span></span>
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




