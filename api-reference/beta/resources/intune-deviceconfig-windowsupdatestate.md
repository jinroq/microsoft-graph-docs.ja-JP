---
title: windowsUpdateState リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 20387d9e1fd9b84853a7bc097dfa08d128809358
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430458"
---
# <a name="windowsupdatestate-resource-type"></a><span data-ttu-id="6929d-103">windowsUpdateState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6929d-103">windowsUpdateState resource type</span></span>

> <span data-ttu-id="6929d-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6929d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6929d-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6929d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6929d-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6929d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6929d-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6929d-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6929d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6929d-108">Properties</span></span>
|<span data-ttu-id="6929d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6929d-109">Property</span></span>|<span data-ttu-id="6929d-110">型</span><span class="sxs-lookup"><span data-stu-id="6929d-110">Type</span></span>|<span data-ttu-id="6929d-111">説明</span><span class="sxs-lookup"><span data-stu-id="6929d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6929d-112">id</span><span class="sxs-lookup"><span data-stu-id="6929d-112">id</span></span>|<span data-ttu-id="6929d-113">String</span><span class="sxs-lookup"><span data-stu-id="6929d-113">String</span></span>|<span data-ttu-id="6929d-114">これは、エンティティの Id です。</span><span class="sxs-lookup"><span data-stu-id="6929d-114">This is Id of the entity.</span></span>|
|<span data-ttu-id="6929d-115">deviceId</span><span class="sxs-lookup"><span data-stu-id="6929d-115">deviceId</span></span>|<span data-ttu-id="6929d-116">String</span><span class="sxs-lookup"><span data-stu-id="6929d-116">String</span></span>|<span data-ttu-id="6929d-117">デバイスの id です。</span><span class="sxs-lookup"><span data-stu-id="6929d-117">The id of the device.</span></span>|
|<span data-ttu-id="6929d-118">userId</span><span class="sxs-lookup"><span data-stu-id="6929d-118">userId</span></span>|<span data-ttu-id="6929d-119">String</span><span class="sxs-lookup"><span data-stu-id="6929d-119">String</span></span>|<span data-ttu-id="6929d-120">ユーザーの id です。</span><span class="sxs-lookup"><span data-stu-id="6929d-120">The id of the user.</span></span>|
|<span data-ttu-id="6929d-121">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6929d-121">deviceDisplayName</span></span>|<span data-ttu-id="6929d-122">String</span><span class="sxs-lookup"><span data-stu-id="6929d-122">String</span></span>|<span data-ttu-id="6929d-123">デバイスの表示名です。</span><span class="sxs-lookup"><span data-stu-id="6929d-123">Device display name.</span></span>|
|<span data-ttu-id="6929d-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6929d-124">userPrincipalName</span></span>|<span data-ttu-id="6929d-125">String</span><span class="sxs-lookup"><span data-stu-id="6929d-125">String</span></span>|<span data-ttu-id="6929d-126">ユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="6929d-126">User principal name.</span></span>|
|<span data-ttu-id="6929d-127">status</span><span class="sxs-lookup"><span data-stu-id="6929d-127">status</span></span>|<span data-ttu-id="6929d-128">[windowsUpdateStatus](../resources/intune-deviceconfig-windowsupdatestatus.md)</span><span class="sxs-lookup"><span data-stu-id="6929d-128">[windowsUpdateStatus] (../resources/intune-deviceconfig-windowsupdatestatus.md)</span></span>|<span data-ttu-id="6929d-129">Windows udpate の状態です。</span><span class="sxs-lookup"><span data-stu-id="6929d-129">Windows udpate status.</span></span>|
|<span data-ttu-id="6929d-130">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="6929d-130">qualityUpdateVersion</span></span>|<span data-ttu-id="6929d-131">String</span><span class="sxs-lookup"><span data-stu-id="6929d-131">String</span></span>|<span data-ttu-id="6929d-132">デバイスの品質の更新プログラムのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="6929d-132">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="6929d-133">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="6929d-133">featureUpdateVersion</span></span>|<span data-ttu-id="6929d-134">String</span><span class="sxs-lookup"><span data-stu-id="6929d-134">String</span></span>|<span data-ttu-id="6929d-135">デバイスの現在の機能の更新バージョンです。</span><span class="sxs-lookup"><span data-stu-id="6929d-135">The current feature update version of the device.</span></span>|
|<span data-ttu-id="6929d-136">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="6929d-136">lastScanDateTime</span></span>|<span data-ttu-id="6929d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6929d-137">DateTimeOffset</span></span>|<span data-ttu-id="6929d-138">日付時刻を Windows Update エージェントは、スキャンが成功をしました。</span><span class="sxs-lookup"><span data-stu-id="6929d-138">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="6929d-139">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6929d-139">lastSyncDateTime</span></span>|<span data-ttu-id="6929d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6929d-140">DateTimeOffset</span></span>|<span data-ttu-id="6929d-141">Microsoft Intune でデバイスが同期で最後の日に。</span><span class="sxs-lookup"><span data-stu-id="6929d-141">Last date time that the device sync with with Microsoft Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6929d-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6929d-142">Relationships</span></span>
<span data-ttu-id="6929d-143">なし</span><span class="sxs-lookup"><span data-stu-id="6929d-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6929d-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6929d-144">JSON Representation</span></span>
<span data-ttu-id="6929d-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6929d-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.WindowsUpdateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.WindowsUpdateState",
  "id": "String (identifier)",
  "deviceId": "String (identifier)",
  "userId": "String (identifier)",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "status": "String",
  "qualityUpdateVersion": "String",
  "featureUpdateVersion": "String",
  "lastScanDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)"
}
```


