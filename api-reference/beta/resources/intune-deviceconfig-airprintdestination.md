---
title: airPrintDestination リソースの種類
description: AirPrint のリンク先を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ede4f580557e75d206e0b429069acb13f81bcc5f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962514"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="f11c3-103">airPrintDestination リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f11c3-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="f11c3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f11c3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f11c3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f11c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f11c3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f11c3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f11c3-107">AirPrint のリンク先を表します。</span><span class="sxs-lookup"><span data-stu-id="f11c3-107">Represents an AirPrint destination.</span></span>
## <a name="properties"></a><span data-ttu-id="f11c3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f11c3-108">Properties</span></span>
|<span data-ttu-id="f11c3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f11c3-109">Property</span></span>|<span data-ttu-id="f11c3-110">種類</span><span class="sxs-lookup"><span data-stu-id="f11c3-110">Type</span></span>|<span data-ttu-id="f11c3-111">説明</span><span class="sxs-lookup"><span data-stu-id="f11c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f11c3-112">ipAddress</span><span class="sxs-lookup"><span data-stu-id="f11c3-112">ipAddress</span></span>|<span data-ttu-id="f11c3-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f11c3-113">String</span></span>|<span data-ttu-id="f11c3-114">AirPrint の宛先の IP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="f11c3-114">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="f11c3-115">resourcePath</span><span class="sxs-lookup"><span data-stu-id="f11c3-115">resourcePath</span></span>|<span data-ttu-id="f11c3-116">String</span><span class="sxs-lookup"><span data-stu-id="f11c3-116">String</span></span>|<span data-ttu-id="f11c3-117">プリンターに関連付けられているリソースのパスです。</span><span class="sxs-lookup"><span data-stu-id="f11c3-117">The Resource Path associated with the printer.</span></span> <span data-ttu-id="f11c3-118">これは、Bonjour のレコードの _ipps.tcp の rp のパラメーターに対応しています。</span><span class="sxs-lookup"><span data-stu-id="f11c3-118">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="f11c3-119">例: プリンター/Canon_MG5300_series、プリンター/Xerox_Phaser_7600、ipp 印刷/Epson_IPP_Printer です。</span><span class="sxs-lookup"><span data-stu-id="f11c3-119">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="f11c3-120">port</span><span class="sxs-lookup"><span data-stu-id="f11c3-120">port</span></span>|<span data-ttu-id="f11c3-121">Int32</span><span class="sxs-lookup"><span data-stu-id="f11c3-121">Int32</span></span>|<span data-ttu-id="f11c3-122">AirPrint のリンク先のリッスン ポート。</span><span class="sxs-lookup"><span data-stu-id="f11c3-122">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="f11c3-123">このキーが既定のポートは AirPrint を使用して、指定されていない場合。</span><span class="sxs-lookup"><span data-stu-id="f11c3-123">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="f11c3-124">IOS 11.0 で利用可能な後で。</span><span class="sxs-lookup"><span data-stu-id="f11c3-124">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="f11c3-125">forceTls</span><span class="sxs-lookup"><span data-stu-id="f11c3-125">forceTls</span></span>|<span data-ttu-id="f11c3-126">ブール型</span><span class="sxs-lookup"><span data-stu-id="f11c3-126">Boolean</span></span>|<span data-ttu-id="f11c3-127">AirPrint 接続の場合は true、トランスポート層セキュリティ (TLS) によって保護されている場合。</span><span class="sxs-lookup"><span data-stu-id="f11c3-127">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="f11c3-128">既定では false を指定します。</span><span class="sxs-lookup"><span data-stu-id="f11c3-128">Default is false.</span></span> <span data-ttu-id="f11c3-129">IOS 11.0 で利用可能な後で。</span><span class="sxs-lookup"><span data-stu-id="f11c3-129">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f11c3-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f11c3-130">Relationships</span></span>
<span data-ttu-id="f11c3-131">なし</span><span class="sxs-lookup"><span data-stu-id="f11c3-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f11c3-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f11c3-132">JSON Representation</span></span>
<span data-ttu-id="f11c3-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f11c3-133">Here is a JSON representation of the resource.</span></span>
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





