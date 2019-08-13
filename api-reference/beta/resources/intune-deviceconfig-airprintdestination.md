---
title: 放映 Printdestination リソースの種類
description: 放映印刷先を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c8e359e5df1ae55fdc50c42d98c2c5f44f8ea7dc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36334942"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="40fb5-103">放映 Printdestination リソースの種類</span><span class="sxs-lookup"><span data-stu-id="40fb5-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="40fb5-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40fb5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40fb5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="40fb5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40fb5-106">放映印刷先を表します。</span><span class="sxs-lookup"><span data-stu-id="40fb5-106">Represents an AirPrint destination.</span></span>

## <a name="properties"></a><span data-ttu-id="40fb5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40fb5-107">Properties</span></span>
|<span data-ttu-id="40fb5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40fb5-108">Property</span></span>|<span data-ttu-id="40fb5-109">型</span><span class="sxs-lookup"><span data-stu-id="40fb5-109">Type</span></span>|<span data-ttu-id="40fb5-110">説明</span><span class="sxs-lookup"><span data-stu-id="40fb5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40fb5-111">ipAddress</span><span class="sxs-lookup"><span data-stu-id="40fb5-111">ipAddress</span></span>|<span data-ttu-id="40fb5-112">String</span><span class="sxs-lookup"><span data-stu-id="40fb5-112">String</span></span>|<span data-ttu-id="40fb5-113">放映される印刷先の IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="40fb5-113">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="40fb5-114">resourcePath</span><span class="sxs-lookup"><span data-stu-id="40fb5-114">resourcePath</span></span>|<span data-ttu-id="40fb5-115">String</span><span class="sxs-lookup"><span data-stu-id="40fb5-115">String</span></span>|<span data-ttu-id="40fb5-116">プリンターに関連付けられているリソースパス。</span><span class="sxs-lookup"><span data-stu-id="40fb5-116">The Resource Path associated with the printer.</span></span> <span data-ttu-id="40fb5-117">これは、(ipBonjour レコードの rp パラメーターに対応します。</span><span class="sxs-lookup"><span data-stu-id="40fb5-117">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="40fb5-118">例: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer</span><span class="sxs-lookup"><span data-stu-id="40fb5-118">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="40fb5-119">ポート</span><span class="sxs-lookup"><span data-stu-id="40fb5-119">port</span></span>|<span data-ttu-id="40fb5-120">Int32</span><span class="sxs-lookup"><span data-stu-id="40fb5-120">Int32</span></span>|<span data-ttu-id="40fb5-121">放映された印刷先のリスニングポート。</span><span class="sxs-lookup"><span data-stu-id="40fb5-121">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="40fb5-122">このキーが指定されていない場合、印刷時に既定のポートが使用されます。</span><span class="sxs-lookup"><span data-stu-id="40fb5-122">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="40fb5-123">IOS 11.0 以降で利用可能です。</span><span class="sxs-lookup"><span data-stu-id="40fb5-123">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="40fb5-124">forceTls</span><span class="sxs-lookup"><span data-stu-id="40fb5-124">forceTls</span></span>|<span data-ttu-id="40fb5-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="40fb5-125">Boolean</span></span>|<span data-ttu-id="40fb5-126">True の場合、放送印刷接続はトランスポート層セキュリティ (TLS) によって保護されます。</span><span class="sxs-lookup"><span data-stu-id="40fb5-126">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="40fb5-127">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="40fb5-127">Default is false.</span></span> <span data-ttu-id="40fb5-128">IOS 11.0 以降で利用可能です。</span><span class="sxs-lookup"><span data-stu-id="40fb5-128">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40fb5-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="40fb5-129">Relationships</span></span>
<span data-ttu-id="40fb5-130">なし</span><span class="sxs-lookup"><span data-stu-id="40fb5-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40fb5-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="40fb5-131">JSON Representation</span></span>
<span data-ttu-id="40fb5-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="40fb5-132">Here is a JSON representation of the resource.</span></span>
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



