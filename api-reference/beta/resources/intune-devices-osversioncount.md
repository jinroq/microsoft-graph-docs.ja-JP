---
title: osversioncount リソースの種類
description: 各 OS バージョンのマルウェアがあるデバイスの数
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12ee68855f45ed6827f84a64084118c24081d266
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142750"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="b3e09-103">osversioncount リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b3e09-103">osVersionCount resource type</span></span>

> <span data-ttu-id="b3e09-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3e09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3e09-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b3e09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3e09-106">各 OS バージョンのマルウェアがあるデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b3e09-106">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="b3e09-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3e09-107">Properties</span></span>
|<span data-ttu-id="b3e09-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3e09-108">Property</span></span>|<span data-ttu-id="b3e09-109">型</span><span class="sxs-lookup"><span data-stu-id="b3e09-109">Type</span></span>|<span data-ttu-id="b3e09-110">説明</span><span class="sxs-lookup"><span data-stu-id="b3e09-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3e09-111">osVersion</span><span class="sxs-lookup"><span data-stu-id="b3e09-111">osVersion</span></span>|<span data-ttu-id="b3e09-112">String</span><span class="sxs-lookup"><span data-stu-id="b3e09-112">String</span></span>|<span data-ttu-id="b3e09-113">OS のバージョン</span><span class="sxs-lookup"><span data-stu-id="b3e09-113">OS version</span></span>|
|<span data-ttu-id="b3e09-114">deviceCount</span><span class="sxs-lookup"><span data-stu-id="b3e09-114">deviceCount</span></span>|<span data-ttu-id="b3e09-115">Int32</span><span class="sxs-lookup"><span data-stu-id="b3e09-115">Int32</span></span>|<span data-ttu-id="b3e09-116">OS バージョン用のマルウェアがあるデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b3e09-116">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="b3e09-117">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="b3e09-117">lastUpdateDateTime</span></span>|<span data-ttu-id="b3e09-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3e09-118">DateTimeOffset</span></span>|<span data-ttu-id="b3e09-119">デバイス数の最終更新のタイムスタンプ (UTC)</span><span class="sxs-lookup"><span data-stu-id="b3e09-119">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3e09-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b3e09-120">Relationships</span></span>
<span data-ttu-id="b3e09-121">なし</span><span class="sxs-lookup"><span data-stu-id="b3e09-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3e09-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b3e09-122">JSON Representation</span></span>
<span data-ttu-id="b3e09-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b3e09-123">Here is a JSON representation of the resource.</span></span>
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




