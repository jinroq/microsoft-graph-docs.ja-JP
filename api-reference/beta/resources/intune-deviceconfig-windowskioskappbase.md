---
title: windowsKioskAppBase リソースの種類
description: アプリの種類の基本クラス
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 93884a53ce20f67fadbd60fa2a8f180aba8fa826
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944090"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="2c0f5-103">windowsKioskAppBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2c0f5-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="2c0f5-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2c0f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c0f5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2c0f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c0f5-106">アプリの種類の基本クラス</span><span class="sxs-lookup"><span data-stu-id="2c0f5-106">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="2c0f5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c0f5-107">Properties</span></span>
|<span data-ttu-id="2c0f5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c0f5-108">Property</span></span>|<span data-ttu-id="2c0f5-109">型</span><span class="sxs-lookup"><span data-stu-id="2c0f5-109">Type</span></span>|<span data-ttu-id="2c0f5-110">説明</span><span class="sxs-lookup"><span data-stu-id="2c0f5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c0f5-111">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="2c0f5-111">startLayoutTileSize</span></span>|[<span data-ttu-id="2c0f5-112">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="2c0f5-112">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="2c0f5-113">開始レイアウトのアプリタイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="2c0f5-113">The app tile size for the start layout.</span></span> <span data-ttu-id="2c0f5-114">可能な値は、`hidden`、`small`、`medium`、`wide`、`large` です。</span><span class="sxs-lookup"><span data-stu-id="2c0f5-114">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="2c0f5-115">name</span><span class="sxs-lookup"><span data-stu-id="2c0f5-115">name</span></span>|<span data-ttu-id="2c0f5-116">String</span><span class="sxs-lookup"><span data-stu-id="2c0f5-116">String</span></span>|<span data-ttu-id="2c0f5-117">アプリのフレンドリ名を表します。</span><span class="sxs-lookup"><span data-stu-id="2c0f5-117">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="2c0f5-118">appType</span><span class="sxs-lookup"><span data-stu-id="2c0f5-118">appType</span></span>|[<span data-ttu-id="2c0f5-119">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="2c0f5-119">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="2c0f5-120">アプリの種類。</span><span class="sxs-lookup"><span data-stu-id="2c0f5-120">The app type.</span></span> <span data-ttu-id="2c0f5-121">使用可能な値は、`unknown`、`store`、`desktop`、`aumId` です。</span><span class="sxs-lookup"><span data-stu-id="2c0f5-121">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="2c0f5-122">autoLaunch</span><span class="sxs-lookup"><span data-stu-id="2c0f5-122">autoLaunch</span></span>|<span data-ttu-id="2c0f5-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c0f5-123">Boolean</span></span>|<span data-ttu-id="2c0f5-124">アプリをマルチアプリキオスクモードで自動起動できるようにする</span><span class="sxs-lookup"><span data-stu-id="2c0f5-124">Allow the app to be auto-launched in multi-app kiosk mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c0f5-125">関係</span><span class="sxs-lookup"><span data-stu-id="2c0f5-125">Relationships</span></span>
<span data-ttu-id="2c0f5-126">なし</span><span class="sxs-lookup"><span data-stu-id="2c0f5-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c0f5-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2c0f5-127">JSON Representation</span></span>
<span data-ttu-id="2c0f5-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2c0f5-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAppBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAppBase",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true
}
```




