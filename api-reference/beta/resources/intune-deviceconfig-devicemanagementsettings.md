---
title: deviceManagementSettings リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4e92c8e88ecf620b4731bd3694dfb97e252d042f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973028"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="2cd1a-103">deviceManagementSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2cd1a-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="2cd1a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2cd1a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2cd1a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2cd1a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2cd1a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2cd1a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2cd1a-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2cd1a-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="2cd1a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2cd1a-108">Properties</span></span>
|<span data-ttu-id="2cd1a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2cd1a-109">Property</span></span>|<span data-ttu-id="2cd1a-110">型</span><span class="sxs-lookup"><span data-stu-id="2cd1a-110">Type</span></span>|<span data-ttu-id="2cd1a-111">説明</span><span class="sxs-lookup"><span data-stu-id="2cd1a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cd1a-112">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="2cd1a-112">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="2cd1a-113">Int32</span><span class="sxs-lookup"><span data-stu-id="2cd1a-113">Int32</span></span>|<span data-ttu-id="2cd1a-114">デバイスがチェックインせずに移動し、準拠性を維持できる日数です。</span><span class="sxs-lookup"><span data-stu-id="2cd1a-114">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="2cd1a-115">有効な値は 0 から 120 までです</span><span class="sxs-lookup"><span data-stu-id="2cd1a-115">Valid values 0 to 120</span></span>|
|<span data-ttu-id="2cd1a-116">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="2cd1a-116">isScheduledActionEnabled</span></span>|<span data-ttu-id="2cd1a-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="2cd1a-117">Boolean</span></span>|<span data-ttu-id="2cd1a-118">ルールのスケジュール済みアクションの機能が有効かどうか。</span><span class="sxs-lookup"><span data-stu-id="2cd1a-118">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="2cd1a-119">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="2cd1a-119">secureByDefault</span></span>|<span data-ttu-id="2cd1a-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="2cd1a-120">Boolean</span></span>|<span data-ttu-id="2cd1a-121">これが true の場合に、対象となるコンプライアンス ポリシーがないと、デバイスは非準拠となります</span><span class="sxs-lookup"><span data-stu-id="2cd1a-121">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="2cd1a-122">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="2cd1a-122">enhancedJailBreak</span></span>|<span data-ttu-id="2cd1a-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="2cd1a-123">Boolean</span></span>|<span data-ttu-id="2cd1a-124">機能が有効かではなく、jailbreak の検出を強化します。</span><span class="sxs-lookup"><span data-stu-id="2cd1a-124">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="2cd1a-125">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="2cd1a-125">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="2cd1a-126">Int32</span><span class="sxs-lookup"><span data-stu-id="2cd1a-126">Int32</span></span>|<span data-ttu-id="2cd1a-127">デバイスをチェックしません指定した日数、会社のデータを削除する可能性があり、デバイスを [管理] ではできません。</span><span class="sxs-lookup"><span data-stu-id="2cd1a-127">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="2cd1a-128">有効な値の 30 ~ 270</span><span class="sxs-lookup"><span data-stu-id="2cd1a-128">Valid values 30 to 270</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cd1a-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2cd1a-129">Relationships</span></span>
<span data-ttu-id="2cd1a-130">なし</span><span class="sxs-lookup"><span data-stu-id="2cd1a-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2cd1a-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2cd1a-131">JSON Representation</span></span>
<span data-ttu-id="2cd1a-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2cd1a-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true,
  "enhancedJailBreak": true,
  "deviceInactivityBeforeRetirementInDay": 1024
}
```





