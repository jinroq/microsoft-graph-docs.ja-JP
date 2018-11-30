---
title: 社員のリソースの種類
description: 定期的なデバイスの管理スクリプトの実行スケジュールを日単位です。
ms.openlocfilehash: 5d517b0bcd15f041b934a0ca936075bc6d3d3741
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072145"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="91e4c-103">社員のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="91e4c-103">dailySchedule resource type</span></span>

> <span data-ttu-id="91e4c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="91e4c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91e4c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91e4c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91e4c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="91e4c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91e4c-107">定期的なデバイスの管理スクリプトの実行スケジュールを日単位です。</span><span class="sxs-lookup"><span data-stu-id="91e4c-107">Daily run schedule of a recurring device management script.</span></span>

<span data-ttu-id="91e4c-108">[RunSchedule](../resources/intune-devices-runschedule.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="91e4c-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="91e4c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91e4c-109">Properties</span></span>
|<span data-ttu-id="91e4c-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91e4c-110">Property</span></span>|<span data-ttu-id="91e4c-111">型</span><span class="sxs-lookup"><span data-stu-id="91e4c-111">Type</span></span>|<span data-ttu-id="91e4c-112">説明</span><span class="sxs-lookup"><span data-stu-id="91e4c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91e4c-113">interval</span><span class="sxs-lookup"><span data-stu-id="91e4c-113">interval</span></span>|<span data-ttu-id="91e4c-114">Int32</span><span class="sxs-lookup"><span data-stu-id="91e4c-114">Int32</span></span>|<span data-ttu-id="91e4c-115">間隔の日数</span><span class="sxs-lookup"><span data-stu-id="91e4c-115">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="91e4c-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="91e4c-116">Relationships</span></span>
<span data-ttu-id="91e4c-117">なし</span><span class="sxs-lookup"><span data-stu-id="91e4c-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="91e4c-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91e4c-118">JSON Representation</span></span>
<span data-ttu-id="91e4c-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="91e4c-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dailySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dailySchedule",
  "interval": 1024
}
```





