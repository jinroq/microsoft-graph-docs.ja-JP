---
title: windowsUpdateActiveHoursInstall リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 6d1328723f546f553bc31903d36ada2242d8cda3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307106"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="8839f-103">windowsUpdateActiveHoursInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8839f-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="8839f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8839f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8839f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8839f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8839f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8839f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8839f-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8839f-107">Not yet documented</span></span>

<span data-ttu-id="8839f-108">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="8839f-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8839f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8839f-109">Properties</span></span>
|<span data-ttu-id="8839f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8839f-110">Property</span></span>|<span data-ttu-id="8839f-111">種類</span><span class="sxs-lookup"><span data-stu-id="8839f-111">Type</span></span>|<span data-ttu-id="8839f-112">説明</span><span class="sxs-lookup"><span data-stu-id="8839f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8839f-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="8839f-113">activeHoursStart</span></span>|<span data-ttu-id="8839f-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8839f-114">TimeOfDay</span></span>|<span data-ttu-id="8839f-115">アクティブ時間の開始</span><span class="sxs-lookup"><span data-stu-id="8839f-115">Active Hours Start</span></span>|
|<span data-ttu-id="8839f-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="8839f-116">activeHoursEnd</span></span>|<span data-ttu-id="8839f-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8839f-117">TimeOfDay</span></span>|<span data-ttu-id="8839f-118">アクティブ時間の終了</span><span class="sxs-lookup"><span data-stu-id="8839f-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="8839f-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8839f-119">Relationships</span></span>
<span data-ttu-id="8839f-120">なし</span><span class="sxs-lookup"><span data-stu-id="8839f-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8839f-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8839f-121">JSON Representation</span></span>
<span data-ttu-id="8839f-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8839f-122">Here is a JSON representation of the resource.</span></span>
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





