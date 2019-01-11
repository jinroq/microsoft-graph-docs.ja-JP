---
title: windowsUpdateActiveHoursInstall リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 797cfc0f9279f0ab232991a95714d31ce37211a3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818425"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="9b4f7-103">windowsUpdateActiveHoursInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9b4f7-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="9b4f7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9b4f7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b4f7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b4f7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b4f7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9b4f7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b4f7-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9b4f7-107">Not yet documented</span></span>

<span data-ttu-id="9b4f7-108">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="9b4f7-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9b4f7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b4f7-109">Properties</span></span>
|<span data-ttu-id="9b4f7-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b4f7-110">Property</span></span>|<span data-ttu-id="9b4f7-111">種類</span><span class="sxs-lookup"><span data-stu-id="9b4f7-111">Type</span></span>|<span data-ttu-id="9b4f7-112">説明</span><span class="sxs-lookup"><span data-stu-id="9b4f7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b4f7-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="9b4f7-113">activeHoursStart</span></span>|<span data-ttu-id="9b4f7-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9b4f7-114">TimeOfDay</span></span>|<span data-ttu-id="9b4f7-115">アクティブ時間の開始</span><span class="sxs-lookup"><span data-stu-id="9b4f7-115">Active Hours Start</span></span>|
|<span data-ttu-id="9b4f7-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="9b4f7-116">activeHoursEnd</span></span>|<span data-ttu-id="9b4f7-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9b4f7-117">TimeOfDay</span></span>|<span data-ttu-id="9b4f7-118">アクティブ時間の終了</span><span class="sxs-lookup"><span data-stu-id="9b4f7-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b4f7-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9b4f7-119">Relationships</span></span>
<span data-ttu-id="9b4f7-120">なし</span><span class="sxs-lookup"><span data-stu-id="9b4f7-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9b4f7-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9b4f7-121">JSON Representation</span></span>
<span data-ttu-id="9b4f7-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9b4f7-122">Here is a JSON representation of the resource.</span></span>
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





