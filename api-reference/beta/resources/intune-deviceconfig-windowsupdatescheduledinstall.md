---
title: windowsUpdateScheduledInstall リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 55a53c169f60361af1f695aa07452c4e4a60bedf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301646"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="f3d83-103">windowsUpdateScheduledInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f3d83-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="f3d83-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f3d83-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3d83-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3d83-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3d83-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3d83-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3d83-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f3d83-107">Not yet documented</span></span>

<span data-ttu-id="f3d83-108">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f3d83-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f3d83-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3d83-109">Properties</span></span>
|<span data-ttu-id="f3d83-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3d83-110">Property</span></span>|<span data-ttu-id="f3d83-111">種類</span><span class="sxs-lookup"><span data-stu-id="f3d83-111">Type</span></span>|<span data-ttu-id="f3d83-112">説明</span><span class="sxs-lookup"><span data-stu-id="f3d83-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3d83-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="f3d83-113">scheduledInstallDay</span></span>|[<span data-ttu-id="f3d83-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="f3d83-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="f3d83-115">スケジュールされたインストールの週の曜日です。</span><span class="sxs-lookup"><span data-stu-id="f3d83-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="f3d83-116">可能な値は、`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="f3d83-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="f3d83-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="f3d83-117">scheduledInstallTime</span></span>|<span data-ttu-id="f3d83-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f3d83-118">TimeOfDay</span></span>|<span data-ttu-id="f3d83-119">スケジュールされたインストール時刻</span><span class="sxs-lookup"><span data-stu-id="f3d83-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3d83-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f3d83-120">Relationships</span></span>
<span data-ttu-id="f3d83-121">なし</span><span class="sxs-lookup"><span data-stu-id="f3d83-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f3d83-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3d83-122">JSON Representation</span></span>
<span data-ttu-id="f3d83-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f3d83-123">Here is a JSON representation of the resource.</span></span>
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





