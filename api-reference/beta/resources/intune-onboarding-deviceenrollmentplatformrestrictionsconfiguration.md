---
title: deviceEnrollmentPlatformRestrictionsConfiguration リソースの種類
description: ユーザーが登録できるデバイスの種類を制限するデバイスの登録構成
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4f4dc3eb25efe1fe14bd1b12bea2f196f92ccea
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993131"
---
# <a name="deviceenrollmentplatformrestrictionsconfiguration-resource-type"></a><span data-ttu-id="a8564-103">deviceEnrollmentPlatformRestrictionsConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a8564-103">deviceEnrollmentPlatformRestrictionsConfiguration resource type</span></span>

> <span data-ttu-id="a8564-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8564-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8564-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a8564-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8564-106">ユーザーが登録できるデバイスの種類を制限するデバイスの登録構成</span><span class="sxs-lookup"><span data-stu-id="a8564-106">Device Enrollment Configuration that restricts the types of devices a user can enroll</span></span>


<span data-ttu-id="a8564-107">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a8564-107">Inherits from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a8564-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a8564-108">Methods</span></span>
|<span data-ttu-id="a8564-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="a8564-109">Method</span></span>|<span data-ttu-id="a8564-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a8564-110">Return Type</span></span>|<span data-ttu-id="a8564-111">説明</span><span class="sxs-lookup"><span data-stu-id="a8564-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a8564-112">List deviceEnrollmentPlatformRestrictionsConfigurations</span><span class="sxs-lookup"><span data-stu-id="a8564-112">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-list.md)|<span data-ttu-id="a8564-113">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a8564-113">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) collection</span></span>|<span data-ttu-id="a8564-114">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a8564-114">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="a8564-115">Get deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8564-115">Get deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-get.md)|[<span data-ttu-id="a8564-116">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8564-116">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="a8564-117">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a8564-117">Read properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|
|[<span data-ttu-id="a8564-118">Create deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8564-118">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-create.md)|[<span data-ttu-id="a8564-119">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8564-119">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="a8564-120">新しい [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a8564-120">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|
|[<span data-ttu-id="a8564-121">Delete deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8564-121">Delete deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-delete.md)|<span data-ttu-id="a8564-122">なし</span><span class="sxs-lookup"><span data-stu-id="a8564-122">None</span></span>|<span data-ttu-id="a8564-123">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="a8564-123">Deletes a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>|
|[<span data-ttu-id="a8564-124">Update deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8564-124">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-update.md)|[<span data-ttu-id="a8564-125">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8564-125">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="a8564-126">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a8564-126">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a8564-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8564-127">Properties</span></span>
|<span data-ttu-id="a8564-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8564-128">Property</span></span>|<span data-ttu-id="a8564-129">型</span><span class="sxs-lookup"><span data-stu-id="a8564-129">Type</span></span>|<span data-ttu-id="a8564-130">説明</span><span class="sxs-lookup"><span data-stu-id="a8564-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8564-131">id</span><span class="sxs-lookup"><span data-stu-id="a8564-131">id</span></span>|<span data-ttu-id="a8564-132">文字列</span><span class="sxs-lookup"><span data-stu-id="a8564-132">String</span></span>|<span data-ttu-id="a8564-133">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたアカウントの一意識別子</span><span class="sxs-lookup"><span data-stu-id="a8564-133">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a8564-134">displayName</span><span class="sxs-lookup"><span data-stu-id="a8564-134">displayName</span></span>|<span data-ttu-id="a8564-135">String</span><span class="sxs-lookup"><span data-stu-id="a8564-135">String</span></span>|<span data-ttu-id="a8564-136">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の表示名。</span><span class="sxs-lookup"><span data-stu-id="a8564-136">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a8564-137">description</span><span class="sxs-lookup"><span data-stu-id="a8564-137">description</span></span>|<span data-ttu-id="a8564-138">String</span><span class="sxs-lookup"><span data-stu-id="a8564-138">String</span></span>|<span data-ttu-id="a8564-139">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の説明</span><span class="sxs-lookup"><span data-stu-id="a8564-139">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a8564-140">priority</span><span class="sxs-lookup"><span data-stu-id="a8564-140">priority</span></span>|<span data-ttu-id="a8564-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a8564-141">Int32</span></span>|<span data-ttu-id="a8564-142">優先度は、登録構成が割り当てられている複数のグループにユーザーが存在するときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="a8564-142">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="a8564-143">ユーザーは、優先度の低い値を持つ構成のみに適用されます。</span><span class="sxs-lookup"><span data-stu-id="a8564-143">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="a8564-144">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a8564-144">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a8564-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8564-145">createdDateTime</span></span>|<span data-ttu-id="a8564-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8564-146">DateTimeOffset</span></span>|<span data-ttu-id="a8564-147">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された、デバイス登録構成の日時を UTC として作成した日時</span><span class="sxs-lookup"><span data-stu-id="a8564-147">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a8564-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8564-148">lastModifiedDateTime</span></span>|<span data-ttu-id="a8564-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8564-149">DateTimeOffset</span></span>|<span data-ttu-id="a8564-150">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の最終変更日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="a8564-150">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a8564-151">version</span><span class="sxs-lookup"><span data-stu-id="a8564-151">version</span></span>|<span data-ttu-id="a8564-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a8564-152">Int32</span></span>|<span data-ttu-id="a8564-153">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成のバージョン</span><span class="sxs-lookup"><span data-stu-id="a8564-153">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a8564-154">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="a8564-154">iosRestriction</span></span>|[<span data-ttu-id="a8564-155">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a8564-155">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a8564-156">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Ios の制限</span><span class="sxs-lookup"><span data-stu-id="a8564-156">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="a8564-157">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="a8564-157">windowsRestriction</span></span>|[<span data-ttu-id="a8564-158">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a8564-158">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a8564-159">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Windows の制限</span><span class="sxs-lookup"><span data-stu-id="a8564-159">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="a8564-160">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="a8564-160">windowsMobileRestriction</span></span>|[<span data-ttu-id="a8564-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a8564-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a8564-162">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Windows mobile の制限</span><span class="sxs-lookup"><span data-stu-id="a8564-162">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="a8564-163">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="a8564-163">androidRestriction</span></span>|[<span data-ttu-id="a8564-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a8564-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a8564-165">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Android の制限</span><span class="sxs-lookup"><span data-stu-id="a8564-165">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="a8564-166">Androidforwork 制限</span><span class="sxs-lookup"><span data-stu-id="a8564-166">androidForWorkRestriction</span></span>|[<span data-ttu-id="a8564-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a8564-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a8564-168">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づいた、Android for work 制限</span><span class="sxs-lookup"><span data-stu-id="a8564-168">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="a8564-169">macRestriction</span><span class="sxs-lookup"><span data-stu-id="a8564-169">macRestriction</span></span>|[<span data-ttu-id="a8564-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a8564-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a8564-171">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Mac 制限</span><span class="sxs-lookup"><span data-stu-id="a8564-171">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="a8564-172">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="a8564-172">macOSRestriction</span></span>|[<span data-ttu-id="a8564-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a8564-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a8564-174">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Mac 制限</span><span class="sxs-lookup"><span data-stu-id="a8564-174">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8564-175">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a8564-175">Relationships</span></span>
|<span data-ttu-id="a8564-176">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a8564-176">Relationship</span></span>|<span data-ttu-id="a8564-177">型</span><span class="sxs-lookup"><span data-stu-id="a8564-177">Type</span></span>|<span data-ttu-id="a8564-178">説明</span><span class="sxs-lookup"><span data-stu-id="a8564-178">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8564-179">assignments</span><span class="sxs-lookup"><span data-stu-id="a8564-179">assignments</span></span>|<span data-ttu-id="a8564-180">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a8564-180">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a8564-181">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス構成プロファイルのグループ割り当ての一覧</span><span class="sxs-lookup"><span data-stu-id="a8564-181">The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8564-182">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a8564-182">JSON Representation</span></span>
<span data-ttu-id="a8564-183">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a8564-183">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "macRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  }
}
```





