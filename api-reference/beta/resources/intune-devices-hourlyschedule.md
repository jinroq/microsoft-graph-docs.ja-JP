---
title: hourlySchedule リソースの種類
description: 定期的なデバイスの管理スクリプトのスケジュールを 1 時間ごとに実行します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2f22cc44fdd9017ef6db6f014e4a9b756d46d034
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811292"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="c9f30-103">hourlySchedule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c9f30-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="c9f30-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c9f30-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9f30-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9f30-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9f30-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c9f30-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9f30-107">定期的なデバイスの管理スクリプトのスケジュールを 1 時間ごとに実行します。</span><span class="sxs-lookup"><span data-stu-id="c9f30-107">Hourly run schedule of a recurring device management script.</span></span>

<span data-ttu-id="c9f30-108">[RunSchedule](../resources/intune-devices-runschedule.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c9f30-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c9f30-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9f30-109">Properties</span></span>
|<span data-ttu-id="c9f30-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9f30-110">Property</span></span>|<span data-ttu-id="c9f30-111">種類</span><span class="sxs-lookup"><span data-stu-id="c9f30-111">Type</span></span>|<span data-ttu-id="c9f30-112">説明</span><span class="sxs-lookup"><span data-stu-id="c9f30-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9f30-113">interval</span><span class="sxs-lookup"><span data-stu-id="c9f30-113">interval</span></span>|<span data-ttu-id="c9f30-114">Int32</span><span class="sxs-lookup"><span data-stu-id="c9f30-114">Int32</span></span>|<span data-ttu-id="c9f30-115">間隔 (時間数単位)</span><span class="sxs-lookup"><span data-stu-id="c9f30-115">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9f30-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c9f30-116">Relationships</span></span>
<span data-ttu-id="c9f30-117">なし</span><span class="sxs-lookup"><span data-stu-id="c9f30-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c9f30-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c9f30-118">JSON Representation</span></span>
<span data-ttu-id="c9f30-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c9f30-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hourlySchedule",
  "interval": 1024
}
```





