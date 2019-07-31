---
title: importedAppleDeviceIdentity リソースの種類
description: ImportedAppleDeviceIdentity リソースは、Apple デバイスのインポートされたデバイス id を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 08e9487fc4c3f63399027e0fe40b5c90ba761547
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999165"
---
# <a name="importedappledeviceidentity-resource-type"></a><span data-ttu-id="964e5-103">importedAppleDeviceIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="964e5-103">importedAppleDeviceIdentity resource type</span></span>

> <span data-ttu-id="964e5-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="964e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="964e5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="964e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="964e5-106">ImportedAppleDeviceIdentity リソースは、Apple デバイスのインポートされたデバイス id を表します。</span><span class="sxs-lookup"><span data-stu-id="964e5-106">The importedAppleDeviceIdentity resource represents the imported device identity of an Apple device .</span></span>

## <a name="methods"></a><span data-ttu-id="964e5-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="964e5-107">Methods</span></span>
|<span data-ttu-id="964e5-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="964e5-108">Method</span></span>|<span data-ttu-id="964e5-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="964e5-109">Return Type</span></span>|<span data-ttu-id="964e5-110">説明</span><span class="sxs-lookup"><span data-stu-id="964e5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="964e5-111">リスト importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="964e5-111">List importedAppleDeviceIdentities</span></span>](../api/intune-enrollment-importedappledeviceidentity-list.md)|<span data-ttu-id="964e5-112">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="964e5-112">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="964e5-113">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="964e5-113">List properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="964e5-114">ImportedAppleDeviceIdentity を取得する</span><span class="sxs-lookup"><span data-stu-id="964e5-114">Get importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-get.md)|[<span data-ttu-id="964e5-115">importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="964e5-115">importedAppleDeviceIdentity</span></span>](../resources/intune-enrollment-importedappledeviceidentity.md)|<span data-ttu-id="964e5-116">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="964e5-116">Read properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="964e5-117">ImportedAppleDeviceIdentity を作成する</span><span class="sxs-lookup"><span data-stu-id="964e5-117">Create importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-create.md)|[<span data-ttu-id="964e5-118">importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="964e5-118">importedAppleDeviceIdentity</span></span>](../resources/intune-enrollment-importedappledeviceidentity.md)|<span data-ttu-id="964e5-119">新しい[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="964e5-119">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="964e5-120">ImportedAppleDeviceIdentity の削除</span><span class="sxs-lookup"><span data-stu-id="964e5-120">Delete importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-delete.md)|<span data-ttu-id="964e5-121">None</span><span class="sxs-lookup"><span data-stu-id="964e5-121">None</span></span>|<span data-ttu-id="964e5-122">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="964e5-122">Deletes a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>|
|[<span data-ttu-id="964e5-123">ImportedAppleDeviceIdentity の更新</span><span class="sxs-lookup"><span data-stu-id="964e5-123">Update importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-update.md)|[<span data-ttu-id="964e5-124">importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="964e5-124">importedAppleDeviceIdentity</span></span>](../resources/intune-enrollment-importedappledeviceidentity.md)|<span data-ttu-id="964e5-125">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="964e5-125">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="964e5-126">importAppleDeviceIdentityList アクション</span><span class="sxs-lookup"><span data-stu-id="964e5-126">importAppleDeviceIdentityList action</span></span>](../api/intune-enrollment-importedappledeviceidentity-importappledeviceidentitylist.md)|<span data-ttu-id="964e5-127">[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="964e5-127">[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection</span></span>|<span data-ttu-id="964e5-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="964e5-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="964e5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="964e5-129">Properties</span></span>
|<span data-ttu-id="964e5-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="964e5-130">Property</span></span>|<span data-ttu-id="964e5-131">型</span><span class="sxs-lookup"><span data-stu-id="964e5-131">Type</span></span>|<span data-ttu-id="964e5-132">説明</span><span class="sxs-lookup"><span data-stu-id="964e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="964e5-133">id</span><span class="sxs-lookup"><span data-stu-id="964e5-133">id</span></span>|<span data-ttu-id="964e5-134">String</span><span class="sxs-lookup"><span data-stu-id="964e5-134">String</span></span>|<span data-ttu-id="964e5-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="964e5-135">Key of the entity.</span></span>|
|<span data-ttu-id="964e5-136">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="964e5-136">serialNumber</span></span>|<span data-ttu-id="964e5-137">String</span><span class="sxs-lookup"><span data-stu-id="964e5-137">String</span></span>|<span data-ttu-id="964e5-138">デバイスのシリアル番号</span><span class="sxs-lookup"><span data-stu-id="964e5-138">Device serial number</span></span>|
|<span data-ttu-id="964e5-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="964e5-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="964e5-140">String</span><span class="sxs-lookup"><span data-stu-id="964e5-140">String</span></span>|<span data-ttu-id="964e5-141">登録プロファイル Id 管理者が次回の登録時にデバイスに適用する予定</span><span class="sxs-lookup"><span data-stu-id="964e5-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="964e5-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="964e5-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="964e5-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="964e5-143">DateTimeOffset</span></span>|<span data-ttu-id="964e5-144">時間登録プロファイルがデバイスに割り当てられている</span><span class="sxs-lookup"><span data-stu-id="964e5-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="964e5-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="964e5-145">isSupervised</span></span>|<span data-ttu-id="964e5-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="964e5-146">Boolean</span></span>|<span data-ttu-id="964e5-147">Apple デバイスが監視されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="964e5-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="964e5-148">詳細情報は次のとおりです。https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="964e5-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="964e5-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="964e5-149">discoverySource</span></span>|[<span data-ttu-id="964e5-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="964e5-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="964e5-151">Apple デバイスの検出ソース。</span><span class="sxs-lookup"><span data-stu-id="964e5-151">Apple device discovery source.</span></span> <span data-ttu-id="964e5-152">可能な値は、`unknown`、`adminImport`、`deviceEnrollmentProgram` です。</span><span class="sxs-lookup"><span data-stu-id="964e5-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="964e5-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="964e5-153">createdDateTime</span></span>|<span data-ttu-id="964e5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="964e5-154">DateTimeOffset</span></span>|<span data-ttu-id="964e5-155">デバイスの日時の作成日時</span><span class="sxs-lookup"><span data-stu-id="964e5-155">Created Date Time of the device</span></span>|
|<span data-ttu-id="964e5-156">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="964e5-156">lastContactedDateTime</span></span>|<span data-ttu-id="964e5-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="964e5-157">DateTimeOffset</span></span>|<span data-ttu-id="964e5-158">デバイスの最終連絡日時</span><span class="sxs-lookup"><span data-stu-id="964e5-158">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="964e5-159">description</span><span class="sxs-lookup"><span data-stu-id="964e5-159">description</span></span>|<span data-ttu-id="964e5-160">String</span><span class="sxs-lookup"><span data-stu-id="964e5-160">String</span></span>|<span data-ttu-id="964e5-161">デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="964e5-161">The description of the device</span></span>|
|<span data-ttu-id="964e5-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="964e5-162">enrollmentState</span></span>|[<span data-ttu-id="964e5-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="964e5-163">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="964e5-164">Intune でのデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="964e5-164">The state of the device in Intune.</span></span> <span data-ttu-id="964e5-165">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="964e5-165">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="964e5-166">platform</span><span class="sxs-lookup"><span data-stu-id="964e5-166">platform</span></span>|[<span data-ttu-id="964e5-167">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="964e5-167">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="964e5-168">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="964e5-168">The platform of the Device.</span></span> <span data-ttu-id="964e5-169">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="964e5-169">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="964e5-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="964e5-170">Relationships</span></span>
<span data-ttu-id="964e5-171">なし</span><span class="sxs-lookup"><span data-stu-id="964e5-171">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="964e5-172">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="964e5-172">JSON Representation</span></span>
<span data-ttu-id="964e5-173">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="964e5-173">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedAppleDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "String (identifier)",
  "serialNumber": "String",
  "requestedEnrollmentProfileId": "String",
  "requestedEnrollmentProfileAssignmentDateTime": "String (timestamp)",
  "isSupervised": true,
  "discoverySource": "String",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```





