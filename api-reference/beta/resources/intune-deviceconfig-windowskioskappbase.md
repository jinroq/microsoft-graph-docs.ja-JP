---
title: windowskioskappbase リソースの種類
description: アプリの種類の基本クラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0247febfbeebe7fc047df4bb14a9d421b79bf01
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145298"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="220c0-103">windowskioskappbase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="220c0-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="220c0-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="220c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="220c0-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="220c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="220c0-106">アプリの種類の基本クラス</span><span class="sxs-lookup"><span data-stu-id="220c0-106">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="220c0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="220c0-107">Properties</span></span>
|<span data-ttu-id="220c0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="220c0-108">Property</span></span>|<span data-ttu-id="220c0-109">型</span><span class="sxs-lookup"><span data-stu-id="220c0-109">Type</span></span>|<span data-ttu-id="220c0-110">説明</span><span class="sxs-lookup"><span data-stu-id="220c0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="220c0-111">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="220c0-111">startLayoutTileSize</span></span>|[<span data-ttu-id="220c0-112">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="220c0-112">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="220c0-113">開始レイアウトのアプリタイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="220c0-113">The app tile size for the start layout.</span></span> <span data-ttu-id="220c0-114">可能な値は、`hidden`、`small`、`medium`、`wide`、`large` です。</span><span class="sxs-lookup"><span data-stu-id="220c0-114">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="220c0-115">name</span><span class="sxs-lookup"><span data-stu-id="220c0-115">name</span></span>|<span data-ttu-id="220c0-116">String</span><span class="sxs-lookup"><span data-stu-id="220c0-116">String</span></span>|<span data-ttu-id="220c0-117">アプリのフレンドリ名を表します。</span><span class="sxs-lookup"><span data-stu-id="220c0-117">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="220c0-118">appType</span><span class="sxs-lookup"><span data-stu-id="220c0-118">appType</span></span>|[<span data-ttu-id="220c0-119">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="220c0-119">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="220c0-120">アプリの種類。</span><span class="sxs-lookup"><span data-stu-id="220c0-120">The app type.</span></span> <span data-ttu-id="220c0-121">可能な値は、`unknown`、`store`、`desktop`、`aumId` です。</span><span class="sxs-lookup"><span data-stu-id="220c0-121">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="220c0-122">関係</span><span class="sxs-lookup"><span data-stu-id="220c0-122">Relationships</span></span>
<span data-ttu-id="220c0-123">なし</span><span class="sxs-lookup"><span data-stu-id="220c0-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="220c0-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="220c0-124">JSON Representation</span></span>
<span data-ttu-id="220c0-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="220c0-125">Here is a JSON representation of the resource.</span></span>
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




