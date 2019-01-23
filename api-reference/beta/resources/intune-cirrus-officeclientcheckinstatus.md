---
title: officeClientCheckinStatus リソースの種類
description: チェックインのテナント統計 (stats) を記述するエンティティです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aebc534a6c424a9dac4316d0029e2fd35839f0a7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403260"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="0818b-103">officeClientCheckinStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0818b-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="0818b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0818b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0818b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0818b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0818b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0818b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0818b-107">チェックインのテナント統計 (stats) を記述するエンティティです。</span><span class="sxs-lookup"><span data-stu-id="0818b-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="0818b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0818b-108">Properties</span></span>
|<span data-ttu-id="0818b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0818b-109">Property</span></span>|<span data-ttu-id="0818b-110">型</span><span class="sxs-lookup"><span data-stu-id="0818b-110">Type</span></span>|<span data-ttu-id="0818b-111">説明</span><span class="sxs-lookup"><span data-stu-id="0818b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0818b-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0818b-112">userPrincipalName</span></span>|<span data-ttu-id="0818b-113">String</span><span class="sxs-lookup"><span data-stu-id="0818b-113">String</span></span>|<span data-ttu-id="0818b-114">ユーザー プリンシパル名は、デバイスを使用します。</span><span class="sxs-lookup"><span data-stu-id="0818b-114">User principal name using the device.</span></span>|
|<span data-ttu-id="0818b-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="0818b-115">deviceName</span></span>|<span data-ttu-id="0818b-116">String</span><span class="sxs-lookup"><span data-stu-id="0818b-116">String</span></span>|<span data-ttu-id="0818b-117">チェックインしようとするデバイスの名前。</span><span class="sxs-lookup"><span data-stu-id="0818b-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="0818b-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="0818b-118">devicePlatform</span></span>|<span data-ttu-id="0818b-119">String</span><span class="sxs-lookup"><span data-stu-id="0818b-119">String</span></span>|<span data-ttu-id="0818b-120">デバイスのプラットフォームにチェックインしようとします。</span><span class="sxs-lookup"><span data-stu-id="0818b-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="0818b-121">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="0818b-121">devicePlatformVersion</span></span>|<span data-ttu-id="0818b-122">String</span><span class="sxs-lookup"><span data-stu-id="0818b-122">String</span></span>|<span data-ttu-id="0818b-123">デバイス プラットフォームのバージョンがチェックインをしようとします。</span><span class="sxs-lookup"><span data-stu-id="0818b-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="0818b-124">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="0818b-124">wasSuccessful</span></span>|<span data-ttu-id="0818b-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="0818b-125">Boolean</span></span>|<span data-ttu-id="0818b-126">最後のチェックインが正常に完了しました。 場合、</span><span class="sxs-lookup"><span data-stu-id="0818b-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="0818b-127">userId</span><span class="sxs-lookup"><span data-stu-id="0818b-127">userId</span></span>|<span data-ttu-id="0818b-128">String</span><span class="sxs-lookup"><span data-stu-id="0818b-128">String</span></span>|<span data-ttu-id="0818b-129">デバイスを使用してユーザーの識別子です。</span><span class="sxs-lookup"><span data-stu-id="0818b-129">User identifier using the device.</span></span>|
|<span data-ttu-id="0818b-130">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="0818b-130">checkinDateTime</span></span>|<span data-ttu-id="0818b-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0818b-131">DateTimeOffset</span></span>|<span data-ttu-id="0818b-132">最後デバイス チェックの時間 (utc) です。</span><span class="sxs-lookup"><span data-stu-id="0818b-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="0818b-133">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="0818b-133">errorMessage</span></span>|<span data-ttu-id="0818b-134">String</span><span class="sxs-lookup"><span data-stu-id="0818b-134">String</span></span>|<span data-ttu-id="0818b-135">最後のチェックインに関連付けられている場合のエラー メッセージです。</span><span class="sxs-lookup"><span data-stu-id="0818b-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="0818b-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="0818b-136">appliedPolicies</span></span>|<span data-ttu-id="0818b-137">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0818b-137">String collection</span></span>|<span data-ttu-id="0818b-138">ポリシーの一覧では、最後のチェックインと、デバイスに配信されます。</span><span class="sxs-lookup"><span data-stu-id="0818b-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0818b-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0818b-139">Relationships</span></span>
<span data-ttu-id="0818b-140">なし</span><span class="sxs-lookup"><span data-stu-id="0818b-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0818b-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0818b-141">JSON Representation</span></span>
<span data-ttu-id="0818b-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0818b-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientCheckinStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientCheckinStatus",
  "userPrincipalName": "String",
  "deviceName": "String",
  "devicePlatform": "String",
  "devicePlatformVersion": "String",
  "wasSuccessful": true,
  "userId": "String",
  "checkinDateTime": "String (timestamp)",
  "errorMessage": "String",
  "appliedPolicies": [
    "String"
  ]
}
```



