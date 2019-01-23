---
title: windowsKioskUWPApp リソースの種類
description: アプリケーションの型の基本クラス
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7ba5367721890f02af3b348ad469b15024de4800
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392683"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="c836c-103">windowsKioskUWPApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c836c-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="c836c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c836c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c836c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c836c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c836c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c836c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c836c-107">アプリケーションの型の基本クラス</span><span class="sxs-lookup"><span data-stu-id="c836c-107">The base class for a type of apps</span></span>


<span data-ttu-id="c836c-108">[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c836c-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c836c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c836c-109">Properties</span></span>
|<span data-ttu-id="c836c-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c836c-110">Property</span></span>|<span data-ttu-id="c836c-111">型</span><span class="sxs-lookup"><span data-stu-id="c836c-111">Type</span></span>|<span data-ttu-id="c836c-112">説明</span><span class="sxs-lookup"><span data-stu-id="c836c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c836c-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="c836c-113">startLayoutTileSize</span></span>|[<span data-ttu-id="c836c-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="c836c-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="c836c-115">[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承される開始レイアウトのアプリケーションのタイルのサイズです。</span><span class="sxs-lookup"><span data-stu-id="c836c-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="c836c-116">可能な値は、`hidden`、`small`、`medium`、`wide`、`large` です。</span><span class="sxs-lookup"><span data-stu-id="c836c-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="c836c-117">name</span><span class="sxs-lookup"><span data-stu-id="c836c-117">name</span></span>|<span data-ttu-id="c836c-118">String</span><span class="sxs-lookup"><span data-stu-id="c836c-118">String</span></span>|<span data-ttu-id="c836c-119">[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承される、アプリケーションのフレンドリ名を表す</span><span class="sxs-lookup"><span data-stu-id="c836c-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="c836c-120">appType</span><span class="sxs-lookup"><span data-stu-id="c836c-120">appType</span></span>|[<span data-ttu-id="c836c-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="c836c-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="c836c-122">[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)からアプリケーション型継承します。</span><span class="sxs-lookup"><span data-stu-id="c836c-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="c836c-123">可能な値は、`unknown`、`store`、`desktop`、`aumId` です。</span><span class="sxs-lookup"><span data-stu-id="c836c-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="c836c-124">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="c836c-124">appUserModelId</span></span>|<span data-ttu-id="c836c-125">String</span><span class="sxs-lookup"><span data-stu-id="c836c-125">String</span></span>|<span data-ttu-id="c836c-126">これは、専用アプリケーション ユーザー モデル ID (AUMID) を表示するキオスク モードでの使用を開始するのには、します。</span><span class="sxs-lookup"><span data-stu-id="c836c-126">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="c836c-127">appId</span><span class="sxs-lookup"><span data-stu-id="c836c-127">appId</span></span>|<span data-ttu-id="c836c-128">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c836c-128">String</span></span>|<span data-ttu-id="c836c-129">Intune キオスクの構成と同じ割り当ての対象となるアプリケーションを参照してこの</span><span class="sxs-lookup"><span data-stu-id="c836c-129">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="c836c-130">containedAppId</span><span class="sxs-lookup"><span data-stu-id="c836c-130">containedAppId</span></span>|<span data-ttu-id="c836c-131">String</span><span class="sxs-lookup"><span data-stu-id="c836c-131">String</span></span>|<span data-ttu-id="c836c-132">Intune アプリから含まれているアプリケーションを参照してこの</span><span class="sxs-lookup"><span data-stu-id="c836c-132">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="c836c-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c836c-133">Relationships</span></span>
<span data-ttu-id="c836c-134">なし</span><span class="sxs-lookup"><span data-stu-id="c836c-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c836c-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c836c-135">JSON Representation</span></span>
<span data-ttu-id="c836c-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c836c-136">Here is a JSON representation of the resource.</span></span>
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




