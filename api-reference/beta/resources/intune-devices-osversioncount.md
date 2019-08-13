---
title: osVersionCount リソースの種類
description: 各 OS バージョンのマルウェアがあるデバイスの数
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b9302a9604c10db0f462eac1de2caab42a933588
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372532"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="9961f-103">osVersionCount リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9961f-103">osVersionCount resource type</span></span>

> <span data-ttu-id="9961f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9961f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9961f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9961f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9961f-106">各 OS バージョンのマルウェアがあるデバイスの数</span><span class="sxs-lookup"><span data-stu-id="9961f-106">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="9961f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9961f-107">Properties</span></span>
|<span data-ttu-id="9961f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9961f-108">Property</span></span>|<span data-ttu-id="9961f-109">型</span><span class="sxs-lookup"><span data-stu-id="9961f-109">Type</span></span>|<span data-ttu-id="9961f-110">説明</span><span class="sxs-lookup"><span data-stu-id="9961f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9961f-111">osVersion</span><span class="sxs-lookup"><span data-stu-id="9961f-111">osVersion</span></span>|<span data-ttu-id="9961f-112">String</span><span class="sxs-lookup"><span data-stu-id="9961f-112">String</span></span>|<span data-ttu-id="9961f-113">OS のバージョン</span><span class="sxs-lookup"><span data-stu-id="9961f-113">OS version</span></span>|
|<span data-ttu-id="9961f-114">deviceCount</span><span class="sxs-lookup"><span data-stu-id="9961f-114">deviceCount</span></span>|<span data-ttu-id="9961f-115">Int32</span><span class="sxs-lookup"><span data-stu-id="9961f-115">Int32</span></span>|<span data-ttu-id="9961f-116">OS バージョン用のマルウェアがあるデバイスの数</span><span class="sxs-lookup"><span data-stu-id="9961f-116">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="9961f-117">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="9961f-117">lastUpdateDateTime</span></span>|<span data-ttu-id="9961f-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9961f-118">DateTimeOffset</span></span>|<span data-ttu-id="9961f-119">デバイス数の最終更新のタイムスタンプ (UTC)</span><span class="sxs-lookup"><span data-stu-id="9961f-119">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="9961f-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9961f-120">Relationships</span></span>
<span data-ttu-id="9961f-121">なし</span><span class="sxs-lookup"><span data-stu-id="9961f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9961f-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9961f-122">JSON Representation</span></span>
<span data-ttu-id="9961f-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9961f-123">Here is a JSON representation of the resource.</span></span>
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



