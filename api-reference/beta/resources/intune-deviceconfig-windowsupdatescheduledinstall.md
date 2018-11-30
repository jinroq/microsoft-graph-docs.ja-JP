---
title: windowsUpdateScheduledInstall リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: 9f39a9716efed39529c54eaddc62cde075b51954
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068540"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="5f1aa-103">windowsUpdateScheduledInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5f1aa-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="5f1aa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5f1aa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f1aa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f1aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f1aa-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5f1aa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f1aa-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5f1aa-107">Not yet documented</span></span>

<span data-ttu-id="5f1aa-108">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="5f1aa-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5f1aa-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f1aa-109">Properties</span></span>
|<span data-ttu-id="5f1aa-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f1aa-110">Property</span></span>|<span data-ttu-id="5f1aa-111">型</span><span class="sxs-lookup"><span data-stu-id="5f1aa-111">Type</span></span>|<span data-ttu-id="5f1aa-112">説明</span><span class="sxs-lookup"><span data-stu-id="5f1aa-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f1aa-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="5f1aa-113">scheduledInstallDay</span></span>|[<span data-ttu-id="5f1aa-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="5f1aa-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="5f1aa-115">スケジュールされたインストールの週の曜日です。</span><span class="sxs-lookup"><span data-stu-id="5f1aa-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="5f1aa-116">可能な値は、`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="5f1aa-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="5f1aa-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="5f1aa-117">scheduledInstallTime</span></span>|<span data-ttu-id="5f1aa-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="5f1aa-118">TimeOfDay</span></span>|<span data-ttu-id="5f1aa-119">スケジュールされたインストール時刻</span><span class="sxs-lookup"><span data-stu-id="5f1aa-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f1aa-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5f1aa-120">Relationships</span></span>
<span data-ttu-id="5f1aa-121">なし</span><span class="sxs-lookup"><span data-stu-id="5f1aa-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5f1aa-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5f1aa-122">JSON Representation</span></span>
<span data-ttu-id="5f1aa-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5f1aa-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```





