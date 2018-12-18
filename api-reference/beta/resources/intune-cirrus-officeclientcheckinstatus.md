---
title: officeClientCheckinStatus リソースの種類
description: チェックインのテナント統計 (stats) を記述するエンティティです。
author: tfitzmac
ms.openlocfilehash: 0c6359d3cb6c776d0f26fdaf88ce7f2f03e5f8c7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331718"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="b1137-103">officeClientCheckinStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b1137-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="b1137-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b1137-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1137-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1137-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1137-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b1137-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1137-107">チェックインのテナント統計 (stats) を記述するエンティティです。</span><span class="sxs-lookup"><span data-stu-id="b1137-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="b1137-108">Properties</span><span class="sxs-lookup"><span data-stu-id="b1137-108">Properties</span></span>
|<span data-ttu-id="b1137-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1137-109">Property</span></span>|<span data-ttu-id="b1137-110">種類</span><span class="sxs-lookup"><span data-stu-id="b1137-110">Type</span></span>|<span data-ttu-id="b1137-111">説明</span><span class="sxs-lookup"><span data-stu-id="b1137-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1137-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1137-112">userPrincipalName</span></span>|<span data-ttu-id="b1137-113">String</span><span class="sxs-lookup"><span data-stu-id="b1137-113">String</span></span>|<span data-ttu-id="b1137-114">ユーザー プリンシパル名は、デバイスを使用します。</span><span class="sxs-lookup"><span data-stu-id="b1137-114">User principal name using the device.</span></span>|
|<span data-ttu-id="b1137-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="b1137-115">deviceName</span></span>|<span data-ttu-id="b1137-116">String</span><span class="sxs-lookup"><span data-stu-id="b1137-116">String</span></span>|<span data-ttu-id="b1137-117">チェックインしようとするデバイスの名前。</span><span class="sxs-lookup"><span data-stu-id="b1137-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="b1137-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="b1137-118">devicePlatform</span></span>|<span data-ttu-id="b1137-119">String</span><span class="sxs-lookup"><span data-stu-id="b1137-119">String</span></span>|<span data-ttu-id="b1137-120">デバイスのプラットフォームにチェックインしようとします。</span><span class="sxs-lookup"><span data-stu-id="b1137-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="b1137-121">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="b1137-121">devicePlatformVersion</span></span>|<span data-ttu-id="b1137-122">String</span><span class="sxs-lookup"><span data-stu-id="b1137-122">String</span></span>|<span data-ttu-id="b1137-123">デバイス プラットフォームのバージョンがチェックインをしようとします。</span><span class="sxs-lookup"><span data-stu-id="b1137-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="b1137-124">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="b1137-124">wasSuccessful</span></span>|<span data-ttu-id="b1137-125">ブール型</span><span class="sxs-lookup"><span data-stu-id="b1137-125">Boolean</span></span>|<span data-ttu-id="b1137-126">最後のチェックインが正常に完了しました。 場合、</span><span class="sxs-lookup"><span data-stu-id="b1137-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="b1137-127">userId</span><span class="sxs-lookup"><span data-stu-id="b1137-127">userId</span></span>|<span data-ttu-id="b1137-128">String</span><span class="sxs-lookup"><span data-stu-id="b1137-128">String</span></span>|<span data-ttu-id="b1137-129">デバイスを使用してユーザーの識別子です。</span><span class="sxs-lookup"><span data-stu-id="b1137-129">User identifier using the device.</span></span>|
|<span data-ttu-id="b1137-130">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="b1137-130">checkinDateTime</span></span>|<span data-ttu-id="b1137-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1137-131">DateTimeOffset</span></span>|<span data-ttu-id="b1137-132">最後デバイス チェックの時間 (utc) です。</span><span class="sxs-lookup"><span data-stu-id="b1137-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="b1137-133">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="b1137-133">errorMessage</span></span>|<span data-ttu-id="b1137-134">String</span><span class="sxs-lookup"><span data-stu-id="b1137-134">String</span></span>|<span data-ttu-id="b1137-135">最後のチェックインに関連付けられている場合のエラー メッセージです。</span><span class="sxs-lookup"><span data-stu-id="b1137-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="b1137-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="b1137-136">appliedPolicies</span></span>|<span data-ttu-id="b1137-137">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b1137-137">String collection</span></span>|<span data-ttu-id="b1137-138">ポリシーの一覧では、最後のチェックインと、デバイスに配信されます。</span><span class="sxs-lookup"><span data-stu-id="b1137-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1137-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b1137-139">Relationships</span></span>
<span data-ttu-id="b1137-140">なし</span><span class="sxs-lookup"><span data-stu-id="b1137-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b1137-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b1137-141">JSON Representation</span></span>
<span data-ttu-id="b1137-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b1137-142">Here is a JSON representation of the resource.</span></span>
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



