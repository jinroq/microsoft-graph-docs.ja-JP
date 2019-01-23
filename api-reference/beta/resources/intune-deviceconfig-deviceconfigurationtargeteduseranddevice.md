---
title: deviceConfigurationTargetedUserAndDevice リソースの種類
description: 競合デバイスの構成のポリシーのセットの概要です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e246d9731f5ed9d2ea888ba2b53d335fcbca19f1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410743"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="30816-103">deviceConfigurationTargetedUserAndDevice リソースの種類</span><span class="sxs-lookup"><span data-stu-id="30816-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="30816-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="30816-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="30816-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30816-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30816-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="30816-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30816-107">競合デバイスの構成のポリシーのセットの概要です。</span><span class="sxs-lookup"><span data-stu-id="30816-107">Conflict summary for a set of device configuration policies.</span></span>

## <a name="properties"></a><span data-ttu-id="30816-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30816-108">Properties</span></span>
|<span data-ttu-id="30816-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30816-109">Property</span></span>|<span data-ttu-id="30816-110">型</span><span class="sxs-lookup"><span data-stu-id="30816-110">Type</span></span>|<span data-ttu-id="30816-111">説明</span><span class="sxs-lookup"><span data-stu-id="30816-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30816-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="30816-112">deviceId</span></span>|<span data-ttu-id="30816-113">String</span><span class="sxs-lookup"><span data-stu-id="30816-113">String</span></span>|<span data-ttu-id="30816-114">チェックインで、デバイスの id です。</span><span class="sxs-lookup"><span data-stu-id="30816-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="30816-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="30816-115">deviceName</span></span>|<span data-ttu-id="30816-116">String</span><span class="sxs-lookup"><span data-stu-id="30816-116">String</span></span>|<span data-ttu-id="30816-117">チェックインで、デバイスの名前。</span><span class="sxs-lookup"><span data-stu-id="30816-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="30816-118">userId</span><span class="sxs-lookup"><span data-stu-id="30816-118">userId</span></span>|<span data-ttu-id="30816-119">String</span><span class="sxs-lookup"><span data-stu-id="30816-119">String</span></span>|<span data-ttu-id="30816-120">チェックインでユーザーの id です。</span><span class="sxs-lookup"><span data-stu-id="30816-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="30816-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="30816-121">userDisplayName</span></span>|<span data-ttu-id="30816-122">String</span><span class="sxs-lookup"><span data-stu-id="30816-122">String</span></span>|<span data-ttu-id="30816-123">チェックインでユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="30816-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="30816-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="30816-124">userPrincipalName</span></span>|<span data-ttu-id="30816-125">String</span><span class="sxs-lookup"><span data-stu-id="30816-125">String</span></span>|<span data-ttu-id="30816-126">チェックインのユーザーの UPN。</span><span class="sxs-lookup"><span data-stu-id="30816-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="30816-127">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="30816-127">lastCheckinDateTime</span></span>|<span data-ttu-id="30816-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30816-128">DateTimeOffset</span></span>|<span data-ttu-id="30816-129">このユーザー/デバイス ・ ペアの最後のチェックインの時間です。</span><span class="sxs-lookup"><span data-stu-id="30816-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30816-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="30816-130">Relationships</span></span>
<span data-ttu-id="30816-131">なし</span><span class="sxs-lookup"><span data-stu-id="30816-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="30816-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="30816-132">JSON Representation</span></span>
<span data-ttu-id="30816-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="30816-133">Here is a JSON representation of the resource.</span></span>
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




