---
title: managedDeviceMobileAppConfigurationDeviceStatus リソースの種類
description: デバイスの MDM モバイルアプリ構成状態のプロパティ、継承されたプロパティ、アクションが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b412bad72649f1965e9945a9dacf03d6ce6cf3e2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005318"
---
# <a name="manageddevicemobileappconfigurationdevicestatus-resource-type"></a><span data-ttu-id="155a4-103">managedDeviceMobileAppConfigurationDeviceStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="155a4-103">managedDeviceMobileAppConfigurationDeviceStatus resource type</span></span>

> <span data-ttu-id="155a4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="155a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="155a4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="155a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="155a4-106">デバイスの MDM モバイルアプリ構成状態のプロパティ、継承されたプロパティ、アクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="155a4-106">Contains properties, inherited properties and actions for an MDM mobile app configuration status for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="155a4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="155a4-107">Methods</span></span>
|<span data-ttu-id="155a4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="155a4-108">Method</span></span>|<span data-ttu-id="155a4-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="155a4-109">Return Type</span></span>|<span data-ttu-id="155a4-110">説明</span><span class="sxs-lookup"><span data-stu-id="155a4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="155a4-111">リスト managedDeviceMobileAppConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="155a4-111">List managedDeviceMobileAppConfigurationDeviceStatuses</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-list.md)|<span data-ttu-id="155a4-112">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="155a4-112">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="155a4-113">[ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="155a4-113">List properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects.</span></span>|
|[<span data-ttu-id="155a4-114">ManagedDeviceMobileAppConfigurationDeviceStatus を取得する</span><span class="sxs-lookup"><span data-stu-id="155a4-114">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-get.md)|[<span data-ttu-id="155a4-115">managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="155a4-115">managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|<span data-ttu-id="155a4-116">[ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="155a4-116">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>|
|[<span data-ttu-id="155a4-117">ManagedDeviceMobileAppConfigurationDeviceStatus を作成する</span><span class="sxs-lookup"><span data-stu-id="155a4-117">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-create.md)|[<span data-ttu-id="155a4-118">managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="155a4-118">managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|<span data-ttu-id="155a4-119">新しい[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="155a4-119">Create a new [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>|
|[<span data-ttu-id="155a4-120">ManagedDeviceMobileAppConfigurationDeviceStatus の削除</span><span class="sxs-lookup"><span data-stu-id="155a4-120">Delete managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-delete.md)|<span data-ttu-id="155a4-121">None</span><span class="sxs-lookup"><span data-stu-id="155a4-121">None</span></span>|<span data-ttu-id="155a4-122">[ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="155a4-122">Deletes a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>|
|[<span data-ttu-id="155a4-123">ManagedDeviceMobileAppConfigurationDeviceStatus の更新</span><span class="sxs-lookup"><span data-stu-id="155a4-123">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-update.md)|[<span data-ttu-id="155a4-124">managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="155a4-124">managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|<span data-ttu-id="155a4-125">[ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="155a4-125">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="155a4-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="155a4-126">Properties</span></span>
|<span data-ttu-id="155a4-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="155a4-127">Property</span></span>|<span data-ttu-id="155a4-128">型</span><span class="sxs-lookup"><span data-stu-id="155a4-128">Type</span></span>|<span data-ttu-id="155a4-129">説明</span><span class="sxs-lookup"><span data-stu-id="155a4-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="155a4-130">id</span><span class="sxs-lookup"><span data-stu-id="155a4-130">id</span></span>|<span data-ttu-id="155a4-131">文字列</span><span class="sxs-lookup"><span data-stu-id="155a4-131">String</span></span>|<span data-ttu-id="155a4-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="155a4-132">Key of the entity.</span></span>|
|<span data-ttu-id="155a4-133">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="155a4-133">deviceDisplayName</span></span>|<span data-ttu-id="155a4-134">String</span><span class="sxs-lookup"><span data-stu-id="155a4-134">String</span></span>|<span data-ttu-id="155a4-135">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="155a4-135">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="155a4-136">userName</span><span class="sxs-lookup"><span data-stu-id="155a4-136">userName</span></span>|<span data-ttu-id="155a4-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="155a4-137">String</span></span>|<span data-ttu-id="155a4-138">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="155a4-138">The User Name that is being reported</span></span>|
|<span data-ttu-id="155a4-139">deviceModel</span><span class="sxs-lookup"><span data-stu-id="155a4-139">deviceModel</span></span>|<span data-ttu-id="155a4-140">String</span><span class="sxs-lookup"><span data-stu-id="155a4-140">String</span></span>|<span data-ttu-id="155a4-141">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="155a4-141">The device model that is being reported</span></span>|
|<span data-ttu-id="155a4-142">platform</span><span class="sxs-lookup"><span data-stu-id="155a4-142">platform</span></span>|<span data-ttu-id="155a4-143">Int32</span><span class="sxs-lookup"><span data-stu-id="155a4-143">Int32</span></span>|<span data-ttu-id="155a4-144">レポートされているデバイスのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="155a4-144">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="155a4-145">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="155a4-145">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="155a4-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="155a4-146">DateTimeOffset</span></span>|<span data-ttu-id="155a4-147">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="155a4-147">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="155a4-148">status</span><span class="sxs-lookup"><span data-stu-id="155a4-148">status</span></span>|[<span data-ttu-id="155a4-149">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="155a4-149">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="155a4-150">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="155a4-150">Compliance status of the policy report.</span></span> <span data-ttu-id="155a4-151">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="155a4-151">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="155a4-152">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="155a4-152">lastReportedDateTime</span></span>|<span data-ttu-id="155a4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="155a4-153">DateTimeOffset</span></span>|<span data-ttu-id="155a4-154">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="155a4-154">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="155a4-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="155a4-155">userPrincipalName</span></span>|<span data-ttu-id="155a4-156">String</span><span class="sxs-lookup"><span data-stu-id="155a4-156">String</span></span>|<span data-ttu-id="155a4-157">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="155a4-157">UserPrincipalName.</span></span>|

## <a name="relationships"></a><span data-ttu-id="155a4-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="155a4-158">Relationships</span></span>
<span data-ttu-id="155a4-159">なし</span><span class="sxs-lookup"><span data-stu-id="155a4-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="155a4-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="155a4-160">JSON Representation</span></span>
<span data-ttu-id="155a4-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="155a4-161">Here is a JSON representation of the resource.</span></span>
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





