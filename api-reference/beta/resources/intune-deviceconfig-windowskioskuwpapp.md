---
title: windowsKioskUWPApp リソースの種類
description: アプリの種類の基本クラス
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9858cbf11ea6f3ef507e285684bf1413a6ebce10
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968849"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="11f0d-103">windowsKioskUWPApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="11f0d-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="11f0d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11f0d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11f0d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="11f0d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11f0d-106">アプリの種類の基本クラス</span><span class="sxs-lookup"><span data-stu-id="11f0d-106">The base class for a type of apps</span></span>


<span data-ttu-id="11f0d-107">[Windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="11f0d-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="11f0d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="11f0d-108">Properties</span></span>
|<span data-ttu-id="11f0d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="11f0d-109">Property</span></span>|<span data-ttu-id="11f0d-110">型</span><span class="sxs-lookup"><span data-stu-id="11f0d-110">Type</span></span>|<span data-ttu-id="11f0d-111">説明</span><span class="sxs-lookup"><span data-stu-id="11f0d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11f0d-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="11f0d-112">startLayoutTileSize</span></span>|[<span data-ttu-id="11f0d-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="11f0d-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="11f0d-114">[Windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承された開始レイアウトのアプリタイルサイズ。</span><span class="sxs-lookup"><span data-stu-id="11f0d-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="11f0d-115">可能な値は、`hidden`、`small`、`medium`、`wide`、`large` です。</span><span class="sxs-lookup"><span data-stu-id="11f0d-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="11f0d-116">name</span><span class="sxs-lookup"><span data-stu-id="11f0d-116">name</span></span>|<span data-ttu-id="11f0d-117">String</span><span class="sxs-lookup"><span data-stu-id="11f0d-117">String</span></span>|<span data-ttu-id="11f0d-118">[Windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承されたアプリのフレンドリ名を表します。</span><span class="sxs-lookup"><span data-stu-id="11f0d-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="11f0d-119">appType</span><span class="sxs-lookup"><span data-stu-id="11f0d-119">appType</span></span>|[<span data-ttu-id="11f0d-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="11f0d-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="11f0d-121">[Windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承されるアプリの種類。</span><span class="sxs-lookup"><span data-stu-id="11f0d-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="11f0d-122">使用可能な値は、`unknown`、`store`、`desktop`、`aumId` です。</span><span class="sxs-lookup"><span data-stu-id="11f0d-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="11f0d-123">autoLaunch</span><span class="sxs-lookup"><span data-stu-id="11f0d-123">autoLaunch</span></span>|<span data-ttu-id="11f0d-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="11f0d-124">Boolean</span></span>|<span data-ttu-id="11f0d-125">[Windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承されたマルチアプリキオスクモードでアプリを自動起動することを許可します。</span><span class="sxs-lookup"><span data-stu-id="11f0d-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="11f0d-126">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="11f0d-126">appUserModelId</span></span>|<span data-ttu-id="11f0d-127">String</span><span class="sxs-lookup"><span data-stu-id="11f0d-127">String</span></span>|<span data-ttu-id="11f0d-128">これは、キオスクモードでの使用が可能になる唯一のアプリケーションユーザーモデル ID (AUMID) です。</span><span class="sxs-lookup"><span data-stu-id="11f0d-128">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="11f0d-129">appId</span><span class="sxs-lookup"><span data-stu-id="11f0d-129">appId</span></span>|<span data-ttu-id="11f0d-130">String</span><span class="sxs-lookup"><span data-stu-id="11f0d-130">String</span></span>|<span data-ttu-id="11f0d-131">これは、キオスクの構成と同じ割り当てに移行する Intune アプリを参照します。</span><span class="sxs-lookup"><span data-stu-id="11f0d-131">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="11f0d-132">containedAppId</span><span class="sxs-lookup"><span data-stu-id="11f0d-132">containedAppId</span></span>|<span data-ttu-id="11f0d-133">String</span><span class="sxs-lookup"><span data-stu-id="11f0d-133">String</span></span>|<span data-ttu-id="11f0d-134">これは、Intune アプリからの含まれているアプリを参照します。</span><span class="sxs-lookup"><span data-stu-id="11f0d-134">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="11f0d-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="11f0d-135">Relationships</span></span>
<span data-ttu-id="11f0d-136">なし</span><span class="sxs-lookup"><span data-stu-id="11f0d-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11f0d-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="11f0d-137">JSON Representation</span></span>
<span data-ttu-id="11f0d-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="11f0d-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskUWPApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```





