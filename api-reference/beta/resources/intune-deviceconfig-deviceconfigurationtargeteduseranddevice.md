---
title: deviceConfigurationTargetedUserAndDevice リソースの種類
description: 一連のデバイス構成ポリシーの競合の概要。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2ddd31671f8cd277dbc7390c8c561189b6c0e3f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567264"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="91929-103">deviceConfigurationTargetedUserAndDevice リソースの種類</span><span class="sxs-lookup"><span data-stu-id="91929-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="91929-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91929-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91929-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="91929-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91929-106">一連のデバイス構成ポリシーの競合の概要。</span><span class="sxs-lookup"><span data-stu-id="91929-106">Conflict summary for a set of device configuration policies.</span></span>

## <a name="properties"></a><span data-ttu-id="91929-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91929-107">Properties</span></span>
|<span data-ttu-id="91929-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91929-108">Property</span></span>|<span data-ttu-id="91929-109">型</span><span class="sxs-lookup"><span data-stu-id="91929-109">Type</span></span>|<span data-ttu-id="91929-110">説明</span><span class="sxs-lookup"><span data-stu-id="91929-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91929-111">deviceId</span><span class="sxs-lookup"><span data-stu-id="91929-111">deviceId</span></span>|<span data-ttu-id="91929-112">String</span><span class="sxs-lookup"><span data-stu-id="91929-112">String</span></span>|<span data-ttu-id="91929-113">チェックイン内のデバイスの id。</span><span class="sxs-lookup"><span data-stu-id="91929-113">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="91929-114">deviceName</span><span class="sxs-lookup"><span data-stu-id="91929-114">deviceName</span></span>|<span data-ttu-id="91929-115">String</span><span class="sxs-lookup"><span data-stu-id="91929-115">String</span></span>|<span data-ttu-id="91929-116">チェックイン内のデバイスの名前。</span><span class="sxs-lookup"><span data-stu-id="91929-116">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="91929-117">userId</span><span class="sxs-lookup"><span data-stu-id="91929-117">userId</span></span>|<span data-ttu-id="91929-118">String</span><span class="sxs-lookup"><span data-stu-id="91929-118">String</span></span>|<span data-ttu-id="91929-119">チェックイン内のユーザーの id。</span><span class="sxs-lookup"><span data-stu-id="91929-119">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="91929-120">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="91929-120">userDisplayName</span></span>|<span data-ttu-id="91929-121">String</span><span class="sxs-lookup"><span data-stu-id="91929-121">String</span></span>|<span data-ttu-id="91929-122">チェックイン内のユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="91929-122">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="91929-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="91929-123">userPrincipalName</span></span>|<span data-ttu-id="91929-124">String</span><span class="sxs-lookup"><span data-stu-id="91929-124">String</span></span>|<span data-ttu-id="91929-125">チェックイン内のユーザーの UPN。</span><span class="sxs-lookup"><span data-stu-id="91929-125">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="91929-126">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="91929-126">lastCheckinDateTime</span></span>|<span data-ttu-id="91929-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91929-127">DateTimeOffset</span></span>|<span data-ttu-id="91929-128">このユーザー/デバイスのペアの最終チェックイン時刻。</span><span class="sxs-lookup"><span data-stu-id="91929-128">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91929-129">関係</span><span class="sxs-lookup"><span data-stu-id="91929-129">Relationships</span></span>
<span data-ttu-id="91929-130">なし</span><span class="sxs-lookup"><span data-stu-id="91929-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91929-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91929-131">JSON Representation</span></span>
<span data-ttu-id="91929-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="91929-132">Here is a JSON representation of the resource.</span></span>
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





