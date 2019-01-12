---
title: deviceConfigurationTargetedUserAndDevice リソースの種類
description: 競合デバイスの構成のポリシーのセットの概要です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 234cc9c909875d835ba54709f30f1ca306eb0954
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947967"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="0c4b1-103">deviceConfigurationTargetedUserAndDevice リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0c4b1-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="0c4b1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0c4b1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c4b1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c4b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c4b1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c4b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c4b1-107">競合デバイスの構成のポリシーのセットの概要です。</span><span class="sxs-lookup"><span data-stu-id="0c4b1-107">Conflict summary for a set of device configuration policies.</span></span>
## <a name="properties"></a><span data-ttu-id="0c4b1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c4b1-108">Properties</span></span>
|<span data-ttu-id="0c4b1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c4b1-109">Property</span></span>|<span data-ttu-id="0c4b1-110">種類</span><span class="sxs-lookup"><span data-stu-id="0c4b1-110">Type</span></span>|<span data-ttu-id="0c4b1-111">説明</span><span class="sxs-lookup"><span data-stu-id="0c4b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c4b1-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="0c4b1-112">deviceId</span></span>|<span data-ttu-id="0c4b1-113">String</span><span class="sxs-lookup"><span data-stu-id="0c4b1-113">String</span></span>|<span data-ttu-id="0c4b1-114">チェックインで、デバイスの id です。</span><span class="sxs-lookup"><span data-stu-id="0c4b1-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="0c4b1-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="0c4b1-115">deviceName</span></span>|<span data-ttu-id="0c4b1-116">String</span><span class="sxs-lookup"><span data-stu-id="0c4b1-116">String</span></span>|<span data-ttu-id="0c4b1-117">チェックインで、デバイスの名前。</span><span class="sxs-lookup"><span data-stu-id="0c4b1-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="0c4b1-118">userId</span><span class="sxs-lookup"><span data-stu-id="0c4b1-118">userId</span></span>|<span data-ttu-id="0c4b1-119">String</span><span class="sxs-lookup"><span data-stu-id="0c4b1-119">String</span></span>|<span data-ttu-id="0c4b1-120">チェックインでユーザーの id です。</span><span class="sxs-lookup"><span data-stu-id="0c4b1-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="0c4b1-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="0c4b1-121">userDisplayName</span></span>|<span data-ttu-id="0c4b1-122">String</span><span class="sxs-lookup"><span data-stu-id="0c4b1-122">String</span></span>|<span data-ttu-id="0c4b1-123">チェックインでユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="0c4b1-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="0c4b1-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0c4b1-124">userPrincipalName</span></span>|<span data-ttu-id="0c4b1-125">String</span><span class="sxs-lookup"><span data-stu-id="0c4b1-125">String</span></span>|<span data-ttu-id="0c4b1-126">チェックインのユーザーの UPN。</span><span class="sxs-lookup"><span data-stu-id="0c4b1-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="0c4b1-127">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="0c4b1-127">lastCheckinDateTime</span></span>|<span data-ttu-id="0c4b1-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c4b1-128">DateTimeOffset</span></span>|<span data-ttu-id="0c4b1-129">このユーザー/デバイス ・ ペアの最後のチェックインの時間です。</span><span class="sxs-lookup"><span data-stu-id="0c4b1-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c4b1-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0c4b1-130">Relationships</span></span>
<span data-ttu-id="0c4b1-131">なし</span><span class="sxs-lookup"><span data-stu-id="0c4b1-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0c4b1-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0c4b1-132">JSON Representation</span></span>
<span data-ttu-id="0c4b1-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0c4b1-133">Here is a JSON representation of the resource.</span></span>
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





