---
title: importedAppleDeviceIdentity リソースの種類
description: ImportedAppleDeviceIdentity リソースは、Apple デバイスのインポートされたデバイス id を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b93929dd02b5ee1f472a89733d2dc6246cad4411
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992648"
---
# <a name="importedappledeviceidentity-resource-type"></a><span data-ttu-id="aad56-103">importedAppleDeviceIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aad56-103">importedAppleDeviceIdentity resource type</span></span>

> <span data-ttu-id="aad56-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aad56-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aad56-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aad56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aad56-106">ImportedAppleDeviceIdentity リソースは、Apple デバイスのインポートされたデバイス id を表します。</span><span class="sxs-lookup"><span data-stu-id="aad56-106">The importedAppleDeviceIdentity resource represents the imported device identity of an Apple device .</span></span>

## <a name="methods"></a><span data-ttu-id="aad56-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="aad56-107">Methods</span></span>
|<span data-ttu-id="aad56-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="aad56-108">Method</span></span>|<span data-ttu-id="aad56-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="aad56-109">Return Type</span></span>|<span data-ttu-id="aad56-110">説明</span><span class="sxs-lookup"><span data-stu-id="aad56-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aad56-111">リスト importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="aad56-111">List importedAppleDeviceIdentities</span></span>](../api/intune-enrollment-importedappledeviceidentity-list.md)|<span data-ttu-id="aad56-112">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="aad56-112">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="aad56-113">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="aad56-113">List properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="aad56-114">ImportedAppleDeviceIdentity を取得する</span><span class="sxs-lookup"><span data-stu-id="aad56-114">Get importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-get.md)|[<span data-ttu-id="aad56-115">importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="aad56-115">importedAppleDeviceIdentity</span></span>](../resources/intune-enrollment-importedappledeviceidentity.md)|<span data-ttu-id="aad56-116">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="aad56-116">Read properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="aad56-117">ImportedAppleDeviceIdentity を作成する</span><span class="sxs-lookup"><span data-stu-id="aad56-117">Create importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-create.md)|[<span data-ttu-id="aad56-118">importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="aad56-118">importedAppleDeviceIdentity</span></span>](../resources/intune-enrollment-importedappledeviceidentity.md)|<span data-ttu-id="aad56-119">新しい[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="aad56-119">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="aad56-120">ImportedAppleDeviceIdentity の削除</span><span class="sxs-lookup"><span data-stu-id="aad56-120">Delete importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-delete.md)|<span data-ttu-id="aad56-121">None</span><span class="sxs-lookup"><span data-stu-id="aad56-121">None</span></span>|<span data-ttu-id="aad56-122">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="aad56-122">Deletes a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>|
|[<span data-ttu-id="aad56-123">ImportedAppleDeviceIdentity の更新</span><span class="sxs-lookup"><span data-stu-id="aad56-123">Update importedAppleDeviceIdentity</span></span>](../api/intune-enrollment-importedappledeviceidentity-update.md)|[<span data-ttu-id="aad56-124">importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="aad56-124">importedAppleDeviceIdentity</span></span>](../resources/intune-enrollment-importedappledeviceidentity.md)|<span data-ttu-id="aad56-125">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="aad56-125">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="aad56-126">importAppleDeviceIdentityList アクション</span><span class="sxs-lookup"><span data-stu-id="aad56-126">importAppleDeviceIdentityList action</span></span>](../api/intune-enrollment-importedappledeviceidentity-importappledeviceidentitylist.md)|<span data-ttu-id="aad56-127">[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="aad56-127">[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection</span></span>|<span data-ttu-id="aad56-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="aad56-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="aad56-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aad56-129">Properties</span></span>
|<span data-ttu-id="aad56-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aad56-130">Property</span></span>|<span data-ttu-id="aad56-131">型</span><span class="sxs-lookup"><span data-stu-id="aad56-131">Type</span></span>|<span data-ttu-id="aad56-132">説明</span><span class="sxs-lookup"><span data-stu-id="aad56-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aad56-133">id</span><span class="sxs-lookup"><span data-stu-id="aad56-133">id</span></span>|<span data-ttu-id="aad56-134">String</span><span class="sxs-lookup"><span data-stu-id="aad56-134">String</span></span>|<span data-ttu-id="aad56-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="aad56-135">Key of the entity.</span></span>|
|<span data-ttu-id="aad56-136">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="aad56-136">serialNumber</span></span>|<span data-ttu-id="aad56-137">String</span><span class="sxs-lookup"><span data-stu-id="aad56-137">String</span></span>|<span data-ttu-id="aad56-138">デバイスのシリアル番号</span><span class="sxs-lookup"><span data-stu-id="aad56-138">Device serial number</span></span>|
|<span data-ttu-id="aad56-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="aad56-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="aad56-140">String</span><span class="sxs-lookup"><span data-stu-id="aad56-140">String</span></span>|<span data-ttu-id="aad56-141">登録プロファイル Id 管理者が次回の登録時にデバイスに適用する予定</span><span class="sxs-lookup"><span data-stu-id="aad56-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="aad56-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="aad56-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="aad56-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aad56-143">DateTimeOffset</span></span>|<span data-ttu-id="aad56-144">時間登録プロファイルがデバイスに割り当てられている</span><span class="sxs-lookup"><span data-stu-id="aad56-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="aad56-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="aad56-145">isSupervised</span></span>|<span data-ttu-id="aad56-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="aad56-146">Boolean</span></span>|<span data-ttu-id="aad56-147">Apple デバイスが監視されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="aad56-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="aad56-148">詳細情報は次のとおりです。https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="aad56-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="aad56-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="aad56-149">discoverySource</span></span>|[<span data-ttu-id="aad56-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="aad56-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="aad56-151">Apple デバイスの検出ソース。</span><span class="sxs-lookup"><span data-stu-id="aad56-151">Apple device discovery source.</span></span> <span data-ttu-id="aad56-152">可能な値は、`unknown`、`adminImport`、`deviceEnrollmentProgram` です。</span><span class="sxs-lookup"><span data-stu-id="aad56-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="aad56-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aad56-153">createdDateTime</span></span>|<span data-ttu-id="aad56-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aad56-154">DateTimeOffset</span></span>|<span data-ttu-id="aad56-155">デバイスの日時の作成日時</span><span class="sxs-lookup"><span data-stu-id="aad56-155">Created Date Time of the device</span></span>|
|<span data-ttu-id="aad56-156">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="aad56-156">lastContactedDateTime</span></span>|<span data-ttu-id="aad56-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aad56-157">DateTimeOffset</span></span>|<span data-ttu-id="aad56-158">デバイスの最終連絡日時</span><span class="sxs-lookup"><span data-stu-id="aad56-158">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="aad56-159">description</span><span class="sxs-lookup"><span data-stu-id="aad56-159">description</span></span>|<span data-ttu-id="aad56-160">String</span><span class="sxs-lookup"><span data-stu-id="aad56-160">String</span></span>|<span data-ttu-id="aad56-161">デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="aad56-161">The description of the device</span></span>|
|<span data-ttu-id="aad56-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="aad56-162">enrollmentState</span></span>|[<span data-ttu-id="aad56-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="aad56-163">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="aad56-164">Intune でのデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="aad56-164">The state of the device in Intune.</span></span> <span data-ttu-id="aad56-165">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="aad56-165">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="aad56-166">platform</span><span class="sxs-lookup"><span data-stu-id="aad56-166">platform</span></span>|[<span data-ttu-id="aad56-167">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="aad56-167">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="aad56-168">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="aad56-168">The platform of the Device.</span></span> <span data-ttu-id="aad56-169">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="aad56-169">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aad56-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aad56-170">Relationships</span></span>
<span data-ttu-id="aad56-171">なし</span><span class="sxs-lookup"><span data-stu-id="aad56-171">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aad56-172">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aad56-172">JSON Representation</span></span>
<span data-ttu-id="aad56-173">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aad56-173">Here is a JSON representation of the resource.</span></span>
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





