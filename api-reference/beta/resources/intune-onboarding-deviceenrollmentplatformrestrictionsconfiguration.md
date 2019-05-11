---
title: deviceEnrollmentPlatformRestrictionsConfiguration リソースの種類
description: ユーザーが登録できるデバイスの種類を制限するデバイスの登録構成
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 009d43eeab219cc482dd1258c1e33426dec81cb1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940450"
---
# <a name="deviceenrollmentplatformrestrictionsconfiguration-resource-type"></a><span data-ttu-id="bb253-103">deviceEnrollmentPlatformRestrictionsConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bb253-103">deviceEnrollmentPlatformRestrictionsConfiguration resource type</span></span>

> <span data-ttu-id="bb253-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb253-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb253-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb253-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb253-106">ユーザーが登録できるデバイスの種類を制限するデバイスの登録構成</span><span class="sxs-lookup"><span data-stu-id="bb253-106">Device Enrollment Configuration that restricts the types of devices a user can enroll</span></span>


<span data-ttu-id="bb253-107">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bb253-107">Inherits from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="bb253-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="bb253-108">Methods</span></span>
|<span data-ttu-id="bb253-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="bb253-109">Method</span></span>|<span data-ttu-id="bb253-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bb253-110">Return Type</span></span>|<span data-ttu-id="bb253-111">説明</span><span class="sxs-lookup"><span data-stu-id="bb253-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bb253-112">List deviceEnrollmentPlatformRestrictionsConfigurations</span><span class="sxs-lookup"><span data-stu-id="bb253-112">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-list.md)|<span data-ttu-id="bb253-113">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bb253-113">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) collection</span></span>|<span data-ttu-id="bb253-114">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="bb253-114">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="bb253-115">Get deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="bb253-115">Get deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-get.md)|[<span data-ttu-id="bb253-116">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="bb253-116">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="bb253-117">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bb253-117">Read properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|
|[<span data-ttu-id="bb253-118">Create deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="bb253-118">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-create.md)|[<span data-ttu-id="bb253-119">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="bb253-119">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="bb253-120">新しい [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bb253-120">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|
|[<span data-ttu-id="bb253-121">Delete deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="bb253-121">Delete deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-delete.md)|<span data-ttu-id="bb253-122">なし</span><span class="sxs-lookup"><span data-stu-id="bb253-122">None</span></span>|<span data-ttu-id="bb253-123">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="bb253-123">Deletes a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>|
|[<span data-ttu-id="bb253-124">Update deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="bb253-124">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-update.md)|[<span data-ttu-id="bb253-125">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="bb253-125">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="bb253-126">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bb253-126">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bb253-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb253-127">Properties</span></span>
|<span data-ttu-id="bb253-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb253-128">Property</span></span>|<span data-ttu-id="bb253-129">種類</span><span class="sxs-lookup"><span data-stu-id="bb253-129">Type</span></span>|<span data-ttu-id="bb253-130">説明</span><span class="sxs-lookup"><span data-stu-id="bb253-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb253-131">id</span><span class="sxs-lookup"><span data-stu-id="bb253-131">id</span></span>|<span data-ttu-id="bb253-132">文字列</span><span class="sxs-lookup"><span data-stu-id="bb253-132">String</span></span>|<span data-ttu-id="bb253-133">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたアカウントの一意識別子</span><span class="sxs-lookup"><span data-stu-id="bb253-133">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="bb253-134">displayName</span><span class="sxs-lookup"><span data-stu-id="bb253-134">displayName</span></span>|<span data-ttu-id="bb253-135">String</span><span class="sxs-lookup"><span data-stu-id="bb253-135">String</span></span>|<span data-ttu-id="bb253-136">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の表示名。</span><span class="sxs-lookup"><span data-stu-id="bb253-136">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="bb253-137">description</span><span class="sxs-lookup"><span data-stu-id="bb253-137">description</span></span>|<span data-ttu-id="bb253-138">String</span><span class="sxs-lookup"><span data-stu-id="bb253-138">String</span></span>|<span data-ttu-id="bb253-139">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の説明</span><span class="sxs-lookup"><span data-stu-id="bb253-139">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="bb253-140">priority</span><span class="sxs-lookup"><span data-stu-id="bb253-140">priority</span></span>|<span data-ttu-id="bb253-141">Int32</span><span class="sxs-lookup"><span data-stu-id="bb253-141">Int32</span></span>|<span data-ttu-id="bb253-142">優先度は、登録構成が割り当てられている複数のグループにユーザーが存在するときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="bb253-142">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="bb253-143">ユーザーは、優先度の低い値を持つ構成のみに適用されます。</span><span class="sxs-lookup"><span data-stu-id="bb253-143">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="bb253-144">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bb253-144">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="bb253-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb253-145">createdDateTime</span></span>|<span data-ttu-id="bb253-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb253-146">DateTimeOffset</span></span>|<span data-ttu-id="bb253-147">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された、デバイス登録構成の日時を UTC として作成した日時</span><span class="sxs-lookup"><span data-stu-id="bb253-147">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="bb253-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb253-148">lastModifiedDateTime</span></span>|<span data-ttu-id="bb253-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb253-149">DateTimeOffset</span></span>|<span data-ttu-id="bb253-150">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の最終変更日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="bb253-150">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="bb253-151">version</span><span class="sxs-lookup"><span data-stu-id="bb253-151">version</span></span>|<span data-ttu-id="bb253-152">Int32</span><span class="sxs-lookup"><span data-stu-id="bb253-152">Int32</span></span>|<span data-ttu-id="bb253-153">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成のバージョン</span><span class="sxs-lookup"><span data-stu-id="bb253-153">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="bb253-154">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="bb253-154">iosRestriction</span></span>|[<span data-ttu-id="bb253-155">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="bb253-155">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="bb253-156">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Ios の制限</span><span class="sxs-lookup"><span data-stu-id="bb253-156">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="bb253-157">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="bb253-157">windowsRestriction</span></span>|[<span data-ttu-id="bb253-158">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="bb253-158">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="bb253-159">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Windows の制限</span><span class="sxs-lookup"><span data-stu-id="bb253-159">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="bb253-160">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="bb253-160">windowsMobileRestriction</span></span>|[<span data-ttu-id="bb253-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="bb253-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="bb253-162">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Windows mobile の制限</span><span class="sxs-lookup"><span data-stu-id="bb253-162">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="bb253-163">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="bb253-163">androidRestriction</span></span>|[<span data-ttu-id="bb253-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="bb253-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="bb253-165">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Android の制限</span><span class="sxs-lookup"><span data-stu-id="bb253-165">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="bb253-166">Androidforwork 制限</span><span class="sxs-lookup"><span data-stu-id="bb253-166">androidForWorkRestriction</span></span>|[<span data-ttu-id="bb253-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="bb253-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="bb253-168">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づいた、Android for work 制限</span><span class="sxs-lookup"><span data-stu-id="bb253-168">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="bb253-169">macRestriction</span><span class="sxs-lookup"><span data-stu-id="bb253-169">macRestriction</span></span>|[<span data-ttu-id="bb253-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="bb253-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="bb253-171">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Mac 制限</span><span class="sxs-lookup"><span data-stu-id="bb253-171">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="bb253-172">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="bb253-172">macOSRestriction</span></span>|[<span data-ttu-id="bb253-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="bb253-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="bb253-174">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Mac 制限</span><span class="sxs-lookup"><span data-stu-id="bb253-174">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb253-175">関係</span><span class="sxs-lookup"><span data-stu-id="bb253-175">Relationships</span></span>
|<span data-ttu-id="bb253-176">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bb253-176">Relationship</span></span>|<span data-ttu-id="bb253-177">型</span><span class="sxs-lookup"><span data-stu-id="bb253-177">Type</span></span>|<span data-ttu-id="bb253-178">説明</span><span class="sxs-lookup"><span data-stu-id="bb253-178">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb253-179">assignments</span><span class="sxs-lookup"><span data-stu-id="bb253-179">assignments</span></span>|<span data-ttu-id="bb253-180">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bb253-180">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="bb253-181">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス構成プロファイルのグループ割り当ての一覧</span><span class="sxs-lookup"><span data-stu-id="bb253-181">The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb253-182">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bb253-182">JSON Representation</span></span>
<span data-ttu-id="bb253-183">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bb253-183">Here is a JSON representation of the resource.</span></span>
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




