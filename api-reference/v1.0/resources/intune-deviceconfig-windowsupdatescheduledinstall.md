---
title: windowsUpdateScheduledInstall リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: 06e26bfb43691c8774e166a65b36d6ab872d44e1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021692"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="748d0-103">windowsUpdateScheduledInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="748d0-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="748d0-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="748d0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="748d0-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="748d0-105">Not yet documented</span></span>

<span data-ttu-id="748d0-106">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="748d0-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="748d0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="748d0-107">Properties</span></span>
|<span data-ttu-id="748d0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="748d0-108">Property</span></span>|<span data-ttu-id="748d0-109">型</span><span class="sxs-lookup"><span data-stu-id="748d0-109">Type</span></span>|<span data-ttu-id="748d0-110">説明</span><span class="sxs-lookup"><span data-stu-id="748d0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="748d0-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="748d0-111">scheduledInstallDay</span></span>|[<span data-ttu-id="748d0-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="748d0-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="748d0-113">スケジュールされたインストールの週の曜日です。</span><span class="sxs-lookup"><span data-stu-id="748d0-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="748d0-114">可能な値は、`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="748d0-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="748d0-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="748d0-115">scheduledInstallTime</span></span>|<span data-ttu-id="748d0-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="748d0-116">TimeOfDay</span></span>|<span data-ttu-id="748d0-117">スケジュールされたインストール時刻</span><span class="sxs-lookup"><span data-stu-id="748d0-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="748d0-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="748d0-118">Relationships</span></span>
<span data-ttu-id="748d0-119">なし</span><span class="sxs-lookup"><span data-stu-id="748d0-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="748d0-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="748d0-120">JSON Representation</span></span>
<span data-ttu-id="748d0-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="748d0-121">Here is a JSON representation of the resource.</span></span>
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



