---
title: windowsKioskAppBase リソースの種類
description: アプリケーションの型の基本クラス
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8ca86969eb32a1a1d129fb5ba4cd48bbb04ffd78
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407145"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="b43e6-103">windowsKioskAppBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b43e6-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="b43e6-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b43e6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b43e6-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b43e6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b43e6-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b43e6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b43e6-107">アプリケーションの型の基本クラス</span><span class="sxs-lookup"><span data-stu-id="b43e6-107">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="b43e6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b43e6-108">Properties</span></span>
|<span data-ttu-id="b43e6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b43e6-109">Property</span></span>|<span data-ttu-id="b43e6-110">型</span><span class="sxs-lookup"><span data-stu-id="b43e6-110">Type</span></span>|<span data-ttu-id="b43e6-111">説明</span><span class="sxs-lookup"><span data-stu-id="b43e6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b43e6-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="b43e6-112">startLayoutTileSize</span></span>|[<span data-ttu-id="b43e6-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="b43e6-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="b43e6-114">開始レイアウトのアプリケーションのタイルのサイズです。</span><span class="sxs-lookup"><span data-stu-id="b43e6-114">The app tile size for the start layout.</span></span> <span data-ttu-id="b43e6-115">可能な値は、`hidden`、`small`、`medium`、`wide`、`large` です。</span><span class="sxs-lookup"><span data-stu-id="b43e6-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="b43e6-116">name</span><span class="sxs-lookup"><span data-stu-id="b43e6-116">name</span></span>|<span data-ttu-id="b43e6-117">String</span><span class="sxs-lookup"><span data-stu-id="b43e6-117">String</span></span>|<span data-ttu-id="b43e6-118">アプリケーションのフレンドリ名を表す</span><span class="sxs-lookup"><span data-stu-id="b43e6-118">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="b43e6-119">appType</span><span class="sxs-lookup"><span data-stu-id="b43e6-119">appType</span></span>|[<span data-ttu-id="b43e6-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="b43e6-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="b43e6-121">アプリケーションの種類です。</span><span class="sxs-lookup"><span data-stu-id="b43e6-121">The app type.</span></span> <span data-ttu-id="b43e6-122">可能な値は、`unknown`、`store`、`desktop`、`aumId` です。</span><span class="sxs-lookup"><span data-stu-id="b43e6-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b43e6-123">関係</span><span class="sxs-lookup"><span data-stu-id="b43e6-123">Relationships</span></span>
<span data-ttu-id="b43e6-124">なし</span><span class="sxs-lookup"><span data-stu-id="b43e6-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b43e6-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b43e6-125">JSON Representation</span></span>
<span data-ttu-id="b43e6-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b43e6-126">Here is a JSON representation of the resource.</span></span>
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
  "appType": "String"
}
```




