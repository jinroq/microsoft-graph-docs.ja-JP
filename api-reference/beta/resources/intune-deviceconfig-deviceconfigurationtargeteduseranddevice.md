---
title: deviceConfigurationTargetedUserAndDevice リソースの種類
description: 競合デバイスの構成のポリシーのセットの概要です。
ms.openlocfilehash: 6f79a8fe24e06d2bdafa81c30cabf8158b4e5773
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067314"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="de81f-103">deviceConfigurationTargetedUserAndDevice リソースの種類</span><span class="sxs-lookup"><span data-stu-id="de81f-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="de81f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="de81f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de81f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de81f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de81f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="de81f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de81f-107">競合デバイスの構成のポリシーのセットの概要です。</span><span class="sxs-lookup"><span data-stu-id="de81f-107">Conflict summary for a set of device configuration policies.</span></span>
## <a name="properties"></a><span data-ttu-id="de81f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de81f-108">Properties</span></span>
|<span data-ttu-id="de81f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de81f-109">Property</span></span>|<span data-ttu-id="de81f-110">型</span><span class="sxs-lookup"><span data-stu-id="de81f-110">Type</span></span>|<span data-ttu-id="de81f-111">説明</span><span class="sxs-lookup"><span data-stu-id="de81f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de81f-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="de81f-112">deviceId</span></span>|<span data-ttu-id="de81f-113">String</span><span class="sxs-lookup"><span data-stu-id="de81f-113">String</span></span>|<span data-ttu-id="de81f-114">チェックインで、デバイスの id です。</span><span class="sxs-lookup"><span data-stu-id="de81f-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="de81f-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="de81f-115">deviceName</span></span>|<span data-ttu-id="de81f-116">String</span><span class="sxs-lookup"><span data-stu-id="de81f-116">String</span></span>|<span data-ttu-id="de81f-117">チェックインで、デバイスの名前。</span><span class="sxs-lookup"><span data-stu-id="de81f-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="de81f-118">userId</span><span class="sxs-lookup"><span data-stu-id="de81f-118">userId</span></span>|<span data-ttu-id="de81f-119">String</span><span class="sxs-lookup"><span data-stu-id="de81f-119">String</span></span>|<span data-ttu-id="de81f-120">チェックインでユーザーの id です。</span><span class="sxs-lookup"><span data-stu-id="de81f-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="de81f-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="de81f-121">userDisplayName</span></span>|<span data-ttu-id="de81f-122">String</span><span class="sxs-lookup"><span data-stu-id="de81f-122">String</span></span>|<span data-ttu-id="de81f-123">チェックインでユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="de81f-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="de81f-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="de81f-124">userPrincipalName</span></span>|<span data-ttu-id="de81f-125">String</span><span class="sxs-lookup"><span data-stu-id="de81f-125">String</span></span>|<span data-ttu-id="de81f-126">チェックインのユーザーの UPN。</span><span class="sxs-lookup"><span data-stu-id="de81f-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="de81f-127">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="de81f-127">lastCheckinDateTime</span></span>|<span data-ttu-id="de81f-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de81f-128">DateTimeOffset</span></span>|<span data-ttu-id="de81f-129">このユーザー/デバイス ・ ペアの最後のチェックインの時間です。</span><span class="sxs-lookup"><span data-stu-id="de81f-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de81f-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="de81f-130">Relationships</span></span>
<span data-ttu-id="de81f-131">なし</span><span class="sxs-lookup"><span data-stu-id="de81f-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="de81f-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="de81f-132">JSON Representation</span></span>
<span data-ttu-id="de81f-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="de81f-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationTargetedUserAndDevice",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "lastCheckinDateTime": "String (timestamp)"
}
```





