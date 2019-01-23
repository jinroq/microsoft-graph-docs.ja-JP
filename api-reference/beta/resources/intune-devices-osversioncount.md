---
title: osVersionCount リソースの種類
description: 各オペレーティング システムのバージョンのマルウェアとデバイスの数
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cbe0d8ac149ad84ba4cd1286fb0f2303cdfb52a1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410463"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="9653b-103">osVersionCount リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9653b-103">osVersionCount resource type</span></span>

> <span data-ttu-id="9653b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9653b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9653b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9653b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9653b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9653b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9653b-107">各オペレーティング システムのバージョンのマルウェアとデバイスの数</span><span class="sxs-lookup"><span data-stu-id="9653b-107">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="9653b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9653b-108">Properties</span></span>
|<span data-ttu-id="9653b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9653b-109">Property</span></span>|<span data-ttu-id="9653b-110">型</span><span class="sxs-lookup"><span data-stu-id="9653b-110">Type</span></span>|<span data-ttu-id="9653b-111">説明</span><span class="sxs-lookup"><span data-stu-id="9653b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9653b-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="9653b-112">osVersion</span></span>|<span data-ttu-id="9653b-113">String</span><span class="sxs-lookup"><span data-stu-id="9653b-113">String</span></span>|<span data-ttu-id="9653b-114">OS のバージョン</span><span class="sxs-lookup"><span data-stu-id="9653b-114">OS version</span></span>|
|<span data-ttu-id="9653b-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="9653b-115">deviceCount</span></span>|<span data-ttu-id="9653b-116">Int32</span><span class="sxs-lookup"><span data-stu-id="9653b-116">Int32</span></span>|<span data-ttu-id="9653b-117">OS のバージョンのマルウェアとデバイスの数</span><span class="sxs-lookup"><span data-stu-id="9653b-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="9653b-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="9653b-118">lastUpdateDateTime</span></span>|<span data-ttu-id="9653b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9653b-119">DateTimeOffset</span></span>|<span data-ttu-id="9653b-120">デバイスの最後の更新のタイムスタンプは UTC でカウントします。</span><span class="sxs-lookup"><span data-stu-id="9653b-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="9653b-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9653b-121">Relationships</span></span>
<span data-ttu-id="9653b-122">なし</span><span class="sxs-lookup"><span data-stu-id="9653b-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9653b-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9653b-123">JSON Representation</span></span>
<span data-ttu-id="9653b-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9653b-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```




