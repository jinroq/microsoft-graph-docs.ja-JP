---
title: managedDeviceMobileAppConfigurationDeviceStatus リソースの種類
description: デバイスの MDM モバイルアプリ構成状態のプロパティ、継承されたプロパティ、アクションが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24f0275c9606e570db7b56685169667940cb79e3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989540"
---
# <a name="manageddevicemobileappconfigurationdevicestatus-resource-type"></a><span data-ttu-id="a064d-103">managedDeviceMobileAppConfigurationDeviceStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a064d-103">managedDeviceMobileAppConfigurationDeviceStatus resource type</span></span>

> <span data-ttu-id="a064d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a064d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a064d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a064d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a064d-106">デバイスの MDM モバイルアプリ構成状態のプロパティ、継承されたプロパティ、アクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a064d-106">Contains properties, inherited properties and actions for an MDM mobile app configuration status for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="a064d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a064d-107">Methods</span></span>
|<span data-ttu-id="a064d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a064d-108">Method</span></span>|<span data-ttu-id="a064d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a064d-109">Return Type</span></span>|<span data-ttu-id="a064d-110">説明</span><span class="sxs-lookup"><span data-stu-id="a064d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a064d-111">リスト managedDeviceMobileAppConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="a064d-111">List managedDeviceMobileAppConfigurationDeviceStatuses</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-list.md)|<span data-ttu-id="a064d-112">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a064d-112">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="a064d-113">[ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a064d-113">List properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects.</span></span>|
|[<span data-ttu-id="a064d-114">ManagedDeviceMobileAppConfigurationDeviceStatus を取得する</span><span class="sxs-lookup"><span data-stu-id="a064d-114">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-get.md)|[<span data-ttu-id="a064d-115">managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="a064d-115">managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|<span data-ttu-id="a064d-116">[ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a064d-116">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>|
|[<span data-ttu-id="a064d-117">ManagedDeviceMobileAppConfigurationDeviceStatus を作成する</span><span class="sxs-lookup"><span data-stu-id="a064d-117">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-create.md)|[<span data-ttu-id="a064d-118">managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="a064d-118">managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|<span data-ttu-id="a064d-119">新しい[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a064d-119">Create a new [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>|
|[<span data-ttu-id="a064d-120">ManagedDeviceMobileAppConfigurationDeviceStatus の削除</span><span class="sxs-lookup"><span data-stu-id="a064d-120">Delete managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-delete.md)|<span data-ttu-id="a064d-121">None</span><span class="sxs-lookup"><span data-stu-id="a064d-121">None</span></span>|<span data-ttu-id="a064d-122">[ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="a064d-122">Deletes a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>|
|[<span data-ttu-id="a064d-123">ManagedDeviceMobileAppConfigurationDeviceStatus の更新</span><span class="sxs-lookup"><span data-stu-id="a064d-123">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-update.md)|[<span data-ttu-id="a064d-124">managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="a064d-124">managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|<span data-ttu-id="a064d-125">[ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a064d-125">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a064d-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a064d-126">Properties</span></span>
|<span data-ttu-id="a064d-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a064d-127">Property</span></span>|<span data-ttu-id="a064d-128">型</span><span class="sxs-lookup"><span data-stu-id="a064d-128">Type</span></span>|<span data-ttu-id="a064d-129">説明</span><span class="sxs-lookup"><span data-stu-id="a064d-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a064d-130">id</span><span class="sxs-lookup"><span data-stu-id="a064d-130">id</span></span>|<span data-ttu-id="a064d-131">文字列</span><span class="sxs-lookup"><span data-stu-id="a064d-131">String</span></span>|<span data-ttu-id="a064d-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a064d-132">Key of the entity.</span></span>|
|<span data-ttu-id="a064d-133">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a064d-133">deviceDisplayName</span></span>|<span data-ttu-id="a064d-134">String</span><span class="sxs-lookup"><span data-stu-id="a064d-134">String</span></span>|<span data-ttu-id="a064d-135">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="a064d-135">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="a064d-136">userName</span><span class="sxs-lookup"><span data-stu-id="a064d-136">userName</span></span>|<span data-ttu-id="a064d-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a064d-137">String</span></span>|<span data-ttu-id="a064d-138">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="a064d-138">The User Name that is being reported</span></span>|
|<span data-ttu-id="a064d-139">deviceModel</span><span class="sxs-lookup"><span data-stu-id="a064d-139">deviceModel</span></span>|<span data-ttu-id="a064d-140">String</span><span class="sxs-lookup"><span data-stu-id="a064d-140">String</span></span>|<span data-ttu-id="a064d-141">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="a064d-141">The device model that is being reported</span></span>|
|<span data-ttu-id="a064d-142">platform</span><span class="sxs-lookup"><span data-stu-id="a064d-142">platform</span></span>|<span data-ttu-id="a064d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a064d-143">Int32</span></span>|<span data-ttu-id="a064d-144">レポートされているデバイスのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="a064d-144">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="a064d-145">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a064d-145">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="a064d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a064d-146">DateTimeOffset</span></span>|<span data-ttu-id="a064d-147">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="a064d-147">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="a064d-148">status</span><span class="sxs-lookup"><span data-stu-id="a064d-148">status</span></span>|[<span data-ttu-id="a064d-149">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a064d-149">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a064d-150">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="a064d-150">Compliance status of the policy report.</span></span> <span data-ttu-id="a064d-151">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="a064d-151">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a064d-152">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a064d-152">lastReportedDateTime</span></span>|<span data-ttu-id="a064d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a064d-153">DateTimeOffset</span></span>|<span data-ttu-id="a064d-154">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="a064d-154">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="a064d-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a064d-155">userPrincipalName</span></span>|<span data-ttu-id="a064d-156">String</span><span class="sxs-lookup"><span data-stu-id="a064d-156">String</span></span>|<span data-ttu-id="a064d-157">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="a064d-157">UserPrincipalName.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a064d-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a064d-158">Relationships</span></span>
<span data-ttu-id="a064d-159">なし</span><span class="sxs-lookup"><span data-stu-id="a064d-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a064d-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a064d-160">JSON Representation</span></span>
<span data-ttu-id="a064d-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a064d-161">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "platform": 1024,
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```





