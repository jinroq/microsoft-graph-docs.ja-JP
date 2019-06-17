---
title: deviceManagementPartner リソースの種類
description: デバイス管理パートナーとの接続を表すエンティティです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c501c6e77dd50a399a6e2a70d2fb868c17dc6c6b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993040"
---
# <a name="devicemanagementpartner-resource-type"></a><span data-ttu-id="3de8c-103">deviceManagementPartner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3de8c-103">deviceManagementPartner resource type</span></span>

> <span data-ttu-id="3de8c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3de8c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3de8c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3de8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3de8c-106">デバイス管理パートナーとの接続を表すエンティティです。</span><span class="sxs-lookup"><span data-stu-id="3de8c-106">Entity which represents a connection to device management partner.</span></span>

## <a name="methods"></a><span data-ttu-id="3de8c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="3de8c-107">Methods</span></span>
|<span data-ttu-id="3de8c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="3de8c-108">Method</span></span>|<span data-ttu-id="3de8c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3de8c-109">Return Type</span></span>|<span data-ttu-id="3de8c-110">説明</span><span class="sxs-lookup"><span data-stu-id="3de8c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3de8c-111">List deviceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="3de8c-111">List deviceManagementPartners</span></span>](../api/intune-onboarding-devicemanagementpartner-list.md)|<span data-ttu-id="3de8c-112">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3de8c-112">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) collection</span></span>|<span data-ttu-id="3de8c-113">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="3de8c-113">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>|
|[<span data-ttu-id="3de8c-114">Get deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="3de8c-114">Get deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-get.md)|[<span data-ttu-id="3de8c-115">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="3de8c-115">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="3de8c-116">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3de8c-116">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="3de8c-117">Create deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="3de8c-117">Create deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-create.md)|[<span data-ttu-id="3de8c-118">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="3de8c-118">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="3de8c-119">新しい [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3de8c-119">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="3de8c-120">Delete deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="3de8c-120">Delete deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-delete.md)|<span data-ttu-id="3de8c-121">なし</span><span class="sxs-lookup"><span data-stu-id="3de8c-121">None</span></span>|<span data-ttu-id="3de8c-122">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="3de8c-122">Deletes a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>|
|[<span data-ttu-id="3de8c-123">Update deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="3de8c-123">Update deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-update.md)|[<span data-ttu-id="3de8c-124">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="3de8c-124">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="3de8c-125">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3de8c-125">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3de8c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3de8c-126">Properties</span></span>
|<span data-ttu-id="3de8c-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3de8c-127">Property</span></span>|<span data-ttu-id="3de8c-128">型</span><span class="sxs-lookup"><span data-stu-id="3de8c-128">Type</span></span>|<span data-ttu-id="3de8c-129">説明</span><span class="sxs-lookup"><span data-stu-id="3de8c-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3de8c-130">id</span><span class="sxs-lookup"><span data-stu-id="3de8c-130">id</span></span>|<span data-ttu-id="3de8c-131">文字列</span><span class="sxs-lookup"><span data-stu-id="3de8c-131">String</span></span>|<span data-ttu-id="3de8c-132">エンティティの Id</span><span class="sxs-lookup"><span data-stu-id="3de8c-132">Id of the entity</span></span>|
|<span data-ttu-id="3de8c-133">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="3de8c-133">lastHeartbeatDateTime</span></span>|<span data-ttu-id="3de8c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3de8c-134">DateTimeOffset</span></span>|<span data-ttu-id="3de8c-135">管理者が [デバイス管理パートナーに接続] オプションを有効にした後の最終ハートビートのタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="3de8c-135">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="3de8c-136">partnerState</span><span class="sxs-lookup"><span data-stu-id="3de8c-136">partnerState</span></span>|[<span data-ttu-id="3de8c-137">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="3de8c-137">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="3de8c-138">このテナントのパートナーの状態。</span><span class="sxs-lookup"><span data-stu-id="3de8c-138">Partner state of this tenant.</span></span> <span data-ttu-id="3de8c-139">使用可能な値: `unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="3de8c-139">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="3de8c-140">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="3de8c-140">partnerAppType</span></span>|[<span data-ttu-id="3de8c-141">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="3de8c-141">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="3de8c-142">パートナーアプリの種類。</span><span class="sxs-lookup"><span data-stu-id="3de8c-142">Partner App type.</span></span> <span data-ttu-id="3de8c-143">可能な値は、`unknown`、`singleTenantApp`、`multiTenantApp` です。</span><span class="sxs-lookup"><span data-stu-id="3de8c-143">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="3de8c-144">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="3de8c-144">singleTenantAppId</span></span>|<span data-ttu-id="3de8c-145">String</span><span class="sxs-lookup"><span data-stu-id="3de8c-145">String</span></span>|<span data-ttu-id="3de8c-146">パートナーのシングル テナントのアプリ ID</span><span class="sxs-lookup"><span data-stu-id="3de8c-146">Partner Single tenant App id</span></span>|
|<span data-ttu-id="3de8c-147">displayName</span><span class="sxs-lookup"><span data-stu-id="3de8c-147">displayName</span></span>|<span data-ttu-id="3de8c-148">String</span><span class="sxs-lookup"><span data-stu-id="3de8c-148">String</span></span>|<span data-ttu-id="3de8c-149">パートナー表示名</span><span class="sxs-lookup"><span data-stu-id="3de8c-149">Partner display name</span></span>|
|<span data-ttu-id="3de8c-150">isConfigured</span><span class="sxs-lookup"><span data-stu-id="3de8c-150">isConfigured</span></span>|<span data-ttu-id="3de8c-151">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="3de8c-151">Boolean</span></span>|<span data-ttu-id="3de8c-152">デバイス管理パートナーが構成されているかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="3de8c-152">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="3de8c-153">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="3de8c-153">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="3de8c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3de8c-154">DateTimeOffset</span></span>|<span data-ttu-id="3de8c-155">パートナーデバイスが削除される日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="3de8c-155">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="3de8c-156">これはすぐに obselete になります。</span><span class="sxs-lookup"><span data-stu-id="3de8c-156">This will become obselete soon.</span></span>|
|<span data-ttu-id="3de8c-157">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="3de8c-157">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="3de8c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3de8c-158">DateTimeOffset</span></span>|<span data-ttu-id="3de8c-159">パートナーデバイスが準拠していないとマークされるときの、UTC の DateTime。</span><span class="sxs-lookup"><span data-stu-id="3de8c-159">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="3de8c-160">これはすぐに obselete になります。</span><span class="sxs-lookup"><span data-stu-id="3de8c-160">This will become obselete soon.</span></span>|
|<span data-ttu-id="3de8c-161">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="3de8c-161">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="3de8c-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3de8c-162">DateTimeOffset</span></span>|<span data-ttu-id="3de8c-163">パートナー デバイスが削除されるときの日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="3de8c-163">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="3de8c-164">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="3de8c-164">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="3de8c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3de8c-165">DateTimeOffset</span></span>|<span data-ttu-id="3de8c-166">パートナー デバイスが準拠していないとマークされるときの日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="3de8c-166">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|

## <a name="relationships"></a><span data-ttu-id="3de8c-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3de8c-167">Relationships</span></span>
<span data-ttu-id="3de8c-168">なし</span><span class="sxs-lookup"><span data-stu-id="3de8c-168">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3de8c-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3de8c-169">JSON Representation</span></span>
<span data-ttu-id="3de8c-170">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3de8c-170">Here is a JSON representation of the resource.</span></span>
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





