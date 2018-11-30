---
title: deviceConfigurationUserStateSummary リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: 4ef482b2d2afc3320ec5af0fcdc3a9e57300787b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067929"
---
# <a name="deviceconfigurationuserstatesummary-resource-type"></a><span data-ttu-id="46072-103">deviceConfigurationUserStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="46072-103">deviceConfigurationUserStateSummary resource type</span></span>

> <span data-ttu-id="46072-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="46072-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46072-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46072-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46072-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="46072-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46072-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="46072-107">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="46072-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="46072-108">Methods</span></span>
|<span data-ttu-id="46072-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="46072-109">Method</span></span>|<span data-ttu-id="46072-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="46072-110">Return Type</span></span>|<span data-ttu-id="46072-111">説明</span><span class="sxs-lookup"><span data-stu-id="46072-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="46072-112">DeviceConfigurationUserStateSummary を取得します。</span><span class="sxs-lookup"><span data-stu-id="46072-112">Get deviceConfigurationUserStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationuserstatesummary-get.md)|[<span data-ttu-id="46072-113">deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="46072-113">deviceConfigurationUserStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|<span data-ttu-id="46072-114">[DeviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46072-114">Read properties and relationships of the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>|
|[<span data-ttu-id="46072-115">DeviceConfigurationUserStateSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="46072-115">Update deviceConfigurationUserStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationuserstatesummary-update.md)|[<span data-ttu-id="46072-116">deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="46072-116">deviceConfigurationUserStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|<span data-ttu-id="46072-117">[DeviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="46072-117">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="46072-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46072-118">Properties</span></span>
|<span data-ttu-id="46072-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46072-119">Property</span></span>|<span data-ttu-id="46072-120">型</span><span class="sxs-lookup"><span data-stu-id="46072-120">Type</span></span>|<span data-ttu-id="46072-121">説明</span><span class="sxs-lookup"><span data-stu-id="46072-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46072-122">id</span><span class="sxs-lookup"><span data-stu-id="46072-122">id</span></span>|<span data-ttu-id="46072-123">String</span><span class="sxs-lookup"><span data-stu-id="46072-123">String</span></span>|<span data-ttu-id="46072-124">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="46072-124">Key of the entity.</span></span>|
|<span data-ttu-id="46072-125">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="46072-125">unknownUserCount</span></span>|<span data-ttu-id="46072-126">Int32</span><span class="sxs-lookup"><span data-stu-id="46072-126">Int32</span></span>|<span data-ttu-id="46072-127">不明なユーザーの数</span><span class="sxs-lookup"><span data-stu-id="46072-127">Number of unknown users</span></span>|
|<span data-ttu-id="46072-128">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="46072-128">notApplicableUserCount</span></span>|<span data-ttu-id="46072-129">Int32</span><span class="sxs-lookup"><span data-stu-id="46072-129">Int32</span></span>|<span data-ttu-id="46072-130">適用されないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="46072-130">Number of not applicable users</span></span>|
|<span data-ttu-id="46072-131">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="46072-131">compliantUserCount</span></span>|<span data-ttu-id="46072-132">Int32</span><span class="sxs-lookup"><span data-stu-id="46072-132">Int32</span></span>|<span data-ttu-id="46072-133">準拠のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="46072-133">Number of compliant users</span></span>|
|<span data-ttu-id="46072-134">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="46072-134">remediatedUserCount</span></span>|<span data-ttu-id="46072-135">Int32</span><span class="sxs-lookup"><span data-stu-id="46072-135">Int32</span></span>|<span data-ttu-id="46072-136">修正されたユーザーの数</span><span class="sxs-lookup"><span data-stu-id="46072-136">Number of remediated users</span></span>|
|<span data-ttu-id="46072-137">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="46072-137">nonCompliantUserCount</span></span>|<span data-ttu-id="46072-138">Int32</span><span class="sxs-lookup"><span data-stu-id="46072-138">Int32</span></span>|<span data-ttu-id="46072-139">準拠していないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="46072-139">Number of NonCompliant users</span></span>|
|<span data-ttu-id="46072-140">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="46072-140">errorUserCount</span></span>|<span data-ttu-id="46072-141">Int32</span><span class="sxs-lookup"><span data-stu-id="46072-141">Int32</span></span>|<span data-ttu-id="46072-142">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="46072-142">Number of error users</span></span>|
|<span data-ttu-id="46072-143">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="46072-143">conflictUserCount</span></span>|<span data-ttu-id="46072-144">Int32</span><span class="sxs-lookup"><span data-stu-id="46072-144">Int32</span></span>|<span data-ttu-id="46072-145">競合ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="46072-145">Number of conflict users</span></span>|

## <a name="relationships"></a><span data-ttu-id="46072-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="46072-146">Relationships</span></span>
<span data-ttu-id="46072-147">なし</span><span class="sxs-lookup"><span data-stu-id="46072-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="46072-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="46072-148">JSON Representation</span></span>
<span data-ttu-id="46072-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="46072-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationUserStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "id": "String (identifier)",
  "unknownUserCount": 1024,
  "notApplicableUserCount": 1024,
  "compliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "errorUserCount": 1024,
  "conflictUserCount": 1024
}
```





