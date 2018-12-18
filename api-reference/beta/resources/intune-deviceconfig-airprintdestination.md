---
title: airPrintDestination リソースの種類
description: AirPrint のリンク先を表します。
author: tfitzmac
ms.openlocfilehash: 046f85c65d382b34e6920f30f6b2718f817371a9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361055"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="0900d-103">airPrintDestination リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0900d-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="0900d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0900d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0900d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0900d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0900d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0900d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0900d-107">AirPrint のリンク先を表します。</span><span class="sxs-lookup"><span data-stu-id="0900d-107">Represents an AirPrint destination.</span></span>
## <a name="properties"></a><span data-ttu-id="0900d-108">Properties</span><span class="sxs-lookup"><span data-stu-id="0900d-108">Properties</span></span>
|<span data-ttu-id="0900d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0900d-109">Property</span></span>|<span data-ttu-id="0900d-110">種類</span><span class="sxs-lookup"><span data-stu-id="0900d-110">Type</span></span>|<span data-ttu-id="0900d-111">説明</span><span class="sxs-lookup"><span data-stu-id="0900d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0900d-112">ipAddress</span><span class="sxs-lookup"><span data-stu-id="0900d-112">ipAddress</span></span>|<span data-ttu-id="0900d-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0900d-113">String</span></span>|<span data-ttu-id="0900d-114">AirPrint の宛先の IP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="0900d-114">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="0900d-115">resourcePath</span><span class="sxs-lookup"><span data-stu-id="0900d-115">resourcePath</span></span>|<span data-ttu-id="0900d-116">String</span><span class="sxs-lookup"><span data-stu-id="0900d-116">String</span></span>|<span data-ttu-id="0900d-117">プリンターに関連付けられているリソースのパスです。</span><span class="sxs-lookup"><span data-stu-id="0900d-117">The Resource Path associated with the printer.</span></span> <span data-ttu-id="0900d-118">これは、Bonjour のレコードの _ipps.tcp の rp のパラメーターに対応しています。</span><span class="sxs-lookup"><span data-stu-id="0900d-118">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="0900d-119">例: プリンター/Canon_MG5300_series、プリンター/Xerox_Phaser_7600、ipp 印刷/Epson_IPP_Printer です。</span><span class="sxs-lookup"><span data-stu-id="0900d-119">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="0900d-120">port</span><span class="sxs-lookup"><span data-stu-id="0900d-120">port</span></span>|<span data-ttu-id="0900d-121">Int32</span><span class="sxs-lookup"><span data-stu-id="0900d-121">Int32</span></span>|<span data-ttu-id="0900d-122">AirPrint のリンク先のリッスン ポート。</span><span class="sxs-lookup"><span data-stu-id="0900d-122">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="0900d-123">このキーが既定のポートは AirPrint を使用して、指定されていない場合。</span><span class="sxs-lookup"><span data-stu-id="0900d-123">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="0900d-124">IOS 11.0 で利用可能な後で。</span><span class="sxs-lookup"><span data-stu-id="0900d-124">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="0900d-125">forceTls</span><span class="sxs-lookup"><span data-stu-id="0900d-125">forceTls</span></span>|<span data-ttu-id="0900d-126">ブール型</span><span class="sxs-lookup"><span data-stu-id="0900d-126">Boolean</span></span>|<span data-ttu-id="0900d-127">AirPrint 接続の場合は true、トランスポート層セキュリティ (TLS) によって保護されている場合。</span><span class="sxs-lookup"><span data-stu-id="0900d-127">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="0900d-128">既定では false を指定します。</span><span class="sxs-lookup"><span data-stu-id="0900d-128">Default is false.</span></span> <span data-ttu-id="0900d-129">IOS 11.0 で利用可能な後で。</span><span class="sxs-lookup"><span data-stu-id="0900d-129">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0900d-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0900d-130">Relationships</span></span>
<span data-ttu-id="0900d-131">なし</span><span class="sxs-lookup"><span data-stu-id="0900d-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0900d-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0900d-132">JSON Representation</span></span>
<span data-ttu-id="0900d-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0900d-133">Here is a JSON representation of the resource.</span></span>
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





