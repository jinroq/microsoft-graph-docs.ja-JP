---
title: windowsUpdateActiveHoursInstall リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 556e0f22bb249a8606b3bbf9bb3252d3721793b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845739"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="a0d80-103">windowsUpdateActiveHoursInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a0d80-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="a0d80-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a0d80-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0d80-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a0d80-105">Not yet documented</span></span>

<span data-ttu-id="a0d80-106">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a0d80-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a0d80-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0d80-107">Properties</span></span>
|<span data-ttu-id="a0d80-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0d80-108">Property</span></span>|<span data-ttu-id="a0d80-109">種類</span><span class="sxs-lookup"><span data-stu-id="a0d80-109">Type</span></span>|<span data-ttu-id="a0d80-110">説明</span><span class="sxs-lookup"><span data-stu-id="a0d80-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0d80-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="a0d80-111">activeHoursStart</span></span>|<span data-ttu-id="a0d80-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a0d80-112">TimeOfDay</span></span>|<span data-ttu-id="a0d80-113">アクティブ時間の開始</span><span class="sxs-lookup"><span data-stu-id="a0d80-113">Active Hours Start</span></span>|
|<span data-ttu-id="a0d80-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="a0d80-114">activeHoursEnd</span></span>|<span data-ttu-id="a0d80-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a0d80-115">TimeOfDay</span></span>|<span data-ttu-id="a0d80-116">アクティブ時間の終了</span><span class="sxs-lookup"><span data-stu-id="a0d80-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0d80-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a0d80-117">Relationships</span></span>
<span data-ttu-id="a0d80-118">なし</span><span class="sxs-lookup"><span data-stu-id="a0d80-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a0d80-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a0d80-119">JSON Representation</span></span>
<span data-ttu-id="a0d80-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a0d80-120">Here is a JSON representation of the resource.</span></span>
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



