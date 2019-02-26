---
title: user リソースの種類
description: Azure Active Directory ユーザー オブジェクトを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a7a6c87b5c073e00b660db807ff38c454c302d94
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253408"
---
# <a name="user-resource-type"></a><span data-ttu-id="4c1ae-103">user リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4c1ae-103">user resource type</span></span>

> <span data-ttu-id="4c1ae-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c1ae-105">Azure Active Directory ユーザー オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-105">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="4c1ae-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="4c1ae-106">Methods</span></span>
|<span data-ttu-id="4c1ae-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4c1ae-107">Method</span></span>|<span data-ttu-id="4c1ae-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4c1ae-108">Return Type</span></span>|<span data-ttu-id="4c1ae-109">説明</span><span class="sxs-lookup"><span data-stu-id="4c1ae-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c1ae-110">[ユーザーオブジェクトを一覧表示](../api/intune-shared-user-list.md)します。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-110">[List users](../api/intune-shared-user-list.md) objects.</span></span>|<span data-ttu-id="4c1ae-111">[user](../resources/intune-shared-user.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4c1ae-111">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="4c1ae-112">[user](../resources/intune-shared-user.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-112">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>|
|<span data-ttu-id="4c1ae-113">[ユーザー](../api/intune-shared-user-get.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-113">[Get user](../api/intune-shared-user-get.md) object.</span></span>|<span data-ttu-id="4c1ae-114">[user](../resources/intune-shared-user.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4c1ae-114">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="4c1ae-115">[user](../resources/intune-shared-user.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-115">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="4c1ae-116">[ユーザー](../api/intune-shared-user-create.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-116">[Create user](../api/intune-shared-user-create.md) object.</span></span>|<span data-ttu-id="4c1ae-117">[user](../resources/intune-shared-user.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4c1ae-117">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="4c1ae-118">新しい [user](../resources/intune-shared-user.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-118">Create a new [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="4c1ae-119">[ユーザーを削除](../api/intune-shared-user-delete.md)します。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-119">[Delete user](../api/intune-shared-user-delete.md).</span></span>|<span data-ttu-id="4c1ae-120">なし</span><span class="sxs-lookup"><span data-stu-id="4c1ae-120">None</span></span>|<span data-ttu-id="4c1ae-121">[user](../resources/intune-shared-user.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-121">Deletes a [user](../resources/intune-shared-user.md).</span></span>|
|<span data-ttu-id="4c1ae-122">[ユーザー](../api/intune-shared-user-update.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-122">[Update user](../api/intune-shared-user-update.md) object.</span></span>|[<span data-ttu-id="4c1ae-123">user</span><span class="sxs-lookup"><span data-stu-id="4c1ae-123">user</span></span>](../resources/intune-shared-user.md)|<span data-ttu-id="4c1ae-124">[user](../resources/intune-shared-user.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-124">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="4c1ae-125">**デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="4c1ae-125">**Device management**</span></span>|
|[<span data-ttu-id="4c1ae-126">removeAllDevicesFromManagement アクション</span><span class="sxs-lookup"><span data-stu-id="4c1ae-126">removeAllDevicesFromManagement action</span></span>](../api/intune-shared-user-removealldevicesfrommanagement.md)|<span data-ttu-id="4c1ae-127">なし</span><span class="sxs-lookup"><span data-stu-id="4c1ae-127">None</span></span>|<span data-ttu-id="4c1ae-128">対象ユーザーの管理からすべてのデバイスを破棄します</span><span class="sxs-lookup"><span data-stu-id="4c1ae-128">Retire all devices from management for this user</span></span>|
|<span data-ttu-id="4c1ae-129">**モバイルアプリ管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="4c1ae-129">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="4c1ae-130">getManagedAppDiagnosticStatuses 関数</span><span class="sxs-lookup"><span data-stu-id="4c1ae-130">getManagedAppDiagnosticStatuses function</span></span>](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="4c1ae-131">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4c1ae-131">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="4c1ae-132">特定のユーザーの診断検証状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-132">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="4c1ae-133">getManagedAppPolicies 関数</span><span class="sxs-lookup"><span data-stu-id="4c1ae-133">getManagedAppPolicies function</span></span>](../api/intune-shared-user-getmanagedapppolicies.md)|<span data-ttu-id="4c1ae-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4c1ae-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="4c1ae-135">特定のユーザーのアプリ制限を取得します。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-135">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="4c1ae-136">wipeManagedAppRegistrationsByDeviceTag アクション</span><span class="sxs-lookup"><span data-stu-id="4c1ae-136">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="4c1ae-137">なし</span><span class="sxs-lookup"><span data-stu-id="4c1ae-137">None</span></span>|<span data-ttu-id="4c1ae-138">指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-138">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="4c1ae-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c1ae-139">Properties</span></span>
|<span data-ttu-id="4c1ae-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c1ae-140">Property</span></span>|<span data-ttu-id="4c1ae-141">型</span><span class="sxs-lookup"><span data-stu-id="4c1ae-141">Type</span></span>|<span data-ttu-id="4c1ae-142">説明</span><span class="sxs-lookup"><span data-stu-id="4c1ae-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c1ae-143">id</span><span class="sxs-lookup"><span data-stu-id="4c1ae-143">id</span></span>|<span data-ttu-id="4c1ae-144">String</span><span class="sxs-lookup"><span data-stu-id="4c1ae-144">String</span></span>|<span data-ttu-id="4c1ae-145">ユーザーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-145">Unique identifier of the user.</span></span>|
|<span data-ttu-id="4c1ae-146">**オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="4c1ae-146">**Onboarding**</span></span>|
|<span data-ttu-id="4c1ae-147">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="4c1ae-147">deviceEnrollmentLimit</span></span>|<span data-ttu-id="4c1ae-148">Int32</span><span class="sxs-lookup"><span data-stu-id="4c1ae-148">Int32</span></span>|<span data-ttu-id="4c1ae-149">ユーザーが登録を許可されているデバイスの最大数。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-149">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="4c1ae-150">使用できる値は 5 または 1000 です。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-150">Allowed values are 5 or 1000.</span></span>|


## <a name="relationships"></a><span data-ttu-id="4c1ae-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4c1ae-151">Relationships</span></span>
|<span data-ttu-id="4c1ae-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4c1ae-152">Relationship</span></span>|<span data-ttu-id="4c1ae-153">型</span><span class="sxs-lookup"><span data-stu-id="4c1ae-153">Type</span></span>|<span data-ttu-id="4c1ae-154">説明</span><span class="sxs-lookup"><span data-stu-id="4c1ae-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c1ae-155">**デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="4c1ae-155">**Device management**</span></span>|
|<span data-ttu-id="4c1ae-156">managedDevices</span><span class="sxs-lookup"><span data-stu-id="4c1ae-156">managedDevices</span></span>|<span data-ttu-id="4c1ae-157">[managedDevice](../resources/intune-devices-manageddevice.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4c1ae-157">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="4c1ae-158">対象ユーザーに関連付けられている管理対象デバイス。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-158">The managed devices associated with the user.</span></span>|
|<span data-ttu-id="4c1ae-159">**モバイルアプリ管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="4c1ae-159">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="4c1ae-160">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="4c1ae-160">managedAppRegistrations</span></span>|<span data-ttu-id="4c1ae-161">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4c1ae-161">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="4c1ae-162">対象ユーザーに属する 0 個以上の管理対象アプリ登録。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-162">Zero or more managed app registrations that belong to the user.</span></span>|
|<span data-ttu-id="4c1ae-163">**トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="4c1ae-163">**Troubleshooting**</span></span>|
|<span data-ttu-id="4c1ae-164">deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="4c1ae-164">deviceManagementTroubleshootingEvents</span></span>|<span data-ttu-id="4c1ae-165">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4c1ae-165">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="4c1ae-166">対象ユーザーのトラブルシューティング イベントの一覧です。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-166">The list of troubleshooting events for this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4c1ae-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4c1ae-167">JSON Representation</span></span>
<span data-ttu-id="4c1ae-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4c1ae-168">Here is a JSON representation of the resource.</span></span>
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
