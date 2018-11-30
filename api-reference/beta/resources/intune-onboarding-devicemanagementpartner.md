---
title: deviceManagementPartner リソースの種類
description: デバイス管理パートナーとの接続を表すエンティティです。
ms.openlocfilehash: c682b700636ad80f20719e40f35a929cf740c7a0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073262"
---
# <a name="devicemanagementpartner-resource-type"></a><span data-ttu-id="85c93-103">deviceManagementPartner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="85c93-103">deviceManagementPartner resource type</span></span>

> <span data-ttu-id="85c93-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="85c93-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85c93-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85c93-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85c93-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="85c93-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85c93-107">デバイス管理パートナーとの接続を表すエンティティです。</span><span class="sxs-lookup"><span data-stu-id="85c93-107">Entity which represents a connection to device management partner.</span></span>
## <a name="methods"></a><span data-ttu-id="85c93-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="85c93-108">Methods</span></span>
|<span data-ttu-id="85c93-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="85c93-109">Method</span></span>|<span data-ttu-id="85c93-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="85c93-110">Return Type</span></span>|<span data-ttu-id="85c93-111">説明</span><span class="sxs-lookup"><span data-stu-id="85c93-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="85c93-112">List deviceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="85c93-112">List deviceManagementPartners</span></span>](../api/intune-onboarding-devicemanagementpartner-list.md)|<span data-ttu-id="85c93-113">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="85c93-113">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) collection</span></span>|<span data-ttu-id="85c93-114">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="85c93-114">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>|
|[<span data-ttu-id="85c93-115">Get deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="85c93-115">Get deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-get.md)|[<span data-ttu-id="85c93-116">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="85c93-116">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="85c93-117">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="85c93-117">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="85c93-118">Create deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="85c93-118">Create deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-create.md)|[<span data-ttu-id="85c93-119">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="85c93-119">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="85c93-120">新しい [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="85c93-120">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="85c93-121">Delete deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="85c93-121">Delete deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-delete.md)|<span data-ttu-id="85c93-122">なし</span><span class="sxs-lookup"><span data-stu-id="85c93-122">None</span></span>|<span data-ttu-id="85c93-123">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="85c93-123">Deletes a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>|
|[<span data-ttu-id="85c93-124">Update deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="85c93-124">Update deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-update.md)|[<span data-ttu-id="85c93-125">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="85c93-125">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="85c93-126">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="85c93-126">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="85c93-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85c93-127">Properties</span></span>
|<span data-ttu-id="85c93-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85c93-128">Property</span></span>|<span data-ttu-id="85c93-129">型</span><span class="sxs-lookup"><span data-stu-id="85c93-129">Type</span></span>|<span data-ttu-id="85c93-130">説明</span><span class="sxs-lookup"><span data-stu-id="85c93-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85c93-131">id</span><span class="sxs-lookup"><span data-stu-id="85c93-131">id</span></span>|<span data-ttu-id="85c93-132">String</span><span class="sxs-lookup"><span data-stu-id="85c93-132">String</span></span>|<span data-ttu-id="85c93-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="85c93-133">Not yet documented</span></span>|
|<span data-ttu-id="85c93-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="85c93-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="85c93-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85c93-135">DateTimeOffset</span></span>|<span data-ttu-id="85c93-136">管理者が [デバイス管理パートナーに接続] オプションを有効にした後の最終ハートビートのタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="85c93-136">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="85c93-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="85c93-137">partnerState</span></span>|[<span data-ttu-id="85c93-138">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="85c93-138">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="85c93-139">このテナントのパートナーの状態です。</span><span class="sxs-lookup"><span data-stu-id="85c93-139">Partner state of this tenant.</span></span> <span data-ttu-id="85c93-140">使用可能な値: `unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="85c93-140">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="85c93-141">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="85c93-141">partnerAppType</span></span>|[<span data-ttu-id="85c93-142">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="85c93-142">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="85c93-143">パートナー ・ アプリケーションの種類です。</span><span class="sxs-lookup"><span data-stu-id="85c93-143">Partner App type.</span></span> <span data-ttu-id="85c93-144">可能な値は、`unknown`、`singleTenantApp`、`multiTenantApp` です。</span><span class="sxs-lookup"><span data-stu-id="85c93-144">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="85c93-145">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="85c93-145">singleTenantAppId</span></span>|<span data-ttu-id="85c93-146">String</span><span class="sxs-lookup"><span data-stu-id="85c93-146">String</span></span>|<span data-ttu-id="85c93-147">パートナーのシングル テナントのアプリ ID</span><span class="sxs-lookup"><span data-stu-id="85c93-147">Partner Single tenant App id</span></span>|
|<span data-ttu-id="85c93-148">displayName</span><span class="sxs-lookup"><span data-stu-id="85c93-148">displayName</span></span>|<span data-ttu-id="85c93-149">String</span><span class="sxs-lookup"><span data-stu-id="85c93-149">String</span></span>|<span data-ttu-id="85c93-150">パートナー表示名</span><span class="sxs-lookup"><span data-stu-id="85c93-150">Partner display name</span></span>|
|<span data-ttu-id="85c93-151">isConfigured</span><span class="sxs-lookup"><span data-stu-id="85c93-151">isConfigured</span></span>|<span data-ttu-id="85c93-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="85c93-152">Boolean</span></span>|<span data-ttu-id="85c93-153">デバイス管理パートナーが構成されているかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="85c93-153">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="85c93-154">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="85c93-154">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="85c93-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85c93-155">DateTimeOffset</span></span>|<span data-ttu-id="85c93-156">PartnerDevices が削除されるときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="85c93-156">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="85c93-157">これは、古いもうすぐなります。</span><span class="sxs-lookup"><span data-stu-id="85c93-157">This will become obselete soon.</span></span>|
|<span data-ttu-id="85c93-158">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="85c93-158">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="85c93-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85c93-159">DateTimeOffset</span></span>|<span data-ttu-id="85c93-160">PartnerDevices は、非準拠とマークするときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="85c93-160">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="85c93-161">これは、古いもうすぐなります。</span><span class="sxs-lookup"><span data-stu-id="85c93-161">This will become obselete soon.</span></span>|
|<span data-ttu-id="85c93-162">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="85c93-162">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="85c93-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85c93-163">DateTimeOffset</span></span>|<span data-ttu-id="85c93-164">パートナー デバイスが削除されるときの日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="85c93-164">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="85c93-165">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="85c93-165">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="85c93-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85c93-166">DateTimeOffset</span></span>|<span data-ttu-id="85c93-167">パートナー デバイスが準拠していないとマークされるときの日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="85c93-167">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|

## <a name="relationships"></a><span data-ttu-id="85c93-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="85c93-168">Relationships</span></span>
<span data-ttu-id="85c93-169">なし</span><span class="sxs-lookup"><span data-stu-id="85c93-169">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="85c93-170">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="85c93-170">JSON Representation</span></span>
<span data-ttu-id="85c93-171">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="85c93-171">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementPartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "String",
  "displayName": "String",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "String (timestamp)",
  "whenPartnerDevicesWillBeRemovedDateTime": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "String (timestamp)"
}
```





