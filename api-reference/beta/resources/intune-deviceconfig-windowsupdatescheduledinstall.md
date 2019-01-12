---
title: windowsUpdateScheduledInstall リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8ae4cb747cb4648cd9f4cc9550933688d180dd38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952042"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="fd804-103">windowsUpdateScheduledInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fd804-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="fd804-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fd804-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd804-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd804-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd804-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fd804-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd804-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fd804-107">Not yet documented</span></span>

<span data-ttu-id="fd804-108">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="fd804-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fd804-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd804-109">Properties</span></span>
|<span data-ttu-id="fd804-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd804-110">Property</span></span>|<span data-ttu-id="fd804-111">種類</span><span class="sxs-lookup"><span data-stu-id="fd804-111">Type</span></span>|<span data-ttu-id="fd804-112">説明</span><span class="sxs-lookup"><span data-stu-id="fd804-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd804-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="fd804-113">scheduledInstallDay</span></span>|[<span data-ttu-id="fd804-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="fd804-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="fd804-115">スケジュールされたインストールの週の曜日です。</span><span class="sxs-lookup"><span data-stu-id="fd804-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="fd804-116">可能な値は、`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="fd804-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="fd804-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="fd804-117">scheduledInstallTime</span></span>|<span data-ttu-id="fd804-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fd804-118">TimeOfDay</span></span>|<span data-ttu-id="fd804-119">スケジュールされたインストール時刻</span><span class="sxs-lookup"><span data-stu-id="fd804-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd804-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fd804-120">Relationships</span></span>
<span data-ttu-id="fd804-121">なし</span><span class="sxs-lookup"><span data-stu-id="fd804-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fd804-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fd804-122">JSON Representation</span></span>
<span data-ttu-id="fd804-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fd804-123">Here is a JSON representation of the resource.</span></span>
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





