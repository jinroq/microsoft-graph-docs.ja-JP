---
title: osVersionCount リソースの種類
description: 各オペレーティング システムのバージョンのマルウェアとデバイスの数
ms.openlocfilehash: 7892761bd0dc20f09ab2deb47549aeb157e25644
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072566"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="285b4-103">osVersionCount リソースの種類</span><span class="sxs-lookup"><span data-stu-id="285b4-103">osVersionCount resource type</span></span>

> <span data-ttu-id="285b4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="285b4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="285b4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="285b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="285b4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="285b4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="285b4-107">各オペレーティング システムのバージョンのマルウェアとデバイスの数</span><span class="sxs-lookup"><span data-stu-id="285b4-107">Count of devices with malware for each OS version</span></span>
## <a name="properties"></a><span data-ttu-id="285b4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="285b4-108">Properties</span></span>
|<span data-ttu-id="285b4-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="285b4-109">Property</span></span>|<span data-ttu-id="285b4-110">型</span><span class="sxs-lookup"><span data-stu-id="285b4-110">Type</span></span>|<span data-ttu-id="285b4-111">説明</span><span class="sxs-lookup"><span data-stu-id="285b4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="285b4-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="285b4-112">osVersion</span></span>|<span data-ttu-id="285b4-113">String</span><span class="sxs-lookup"><span data-stu-id="285b4-113">String</span></span>|<span data-ttu-id="285b4-114">OS のバージョン</span><span class="sxs-lookup"><span data-stu-id="285b4-114">OS version</span></span>|
|<span data-ttu-id="285b4-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="285b4-115">deviceCount</span></span>|<span data-ttu-id="285b4-116">Int32</span><span class="sxs-lookup"><span data-stu-id="285b4-116">Int32</span></span>|<span data-ttu-id="285b4-117">OS のバージョンのマルウェアとデバイスの数</span><span class="sxs-lookup"><span data-stu-id="285b4-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="285b4-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="285b4-118">lastUpdateDateTime</span></span>|<span data-ttu-id="285b4-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="285b4-119">DateTimeOffset</span></span>|<span data-ttu-id="285b4-120">デバイスの最後の更新のタイムスタンプは UTC でカウントします。</span><span class="sxs-lookup"><span data-stu-id="285b4-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="285b4-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="285b4-121">Relationships</span></span>
<span data-ttu-id="285b4-122">なし</span><span class="sxs-lookup"><span data-stu-id="285b4-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="285b4-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="285b4-123">JSON Representation</span></span>
<span data-ttu-id="285b4-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="285b4-124">Here is a JSON representation of the resource.</span></span>
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





