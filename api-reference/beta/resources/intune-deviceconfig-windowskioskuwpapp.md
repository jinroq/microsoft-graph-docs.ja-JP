---
title: windowsKioskUWPApp リソースの種類
description: アプリの種類の基本クラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1dbaf8dfd7f2cd488de37378f934ca3f31daedd6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147328"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="eb554-103">windowsKioskUWPApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eb554-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="eb554-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb554-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb554-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eb554-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb554-106">アプリの種類の基本クラス</span><span class="sxs-lookup"><span data-stu-id="eb554-106">The base class for a type of apps</span></span>


<span data-ttu-id="eb554-107">[windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="eb554-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eb554-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb554-108">Properties</span></span>
|<span data-ttu-id="eb554-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb554-109">Property</span></span>|<span data-ttu-id="eb554-110">型</span><span class="sxs-lookup"><span data-stu-id="eb554-110">Type</span></span>|<span data-ttu-id="eb554-111">説明</span><span class="sxs-lookup"><span data-stu-id="eb554-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb554-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="eb554-112">startLayoutTileSize</span></span>|[<span data-ttu-id="eb554-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="eb554-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="eb554-114">[windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承された開始レイアウトのアプリタイルサイズ。</span><span class="sxs-lookup"><span data-stu-id="eb554-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="eb554-115">可能な値は、`hidden`、`small`、`medium`、`wide`、`large` です。</span><span class="sxs-lookup"><span data-stu-id="eb554-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="eb554-116">name</span><span class="sxs-lookup"><span data-stu-id="eb554-116">name</span></span>|<span data-ttu-id="eb554-117">String</span><span class="sxs-lookup"><span data-stu-id="eb554-117">String</span></span>|<span data-ttu-id="eb554-118">[windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承されたアプリのフレンドリ名を表します。</span><span class="sxs-lookup"><span data-stu-id="eb554-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="eb554-119">appType</span><span class="sxs-lookup"><span data-stu-id="eb554-119">appType</span></span>|[<span data-ttu-id="eb554-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="eb554-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="eb554-121">[windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承されるアプリの種類。</span><span class="sxs-lookup"><span data-stu-id="eb554-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="eb554-122">使用可能な値は、`unknown`、`store`、`desktop`、`aumId` です。</span><span class="sxs-lookup"><span data-stu-id="eb554-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="eb554-123">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="eb554-123">appUserModelId</span></span>|<span data-ttu-id="eb554-124">String</span><span class="sxs-lookup"><span data-stu-id="eb554-124">String</span></span>|<span data-ttu-id="eb554-125">これは、キオスクモードでの使用が可能になる唯一のアプリケーションユーザーモデル ID (AUMID) です。</span><span class="sxs-lookup"><span data-stu-id="eb554-125">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="eb554-126">appId</span><span class="sxs-lookup"><span data-stu-id="eb554-126">appId</span></span>|<span data-ttu-id="eb554-127">String</span><span class="sxs-lookup"><span data-stu-id="eb554-127">String</span></span>|<span data-ttu-id="eb554-128">これは、キオスクの構成と同じ割り当てに移行する Intune アプリを参照します。</span><span class="sxs-lookup"><span data-stu-id="eb554-128">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="eb554-129">containedAppId</span><span class="sxs-lookup"><span data-stu-id="eb554-129">containedAppId</span></span>|<span data-ttu-id="eb554-130">String</span><span class="sxs-lookup"><span data-stu-id="eb554-130">String</span></span>|<span data-ttu-id="eb554-131">これは、Intune アプリからの含まれているアプリを参照します。</span><span class="sxs-lookup"><span data-stu-id="eb554-131">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb554-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="eb554-132">Relationships</span></span>
<span data-ttu-id="eb554-133">なし</span><span class="sxs-lookup"><span data-stu-id="eb554-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb554-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eb554-134">JSON Representation</span></span>
<span data-ttu-id="eb554-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eb554-135">Here is a JSON representation of the resource.</span></span>
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
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```




