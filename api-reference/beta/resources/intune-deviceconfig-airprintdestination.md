---
title: airPrintDestination リソースの種類
description: AirPrint のリンク先を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3f56578427427d45a69c4c64fe9fde3cf31f8fd9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422496"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="b27b6-103">airPrintDestination リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b27b6-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="b27b6-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b27b6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b27b6-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b27b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b27b6-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b27b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b27b6-107">AirPrint のリンク先を表します。</span><span class="sxs-lookup"><span data-stu-id="b27b6-107">Represents an AirPrint destination.</span></span>

## <a name="properties"></a><span data-ttu-id="b27b6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b27b6-108">Properties</span></span>
|<span data-ttu-id="b27b6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b27b6-109">Property</span></span>|<span data-ttu-id="b27b6-110">型</span><span class="sxs-lookup"><span data-stu-id="b27b6-110">Type</span></span>|<span data-ttu-id="b27b6-111">説明</span><span class="sxs-lookup"><span data-stu-id="b27b6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b27b6-112">ipAddress</span><span class="sxs-lookup"><span data-stu-id="b27b6-112">ipAddress</span></span>|<span data-ttu-id="b27b6-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b27b6-113">String</span></span>|<span data-ttu-id="b27b6-114">AirPrint の宛先の IP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="b27b6-114">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="b27b6-115">resourcePath</span><span class="sxs-lookup"><span data-stu-id="b27b6-115">resourcePath</span></span>|<span data-ttu-id="b27b6-116">String</span><span class="sxs-lookup"><span data-stu-id="b27b6-116">String</span></span>|<span data-ttu-id="b27b6-117">プリンターに関連付けられているリソースのパスです。</span><span class="sxs-lookup"><span data-stu-id="b27b6-117">The Resource Path associated with the printer.</span></span> <span data-ttu-id="b27b6-118">これは、Bonjour のレコードの _ipps.tcp の rp のパラメーターに対応しています。</span><span class="sxs-lookup"><span data-stu-id="b27b6-118">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="b27b6-119">例: プリンター/Canon_MG5300_series、プリンター/Xerox_Phaser_7600、ipp 印刷/Epson_IPP_Printer です。</span><span class="sxs-lookup"><span data-stu-id="b27b6-119">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="b27b6-120">port</span><span class="sxs-lookup"><span data-stu-id="b27b6-120">port</span></span>|<span data-ttu-id="b27b6-121">Int32</span><span class="sxs-lookup"><span data-stu-id="b27b6-121">Int32</span></span>|<span data-ttu-id="b27b6-122">AirPrint のリンク先のリッスン ポート。</span><span class="sxs-lookup"><span data-stu-id="b27b6-122">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="b27b6-123">このキーが既定のポートは AirPrint を使用して、指定されていない場合。</span><span class="sxs-lookup"><span data-stu-id="b27b6-123">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="b27b6-124">IOS 11.0 で利用可能な後で。</span><span class="sxs-lookup"><span data-stu-id="b27b6-124">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="b27b6-125">forceTls</span><span class="sxs-lookup"><span data-stu-id="b27b6-125">forceTls</span></span>|<span data-ttu-id="b27b6-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="b27b6-126">Boolean</span></span>|<span data-ttu-id="b27b6-127">AirPrint 接続の場合は true、トランスポート層セキュリティ (TLS) によって保護されている場合。</span><span class="sxs-lookup"><span data-stu-id="b27b6-127">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="b27b6-128">既定では false を指定します。</span><span class="sxs-lookup"><span data-stu-id="b27b6-128">Default is false.</span></span> <span data-ttu-id="b27b6-129">IOS 11.0 で利用可能な後で。</span><span class="sxs-lookup"><span data-stu-id="b27b6-129">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b27b6-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b27b6-130">Relationships</span></span>
<span data-ttu-id="b27b6-131">なし</span><span class="sxs-lookup"><span data-stu-id="b27b6-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b27b6-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b27b6-132">JSON Representation</span></span>
<span data-ttu-id="b27b6-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b27b6-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.airPrintDestination"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.airPrintDestination",
  "ipAddress": "String",
  "resourcePath": "String",
  "port": 1024,
  "forceTls": true
}
```




