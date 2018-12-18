---
title: osVersionCount リソースの種類
description: 各オペレーティング システムのバージョンのマルウェアとデバイスの数
author: tfitzmac
ms.openlocfilehash: ccc031c6060604b36166b4869d02f08854dfdd2c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331998"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="dff6c-103">osVersionCount リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dff6c-103">osVersionCount resource type</span></span>

> <span data-ttu-id="dff6c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dff6c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dff6c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dff6c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dff6c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dff6c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dff6c-107">各オペレーティング システムのバージョンのマルウェアとデバイスの数</span><span class="sxs-lookup"><span data-stu-id="dff6c-107">Count of devices with malware for each OS version</span></span>
## <a name="properties"></a><span data-ttu-id="dff6c-108">Properties</span><span class="sxs-lookup"><span data-stu-id="dff6c-108">Properties</span></span>
|<span data-ttu-id="dff6c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dff6c-109">Property</span></span>|<span data-ttu-id="dff6c-110">種類</span><span class="sxs-lookup"><span data-stu-id="dff6c-110">Type</span></span>|<span data-ttu-id="dff6c-111">説明</span><span class="sxs-lookup"><span data-stu-id="dff6c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dff6c-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="dff6c-112">osVersion</span></span>|<span data-ttu-id="dff6c-113">String</span><span class="sxs-lookup"><span data-stu-id="dff6c-113">String</span></span>|<span data-ttu-id="dff6c-114">OS のバージョン</span><span class="sxs-lookup"><span data-stu-id="dff6c-114">OS version</span></span>|
|<span data-ttu-id="dff6c-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="dff6c-115">deviceCount</span></span>|<span data-ttu-id="dff6c-116">Int32</span><span class="sxs-lookup"><span data-stu-id="dff6c-116">Int32</span></span>|<span data-ttu-id="dff6c-117">OS のバージョンのマルウェアとデバイスの数</span><span class="sxs-lookup"><span data-stu-id="dff6c-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="dff6c-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="dff6c-118">lastUpdateDateTime</span></span>|<span data-ttu-id="dff6c-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dff6c-119">DateTimeOffset</span></span>|<span data-ttu-id="dff6c-120">デバイスの最後の更新のタイムスタンプは UTC でカウントします。</span><span class="sxs-lookup"><span data-stu-id="dff6c-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="dff6c-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dff6c-121">Relationships</span></span>
<span data-ttu-id="dff6c-122">なし</span><span class="sxs-lookup"><span data-stu-id="dff6c-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dff6c-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dff6c-123">JSON Representation</span></span>
<span data-ttu-id="dff6c-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dff6c-124">Here is a JSON representation of the resource.</span></span>
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





