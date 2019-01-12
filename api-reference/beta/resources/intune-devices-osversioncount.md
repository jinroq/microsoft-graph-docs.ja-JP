---
title: osVersionCount リソースの種類
description: 各オペレーティング システムのバージョンのマルウェアとデバイスの数
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: de841e679ede22492d26f2a1587e775179c45761
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911841"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="2994b-103">osVersionCount リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2994b-103">osVersionCount resource type</span></span>

> <span data-ttu-id="2994b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2994b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2994b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2994b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2994b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2994b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2994b-107">各オペレーティング システムのバージョンのマルウェアとデバイスの数</span><span class="sxs-lookup"><span data-stu-id="2994b-107">Count of devices with malware for each OS version</span></span>
## <a name="properties"></a><span data-ttu-id="2994b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2994b-108">Properties</span></span>
|<span data-ttu-id="2994b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2994b-109">Property</span></span>|<span data-ttu-id="2994b-110">種類</span><span class="sxs-lookup"><span data-stu-id="2994b-110">Type</span></span>|<span data-ttu-id="2994b-111">説明</span><span class="sxs-lookup"><span data-stu-id="2994b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2994b-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="2994b-112">osVersion</span></span>|<span data-ttu-id="2994b-113">String</span><span class="sxs-lookup"><span data-stu-id="2994b-113">String</span></span>|<span data-ttu-id="2994b-114">OS のバージョン</span><span class="sxs-lookup"><span data-stu-id="2994b-114">OS version</span></span>|
|<span data-ttu-id="2994b-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="2994b-115">deviceCount</span></span>|<span data-ttu-id="2994b-116">Int32</span><span class="sxs-lookup"><span data-stu-id="2994b-116">Int32</span></span>|<span data-ttu-id="2994b-117">OS のバージョンのマルウェアとデバイスの数</span><span class="sxs-lookup"><span data-stu-id="2994b-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="2994b-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="2994b-118">lastUpdateDateTime</span></span>|<span data-ttu-id="2994b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2994b-119">DateTimeOffset</span></span>|<span data-ttu-id="2994b-120">デバイスの最後の更新のタイムスタンプは UTC でカウントします。</span><span class="sxs-lookup"><span data-stu-id="2994b-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="2994b-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2994b-121">Relationships</span></span>
<span data-ttu-id="2994b-122">なし</span><span class="sxs-lookup"><span data-stu-id="2994b-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2994b-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2994b-123">JSON Representation</span></span>
<span data-ttu-id="2994b-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2994b-124">Here is a JSON representation of the resource.</span></span>
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





