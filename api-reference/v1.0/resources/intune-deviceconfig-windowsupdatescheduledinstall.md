---
title: windowsUpdateScheduledInstall リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 4a8943fa0275d8b9e5a668be207c90304f22a327
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340916"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="5fd2c-103">windowsUpdateScheduledInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5fd2c-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="5fd2c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5fd2c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5fd2c-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5fd2c-105">Not yet documented</span></span>

<span data-ttu-id="5fd2c-106">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="5fd2c-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5fd2c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5fd2c-107">Properties</span></span>
|<span data-ttu-id="5fd2c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5fd2c-108">Property</span></span>|<span data-ttu-id="5fd2c-109">種類</span><span class="sxs-lookup"><span data-stu-id="5fd2c-109">Type</span></span>|<span data-ttu-id="5fd2c-110">説明</span><span class="sxs-lookup"><span data-stu-id="5fd2c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fd2c-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="5fd2c-111">scheduledInstallDay</span></span>|[<span data-ttu-id="5fd2c-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="5fd2c-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="5fd2c-113">スケジュールされたインストールの週の曜日です。</span><span class="sxs-lookup"><span data-stu-id="5fd2c-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="5fd2c-114">可能な値は、`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="5fd2c-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="5fd2c-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="5fd2c-115">scheduledInstallTime</span></span>|<span data-ttu-id="5fd2c-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="5fd2c-116">TimeOfDay</span></span>|<span data-ttu-id="5fd2c-117">スケジュールされたインストール時刻</span><span class="sxs-lookup"><span data-stu-id="5fd2c-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="5fd2c-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5fd2c-118">Relationships</span></span>
<span data-ttu-id="5fd2c-119">なし</span><span class="sxs-lookup"><span data-stu-id="5fd2c-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5fd2c-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5fd2c-120">JSON Representation</span></span>
<span data-ttu-id="5fd2c-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5fd2c-121">Here is a JSON representation of the resource.</span></span>
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



