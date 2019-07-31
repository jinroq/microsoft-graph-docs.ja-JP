---
title: deviceEnrollmentPlatformRestrictionsConfiguration リソースの種類
description: ユーザーが登録できるデバイスの種類を制限するデバイスの登録構成
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e3eecac7134d76007a4c23d219c5a4dee5780121
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998185"
---
# <a name="deviceenrollmentplatformrestrictionsconfiguration-resource-type"></a><span data-ttu-id="71b42-103">deviceEnrollmentPlatformRestrictionsConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="71b42-103">deviceEnrollmentPlatformRestrictionsConfiguration resource type</span></span>

> <span data-ttu-id="71b42-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71b42-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71b42-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="71b42-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71b42-106">ユーザーが登録できるデバイスの種類を制限するデバイスの登録構成</span><span class="sxs-lookup"><span data-stu-id="71b42-106">Device Enrollment Configuration that restricts the types of devices a user can enroll</span></span>


<span data-ttu-id="71b42-107">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="71b42-107">Inherits from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="71b42-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="71b42-108">Methods</span></span>
|<span data-ttu-id="71b42-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="71b42-109">Method</span></span>|<span data-ttu-id="71b42-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="71b42-110">Return Type</span></span>|<span data-ttu-id="71b42-111">説明</span><span class="sxs-lookup"><span data-stu-id="71b42-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="71b42-112">List deviceEnrollmentPlatformRestrictionsConfigurations</span><span class="sxs-lookup"><span data-stu-id="71b42-112">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-list.md)|<span data-ttu-id="71b42-113">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="71b42-113">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) collection</span></span>|<span data-ttu-id="71b42-114">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="71b42-114">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="71b42-115">Get deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="71b42-115">Get deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-get.md)|[<span data-ttu-id="71b42-116">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="71b42-116">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="71b42-117">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="71b42-117">Read properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|
|[<span data-ttu-id="71b42-118">Create deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="71b42-118">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-create.md)|[<span data-ttu-id="71b42-119">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="71b42-119">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="71b42-120">新しい [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="71b42-120">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|
|[<span data-ttu-id="71b42-121">Delete deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="71b42-121">Delete deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-delete.md)|<span data-ttu-id="71b42-122">なし</span><span class="sxs-lookup"><span data-stu-id="71b42-122">None</span></span>|<span data-ttu-id="71b42-123">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="71b42-123">Deletes a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>|
|[<span data-ttu-id="71b42-124">Update deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="71b42-124">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-update.md)|[<span data-ttu-id="71b42-125">deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="71b42-125">deviceEnrollmentPlatformRestrictionsConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|<span data-ttu-id="71b42-126">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="71b42-126">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="71b42-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71b42-127">Properties</span></span>
|<span data-ttu-id="71b42-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71b42-128">Property</span></span>|<span data-ttu-id="71b42-129">型</span><span class="sxs-lookup"><span data-stu-id="71b42-129">Type</span></span>|<span data-ttu-id="71b42-130">説明</span><span class="sxs-lookup"><span data-stu-id="71b42-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71b42-131">id</span><span class="sxs-lookup"><span data-stu-id="71b42-131">id</span></span>|<span data-ttu-id="71b42-132">文字列</span><span class="sxs-lookup"><span data-stu-id="71b42-132">String</span></span>|<span data-ttu-id="71b42-133">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたアカウントの一意識別子</span><span class="sxs-lookup"><span data-stu-id="71b42-133">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="71b42-134">displayName</span><span class="sxs-lookup"><span data-stu-id="71b42-134">displayName</span></span>|<span data-ttu-id="71b42-135">String</span><span class="sxs-lookup"><span data-stu-id="71b42-135">String</span></span>|<span data-ttu-id="71b42-136">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の表示名。</span><span class="sxs-lookup"><span data-stu-id="71b42-136">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="71b42-137">description</span><span class="sxs-lookup"><span data-stu-id="71b42-137">description</span></span>|<span data-ttu-id="71b42-138">String</span><span class="sxs-lookup"><span data-stu-id="71b42-138">String</span></span>|<span data-ttu-id="71b42-139">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の説明</span><span class="sxs-lookup"><span data-stu-id="71b42-139">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="71b42-140">priority</span><span class="sxs-lookup"><span data-stu-id="71b42-140">priority</span></span>|<span data-ttu-id="71b42-141">Int32</span><span class="sxs-lookup"><span data-stu-id="71b42-141">Int32</span></span>|<span data-ttu-id="71b42-142">優先度は、登録構成が割り当てられている複数のグループにユーザーが存在するときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="71b42-142">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="71b42-143">ユーザーは、優先度の低い値を持つ構成のみに適用されます。</span><span class="sxs-lookup"><span data-stu-id="71b42-143">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="71b42-144">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="71b42-144">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="71b42-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71b42-145">createdDateTime</span></span>|<span data-ttu-id="71b42-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71b42-146">DateTimeOffset</span></span>|<span data-ttu-id="71b42-147">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された、デバイス登録構成の日時を UTC として作成した日時</span><span class="sxs-lookup"><span data-stu-id="71b42-147">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="71b42-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71b42-148">lastModifiedDateTime</span></span>|<span data-ttu-id="71b42-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71b42-149">DateTimeOffset</span></span>|<span data-ttu-id="71b42-150">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の最終変更日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="71b42-150">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="71b42-151">version</span><span class="sxs-lookup"><span data-stu-id="71b42-151">version</span></span>|<span data-ttu-id="71b42-152">Int32</span><span class="sxs-lookup"><span data-stu-id="71b42-152">Int32</span></span>|<span data-ttu-id="71b42-153">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成のバージョン</span><span class="sxs-lookup"><span data-stu-id="71b42-153">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="71b42-154">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="71b42-154">iosRestriction</span></span>|[<span data-ttu-id="71b42-155">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="71b42-155">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="71b42-156">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Ios の制限</span><span class="sxs-lookup"><span data-stu-id="71b42-156">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="71b42-157">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="71b42-157">windowsRestriction</span></span>|[<span data-ttu-id="71b42-158">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="71b42-158">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="71b42-159">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Windows の制限</span><span class="sxs-lookup"><span data-stu-id="71b42-159">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="71b42-160">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="71b42-160">windowsMobileRestriction</span></span>|[<span data-ttu-id="71b42-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="71b42-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="71b42-162">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Windows mobile の制限</span><span class="sxs-lookup"><span data-stu-id="71b42-162">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="71b42-163">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="71b42-163">androidRestriction</span></span>|[<span data-ttu-id="71b42-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="71b42-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="71b42-165">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Android の制限</span><span class="sxs-lookup"><span data-stu-id="71b42-165">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="71b42-166">Androidforwork 制限</span><span class="sxs-lookup"><span data-stu-id="71b42-166">androidForWorkRestriction</span></span>|[<span data-ttu-id="71b42-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="71b42-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="71b42-168">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づいた、Android for work 制限</span><span class="sxs-lookup"><span data-stu-id="71b42-168">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="71b42-169">macRestriction</span><span class="sxs-lookup"><span data-stu-id="71b42-169">macRestriction</span></span>|[<span data-ttu-id="71b42-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="71b42-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="71b42-171">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Mac 制限</span><span class="sxs-lookup"><span data-stu-id="71b42-171">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="71b42-172">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="71b42-172">macOSRestriction</span></span>|[<span data-ttu-id="71b42-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="71b42-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="71b42-174">プラットフォーム、プラットフォームオペレーティングシステムのバージョン、およびデバイスの所有権に基づく Mac 制限</span><span class="sxs-lookup"><span data-stu-id="71b42-174">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|

## <a name="relationships"></a><span data-ttu-id="71b42-175">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="71b42-175">Relationships</span></span>
|<span data-ttu-id="71b42-176">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="71b42-176">Relationship</span></span>|<span data-ttu-id="71b42-177">型</span><span class="sxs-lookup"><span data-stu-id="71b42-177">Type</span></span>|<span data-ttu-id="71b42-178">説明</span><span class="sxs-lookup"><span data-stu-id="71b42-178">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71b42-179">assignments</span><span class="sxs-lookup"><span data-stu-id="71b42-179">assignments</span></span>|<span data-ttu-id="71b42-180">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="71b42-180">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="71b42-181">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス構成プロファイルのグループ割り当ての一覧</span><span class="sxs-lookup"><span data-stu-id="71b42-181">The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71b42-182">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="71b42-182">JSON Representation</span></span>
<span data-ttu-id="71b42-183">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="71b42-183">Here is a JSON representation of the resource.</span></span>
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





