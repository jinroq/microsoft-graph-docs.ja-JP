---
title: windowsUpdateActiveHoursInstall リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ed4f909db5dd31195ace7d98151b226b03849c81
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967183"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="a567d-103">windowsUpdateActiveHoursInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a567d-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="a567d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a567d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a567d-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a567d-105">Not yet documented</span></span>

<span data-ttu-id="a567d-106">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a567d-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a567d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a567d-107">Properties</span></span>
|<span data-ttu-id="a567d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a567d-108">Property</span></span>|<span data-ttu-id="a567d-109">種類</span><span class="sxs-lookup"><span data-stu-id="a567d-109">Type</span></span>|<span data-ttu-id="a567d-110">説明</span><span class="sxs-lookup"><span data-stu-id="a567d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a567d-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="a567d-111">activeHoursStart</span></span>|<span data-ttu-id="a567d-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a567d-112">TimeOfDay</span></span>|<span data-ttu-id="a567d-113">アクティブ時間の開始</span><span class="sxs-lookup"><span data-stu-id="a567d-113">Active Hours Start</span></span>|
|<span data-ttu-id="a567d-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="a567d-114">activeHoursEnd</span></span>|<span data-ttu-id="a567d-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a567d-115">TimeOfDay</span></span>|<span data-ttu-id="a567d-116">アクティブ時間の終了</span><span class="sxs-lookup"><span data-stu-id="a567d-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="a567d-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a567d-117">Relationships</span></span>
<span data-ttu-id="a567d-118">なし</span><span class="sxs-lookup"><span data-stu-id="a567d-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a567d-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a567d-119">JSON Representation</span></span>
<span data-ttu-id="a567d-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a567d-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateActiveHoursInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateActiveHoursInstall",
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)"
}
```



