---
title: user リソースの種類
description: Azure Active Directory ユーザー オブジェクトを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d8fc3604329a5062a8fe1afb90c2ac64f52f0bed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036835"
---
# <a name="user-resource-type"></a><span data-ttu-id="b851a-103">user リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b851a-103">user resource type</span></span>

> <span data-ttu-id="b851a-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b851a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b851a-105">Azure Active Directory ユーザー オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="b851a-105">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="b851a-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b851a-106">Methods</span></span>
|<span data-ttu-id="b851a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b851a-107">Method</span></span>|<span data-ttu-id="b851a-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b851a-108">Return Type</span></span>|<span data-ttu-id="b851a-109">説明</span><span class="sxs-lookup"><span data-stu-id="b851a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b851a-110">[ユーザーオブジェクトを一覧表示](../api/intune-shared-user-list.md)します。</span><span class="sxs-lookup"><span data-stu-id="b851a-110">[List users](../api/intune-shared-user-list.md) objects.</span></span>|<span data-ttu-id="b851a-111">[user](../resources/intune-shared-user.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b851a-111">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="b851a-112">[user](../resources/intune-shared-user.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b851a-112">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>|
|<span data-ttu-id="b851a-113">[ユーザー](../api/intune-shared-user-get.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="b851a-113">[Get user](../api/intune-shared-user-get.md) object.</span></span>|<span data-ttu-id="b851a-114">[user](../resources/intune-shared-user.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b851a-114">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="b851a-115">[user](../resources/intune-shared-user.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b851a-115">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="b851a-116">[ユーザー](../api/intune-shared-user-create.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b851a-116">[Create user](../api/intune-shared-user-create.md) object.</span></span>|<span data-ttu-id="b851a-117">[user](../resources/intune-shared-user.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b851a-117">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="b851a-118">新しい [user](../resources/intune-shared-user.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b851a-118">Create a new [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="b851a-119">[ユーザーを削除](../api/intune-shared-user-delete.md)します。</span><span class="sxs-lookup"><span data-stu-id="b851a-119">[Delete user](../api/intune-shared-user-delete.md).</span></span>|<span data-ttu-id="b851a-120">None</span><span class="sxs-lookup"><span data-stu-id="b851a-120">None</span></span>|<span data-ttu-id="b851a-121">[user](../resources/intune-shared-user.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="b851a-121">Deletes a [user](../resources/intune-shared-user.md).</span></span>|
|<span data-ttu-id="b851a-122">[ユーザー](../api/intune-shared-user-update.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="b851a-122">[Update user](../api/intune-shared-user-update.md) object.</span></span>|[<span data-ttu-id="b851a-123">user</span><span class="sxs-lookup"><span data-stu-id="b851a-123">user</span></span>](../resources/intune-shared-user.md)|<span data-ttu-id="b851a-124">[user](../resources/intune-shared-user.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b851a-124">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="b851a-125">**デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="b851a-125">**Device management**</span></span>|
|[<span data-ttu-id="b851a-126">removeAllDevicesFromManagement アクション</span><span class="sxs-lookup"><span data-stu-id="b851a-126">removeAllDevicesFromManagement action</span></span>](../api/intune-shared-user-removealldevicesfrommanagement.md)|<span data-ttu-id="b851a-127">None</span><span class="sxs-lookup"><span data-stu-id="b851a-127">None</span></span>|<span data-ttu-id="b851a-128">対象ユーザーの管理からすべてのデバイスを破棄します</span><span class="sxs-lookup"><span data-stu-id="b851a-128">Retire all devices from management for this user</span></span>|
|<span data-ttu-id="b851a-129">**モバイル アプリの管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="b851a-129">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="b851a-130">getManagedAppDiagnosticStatuses 関数</span><span class="sxs-lookup"><span data-stu-id="b851a-130">getManagedAppDiagnosticStatuses function</span></span>](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="b851a-131">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b851a-131">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="b851a-132">特定のユーザーの診断検証状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="b851a-132">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="b851a-133">getManagedAppPolicies 関数</span><span class="sxs-lookup"><span data-stu-id="b851a-133">getManagedAppPolicies function</span></span>](../api/intune-shared-user-getmanagedapppolicies.md)|<span data-ttu-id="b851a-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b851a-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="b851a-135">特定のユーザーのアプリ制限を取得します。</span><span class="sxs-lookup"><span data-stu-id="b851a-135">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="b851a-136">wipeManagedAppRegistrationsByDeviceTag アクション</span><span class="sxs-lookup"><span data-stu-id="b851a-136">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="b851a-137">なし</span><span class="sxs-lookup"><span data-stu-id="b851a-137">None</span></span>|<span data-ttu-id="b851a-138">指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="b851a-138">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="b851a-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b851a-139">Properties</span></span>
|<span data-ttu-id="b851a-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b851a-140">Property</span></span>|<span data-ttu-id="b851a-141">型</span><span class="sxs-lookup"><span data-stu-id="b851a-141">Type</span></span>|<span data-ttu-id="b851a-142">説明</span><span class="sxs-lookup"><span data-stu-id="b851a-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b851a-143">id</span><span class="sxs-lookup"><span data-stu-id="b851a-143">id</span></span>|<span data-ttu-id="b851a-144">String</span><span class="sxs-lookup"><span data-stu-id="b851a-144">String</span></span>|<span data-ttu-id="b851a-145">ユーザーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="b851a-145">Unique identifier of the user.</span></span>|
|<span data-ttu-id="b851a-146">**オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="b851a-146">**Onboarding**</span></span>|
|<span data-ttu-id="b851a-147">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="b851a-147">deviceEnrollmentLimit</span></span>|<span data-ttu-id="b851a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="b851a-148">Int32</span></span>|<span data-ttu-id="b851a-149">ユーザーが登録を許可されているデバイスの最大数。</span><span class="sxs-lookup"><span data-stu-id="b851a-149">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="b851a-150">使用できる値は 5 または 1000 です。</span><span class="sxs-lookup"><span data-stu-id="b851a-150">Allowed values are 5 or 1000.</span></span>|


## <a name="relationships"></a><span data-ttu-id="b851a-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b851a-151">Relationships</span></span>
|<span data-ttu-id="b851a-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b851a-152">Relationship</span></span>|<span data-ttu-id="b851a-153">型</span><span class="sxs-lookup"><span data-stu-id="b851a-153">Type</span></span>|<span data-ttu-id="b851a-154">説明</span><span class="sxs-lookup"><span data-stu-id="b851a-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b851a-155">**デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="b851a-155">**Device management**</span></span>|
|<span data-ttu-id="b851a-156">managedDevices</span><span class="sxs-lookup"><span data-stu-id="b851a-156">managedDevices</span></span>|<span data-ttu-id="b851a-157">[managedDevice](../resources/intune-devices-manageddevice.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b851a-157">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="b851a-158">対象ユーザーに関連付けられている管理対象デバイス。</span><span class="sxs-lookup"><span data-stu-id="b851a-158">The managed devices associated with the user.</span></span>|
|<span data-ttu-id="b851a-159">**モバイル アプリの管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="b851a-159">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="b851a-160">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="b851a-160">managedAppRegistrations</span></span>|<span data-ttu-id="b851a-161">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b851a-161">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="b851a-162">対象ユーザーに属する 0 個以上の管理対象アプリ登録。</span><span class="sxs-lookup"><span data-stu-id="b851a-162">Zero or more managed app registrations that belong to the user.</span></span>|
|<span data-ttu-id="b851a-163">**トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="b851a-163">**Troubleshooting**</span></span>|
|<span data-ttu-id="b851a-164">deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="b851a-164">deviceManagementTroubleshootingEvents</span></span>|<span data-ttu-id="b851a-165">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b851a-165">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="b851a-166">対象ユーザーのトラブルシューティング イベントの一覧です。</span><span class="sxs-lookup"><span data-stu-id="b851a-166">The list of troubleshooting events for this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b851a-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b851a-167">JSON Representation</span></span>
<span data-ttu-id="b851a-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b851a-168">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "@odata.type": "microsoft.graph.user"
}
--> 
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 5
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Resource microsoft.graph.user is defined in multiple files: /api-reference/v1.0/resources/intune_shared_user.md, /api-reference/v1.0/resources/user.md",
  ]
}-->
