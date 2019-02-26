---
title: 放映 printdestination リソースの種類
description: 放映印刷先を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f09301bd791b5fd8b3fa430b50f7cdf58de43944
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167334"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="659c9-103">放映 printdestination リソースの種類</span><span class="sxs-lookup"><span data-stu-id="659c9-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="659c9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="659c9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="659c9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="659c9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="659c9-106">放映印刷先を表します。</span><span class="sxs-lookup"><span data-stu-id="659c9-106">Represents an AirPrint destination.</span></span>

## <a name="properties"></a><span data-ttu-id="659c9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="659c9-107">Properties</span></span>
|<span data-ttu-id="659c9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="659c9-108">Property</span></span>|<span data-ttu-id="659c9-109">型</span><span class="sxs-lookup"><span data-stu-id="659c9-109">Type</span></span>|<span data-ttu-id="659c9-110">説明</span><span class="sxs-lookup"><span data-stu-id="659c9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="659c9-111">ipAddress</span><span class="sxs-lookup"><span data-stu-id="659c9-111">ipAddress</span></span>|<span data-ttu-id="659c9-112">String</span><span class="sxs-lookup"><span data-stu-id="659c9-112">String</span></span>|<span data-ttu-id="659c9-113">放映される印刷先の IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="659c9-113">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="659c9-114">resourcePath</span><span class="sxs-lookup"><span data-stu-id="659c9-114">resourcePath</span></span>|<span data-ttu-id="659c9-115">String</span><span class="sxs-lookup"><span data-stu-id="659c9-115">String</span></span>|<span data-ttu-id="659c9-116">プリンターに関連付けられているリソースパス。</span><span class="sxs-lookup"><span data-stu-id="659c9-116">The Resource Path associated with the printer.</span></span> <span data-ttu-id="659c9-117">これは、(ipBonjour レコードの rp パラメーターに対応します。</span><span class="sxs-lookup"><span data-stu-id="659c9-117">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="659c9-118">例: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer</span><span class="sxs-lookup"><span data-stu-id="659c9-118">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="659c9-119">port</span><span class="sxs-lookup"><span data-stu-id="659c9-119">port</span></span>|<span data-ttu-id="659c9-120">Int32</span><span class="sxs-lookup"><span data-stu-id="659c9-120">Int32</span></span>|<span data-ttu-id="659c9-121">放映された印刷先のリスニングポート。</span><span class="sxs-lookup"><span data-stu-id="659c9-121">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="659c9-122">このキーが指定されていない場合、印刷時に既定のポートが使用されます。</span><span class="sxs-lookup"><span data-stu-id="659c9-122">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="659c9-123">iOS 11.0 以降で利用可能です。</span><span class="sxs-lookup"><span data-stu-id="659c9-123">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="659c9-124">forcetls</span><span class="sxs-lookup"><span data-stu-id="659c9-124">forceTls</span></span>|<span data-ttu-id="659c9-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="659c9-125">Boolean</span></span>|<span data-ttu-id="659c9-126">true の場合、放送印刷接続はトランスポート層セキュリティ (TLS) によって保護されます。</span><span class="sxs-lookup"><span data-stu-id="659c9-126">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="659c9-127">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="659c9-127">Default is false.</span></span> <span data-ttu-id="659c9-128">iOS 11.0 以降で利用可能です。</span><span class="sxs-lookup"><span data-stu-id="659c9-128">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="659c9-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="659c9-129">Relationships</span></span>
<span data-ttu-id="659c9-130">なし</span><span class="sxs-lookup"><span data-stu-id="659c9-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="659c9-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="659c9-131">JSON Representation</span></span>
<span data-ttu-id="659c9-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="659c9-132">Here is a JSON representation of the resource.</span></span>
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




