---
title: osVersionCount リソースの種類
description: 各オペレーティング システムのバージョンのマルウェアとデバイスの数
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 227e802de7226d653d68997268c9bf4eac4aa259
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864149"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="35426-103">osVersionCount リソースの種類</span><span class="sxs-lookup"><span data-stu-id="35426-103">osVersionCount resource type</span></span>

> <span data-ttu-id="35426-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="35426-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35426-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35426-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35426-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="35426-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35426-107">各オペレーティング システムのバージョンのマルウェアとデバイスの数</span><span class="sxs-lookup"><span data-stu-id="35426-107">Count of devices with malware for each OS version</span></span>
## <a name="properties"></a><span data-ttu-id="35426-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35426-108">Properties</span></span>
|<span data-ttu-id="35426-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35426-109">Property</span></span>|<span data-ttu-id="35426-110">種類</span><span class="sxs-lookup"><span data-stu-id="35426-110">Type</span></span>|<span data-ttu-id="35426-111">説明</span><span class="sxs-lookup"><span data-stu-id="35426-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35426-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="35426-112">osVersion</span></span>|<span data-ttu-id="35426-113">String</span><span class="sxs-lookup"><span data-stu-id="35426-113">String</span></span>|<span data-ttu-id="35426-114">OS のバージョン</span><span class="sxs-lookup"><span data-stu-id="35426-114">OS version</span></span>|
|<span data-ttu-id="35426-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="35426-115">deviceCount</span></span>|<span data-ttu-id="35426-116">Int32</span><span class="sxs-lookup"><span data-stu-id="35426-116">Int32</span></span>|<span data-ttu-id="35426-117">OS のバージョンのマルウェアとデバイスの数</span><span class="sxs-lookup"><span data-stu-id="35426-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="35426-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="35426-118">lastUpdateDateTime</span></span>|<span data-ttu-id="35426-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35426-119">DateTimeOffset</span></span>|<span data-ttu-id="35426-120">デバイスの最後の更新のタイムスタンプは UTC でカウントします。</span><span class="sxs-lookup"><span data-stu-id="35426-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="35426-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="35426-121">Relationships</span></span>
<span data-ttu-id="35426-122">なし</span><span class="sxs-lookup"><span data-stu-id="35426-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="35426-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35426-123">JSON Representation</span></span>
<span data-ttu-id="35426-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="35426-124">Here is a JSON representation of the resource.</span></span>
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





