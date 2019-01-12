---
title: hourlySchedule リソースの種類
description: 定期的なデバイスの管理スクリプトのスケジュールを 1 時間ごとに実行します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 004481786fd21ad04e0adbe4e16d3174fc6cc2f4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951888"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="f3901-103">hourlySchedule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f3901-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="f3901-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f3901-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3901-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3901-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3901-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3901-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3901-107">定期的なデバイスの管理スクリプトのスケジュールを 1 時間ごとに実行します。</span><span class="sxs-lookup"><span data-stu-id="f3901-107">Hourly run schedule of a recurring device management script.</span></span>

<span data-ttu-id="f3901-108">[RunSchedule](../resources/intune-devices-runschedule.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f3901-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f3901-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3901-109">Properties</span></span>
|<span data-ttu-id="f3901-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3901-110">Property</span></span>|<span data-ttu-id="f3901-111">種類</span><span class="sxs-lookup"><span data-stu-id="f3901-111">Type</span></span>|<span data-ttu-id="f3901-112">説明</span><span class="sxs-lookup"><span data-stu-id="f3901-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3901-113">interval</span><span class="sxs-lookup"><span data-stu-id="f3901-113">interval</span></span>|<span data-ttu-id="f3901-114">Int32</span><span class="sxs-lookup"><span data-stu-id="f3901-114">Int32</span></span>|<span data-ttu-id="f3901-115">間隔 (時間数単位)</span><span class="sxs-lookup"><span data-stu-id="f3901-115">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3901-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f3901-116">Relationships</span></span>
<span data-ttu-id="f3901-117">なし</span><span class="sxs-lookup"><span data-stu-id="f3901-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f3901-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3901-118">JSON Representation</span></span>
<span data-ttu-id="f3901-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f3901-119">Here is a JSON representation of the resource.</span></span>
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





