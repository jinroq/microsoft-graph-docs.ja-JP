---
title: deviceManagementPartner リソースの種類
description: デバイス管理パートナーとの接続を表すエンティティです。
author: tfitzmac
ms.openlocfilehash: 2174f81f7b9c5e73c3bc42a54cb030cf50c216d2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354041"
---
# <a name="devicemanagementpartner-resource-type"></a><span data-ttu-id="a1efe-103">deviceManagementPartner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a1efe-103">deviceManagementPartner resource type</span></span>

> <span data-ttu-id="a1efe-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a1efe-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1efe-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1efe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1efe-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a1efe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1efe-107">デバイス管理パートナーとの接続を表すエンティティです。</span><span class="sxs-lookup"><span data-stu-id="a1efe-107">Entity which represents a connection to device management partner.</span></span>
## <a name="methods"></a><span data-ttu-id="a1efe-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a1efe-108">Methods</span></span>
|<span data-ttu-id="a1efe-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="a1efe-109">Method</span></span>|<span data-ttu-id="a1efe-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a1efe-110">Return Type</span></span>|<span data-ttu-id="a1efe-111">説明</span><span class="sxs-lookup"><span data-stu-id="a1efe-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a1efe-112">List deviceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="a1efe-112">List deviceManagementPartners</span></span>](../api/intune-onboarding-devicemanagementpartner-list.md)|<span data-ttu-id="a1efe-113">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a1efe-113">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) collection</span></span>|<span data-ttu-id="a1efe-114">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a1efe-114">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>|
|[<span data-ttu-id="a1efe-115">Get deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="a1efe-115">Get deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-get.md)|[<span data-ttu-id="a1efe-116">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="a1efe-116">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="a1efe-117">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a1efe-117">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="a1efe-118">Create deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="a1efe-118">Create deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-create.md)|[<span data-ttu-id="a1efe-119">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="a1efe-119">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="a1efe-120">新しい [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a1efe-120">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="a1efe-121">Delete deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="a1efe-121">Delete deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-delete.md)|<span data-ttu-id="a1efe-122">なし</span><span class="sxs-lookup"><span data-stu-id="a1efe-122">None</span></span>|<span data-ttu-id="a1efe-123">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="a1efe-123">Deletes a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>|
|[<span data-ttu-id="a1efe-124">Update deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="a1efe-124">Update deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-update.md)|[<span data-ttu-id="a1efe-125">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="a1efe-125">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="a1efe-126">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a1efe-126">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a1efe-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1efe-127">Properties</span></span>
|<span data-ttu-id="a1efe-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1efe-128">Property</span></span>|<span data-ttu-id="a1efe-129">種類</span><span class="sxs-lookup"><span data-stu-id="a1efe-129">Type</span></span>|<span data-ttu-id="a1efe-130">説明</span><span class="sxs-lookup"><span data-stu-id="a1efe-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1efe-131">ID</span><span class="sxs-lookup"><span data-stu-id="a1efe-131">id</span></span>|<span data-ttu-id="a1efe-132">String</span><span class="sxs-lookup"><span data-stu-id="a1efe-132">String</span></span>|<span data-ttu-id="a1efe-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a1efe-133">Not yet documented</span></span>|
|<span data-ttu-id="a1efe-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="a1efe-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="a1efe-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1efe-135">DateTimeOffset</span></span>|<span data-ttu-id="a1efe-136">管理者が [デバイス管理パートナーに接続] オプションを有効にした後の最終ハートビートのタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="a1efe-136">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="a1efe-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="a1efe-137">partnerState</span></span>|[<span data-ttu-id="a1efe-138">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="a1efe-138">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="a1efe-139">このテナントのパートナーの状態です。</span><span class="sxs-lookup"><span data-stu-id="a1efe-139">Partner state of this tenant.</span></span> <span data-ttu-id="a1efe-140">使用可能な値: `unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="a1efe-140">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="a1efe-141">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="a1efe-141">partnerAppType</span></span>|[<span data-ttu-id="a1efe-142">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="a1efe-142">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="a1efe-143">パートナー ・ アプリケーションの種類です。</span><span class="sxs-lookup"><span data-stu-id="a1efe-143">Partner App type.</span></span> <span data-ttu-id="a1efe-144">可能な値は、`unknown`、`singleTenantApp`、`multiTenantApp` です。</span><span class="sxs-lookup"><span data-stu-id="a1efe-144">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="a1efe-145">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="a1efe-145">singleTenantAppId</span></span>|<span data-ttu-id="a1efe-146">String</span><span class="sxs-lookup"><span data-stu-id="a1efe-146">String</span></span>|<span data-ttu-id="a1efe-147">パートナーのシングル テナントのアプリ ID</span><span class="sxs-lookup"><span data-stu-id="a1efe-147">Partner Single tenant App id</span></span>|
|<span data-ttu-id="a1efe-148">displayName</span><span class="sxs-lookup"><span data-stu-id="a1efe-148">displayName</span></span>|<span data-ttu-id="a1efe-149">String</span><span class="sxs-lookup"><span data-stu-id="a1efe-149">String</span></span>|<span data-ttu-id="a1efe-150">パートナー表示名</span><span class="sxs-lookup"><span data-stu-id="a1efe-150">Partner display name</span></span>|
|<span data-ttu-id="a1efe-151">isConfigured</span><span class="sxs-lookup"><span data-stu-id="a1efe-151">isConfigured</span></span>|<span data-ttu-id="a1efe-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1efe-152">Boolean</span></span>|<span data-ttu-id="a1efe-153">デバイス管理パートナーが構成されているかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="a1efe-153">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="a1efe-154">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="a1efe-154">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="a1efe-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1efe-155">DateTimeOffset</span></span>|<span data-ttu-id="a1efe-156">PartnerDevices が削除されるときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="a1efe-156">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="a1efe-157">これは、古いもうすぐなります。</span><span class="sxs-lookup"><span data-stu-id="a1efe-157">This will become obselete soon.</span></span>|
|<span data-ttu-id="a1efe-158">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="a1efe-158">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="a1efe-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1efe-159">DateTimeOffset</span></span>|<span data-ttu-id="a1efe-160">PartnerDevices は、非準拠とマークするときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="a1efe-160">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="a1efe-161">これは、古いもうすぐなります。</span><span class="sxs-lookup"><span data-stu-id="a1efe-161">This will become obselete soon.</span></span>|
|<span data-ttu-id="a1efe-162">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1efe-162">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="a1efe-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1efe-163">DateTimeOffset</span></span>|<span data-ttu-id="a1efe-164">パートナー デバイスが削除されるときの日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="a1efe-164">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="a1efe-165">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="a1efe-165">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="a1efe-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1efe-166">DateTimeOffset</span></span>|<span data-ttu-id="a1efe-167">パートナー デバイスが準拠していないとマークされるときの日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="a1efe-167">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1efe-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a1efe-168">Relationships</span></span>
<span data-ttu-id="a1efe-169">なし</span><span class="sxs-lookup"><span data-stu-id="a1efe-169">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a1efe-170">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a1efe-170">JSON Representation</span></span>
<span data-ttu-id="a1efe-171">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a1efe-171">Here is a JSON representation of the resource.</span></span>
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





