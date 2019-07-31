---
title: deviceEnrollmentLimitConfiguration リソースの種類
description: ユーザーが登録できるデバイスの数を制限するデバイスの登録構成
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f8ec4d7a7b8467c58852863673e7a66ee49dfd9f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967750"
---
# <a name="deviceenrollmentlimitconfiguration-resource-type"></a><span data-ttu-id="88604-103">deviceEnrollmentLimitConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="88604-103">deviceEnrollmentLimitConfiguration resource type</span></span>

> <span data-ttu-id="88604-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88604-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88604-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="88604-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88604-106">ユーザーが登録できるデバイスの数を制限するデバイスの登録構成</span><span class="sxs-lookup"><span data-stu-id="88604-106">Device Enrollment Configuration that restricts the number of devices a user can enroll</span></span>


<span data-ttu-id="88604-107">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="88604-107">Inherits from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="88604-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="88604-108">Methods</span></span>
|<span data-ttu-id="88604-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="88604-109">Method</span></span>|<span data-ttu-id="88604-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="88604-110">Return Type</span></span>|<span data-ttu-id="88604-111">説明</span><span class="sxs-lookup"><span data-stu-id="88604-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="88604-112">List deviceEnrollmentLimitConfigurations</span><span class="sxs-lookup"><span data-stu-id="88604-112">List deviceEnrollmentLimitConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-list.md)|<span data-ttu-id="88604-113">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="88604-113">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) collection</span></span>|<span data-ttu-id="88604-114">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="88604-114">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="88604-115">Get deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="88604-115">Get deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-get.md)|[<span data-ttu-id="88604-116">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="88604-116">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="88604-117">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="88604-117">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|
|[<span data-ttu-id="88604-118">Create deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="88604-118">Create deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-create.md)|[<span data-ttu-id="88604-119">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="88604-119">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="88604-120">新しい [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="88604-120">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|
|[<span data-ttu-id="88604-121">Delete deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="88604-121">Delete deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-delete.md)|<span data-ttu-id="88604-122">なし</span><span class="sxs-lookup"><span data-stu-id="88604-122">None</span></span>|<span data-ttu-id="88604-123">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="88604-123">Deletes a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>|
|[<span data-ttu-id="88604-124">Update deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="88604-124">Update deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-update.md)|[<span data-ttu-id="88604-125">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="88604-125">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="88604-126">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="88604-126">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="88604-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88604-127">Properties</span></span>
|<span data-ttu-id="88604-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88604-128">Property</span></span>|<span data-ttu-id="88604-129">型</span><span class="sxs-lookup"><span data-stu-id="88604-129">Type</span></span>|<span data-ttu-id="88604-130">説明</span><span class="sxs-lookup"><span data-stu-id="88604-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88604-131">id</span><span class="sxs-lookup"><span data-stu-id="88604-131">id</span></span>|<span data-ttu-id="88604-132">文字列</span><span class="sxs-lookup"><span data-stu-id="88604-132">String</span></span>|<span data-ttu-id="88604-133">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたアカウントの一意識別子</span><span class="sxs-lookup"><span data-stu-id="88604-133">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="88604-134">displayName</span><span class="sxs-lookup"><span data-stu-id="88604-134">displayName</span></span>|<span data-ttu-id="88604-135">String</span><span class="sxs-lookup"><span data-stu-id="88604-135">String</span></span>|<span data-ttu-id="88604-136">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の表示名。</span><span class="sxs-lookup"><span data-stu-id="88604-136">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="88604-137">description</span><span class="sxs-lookup"><span data-stu-id="88604-137">description</span></span>|<span data-ttu-id="88604-138">String</span><span class="sxs-lookup"><span data-stu-id="88604-138">String</span></span>|<span data-ttu-id="88604-139">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の説明</span><span class="sxs-lookup"><span data-stu-id="88604-139">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="88604-140">priority</span><span class="sxs-lookup"><span data-stu-id="88604-140">priority</span></span>|<span data-ttu-id="88604-141">Int32</span><span class="sxs-lookup"><span data-stu-id="88604-141">Int32</span></span>|<span data-ttu-id="88604-142">優先度は、登録構成が割り当てられている複数のグループにユーザーが存在するときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="88604-142">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="88604-143">ユーザーは、優先度の低い値を持つ構成のみに適用されます。</span><span class="sxs-lookup"><span data-stu-id="88604-143">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="88604-144">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="88604-144">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="88604-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88604-145">createdDateTime</span></span>|<span data-ttu-id="88604-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88604-146">DateTimeOffset</span></span>|<span data-ttu-id="88604-147">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された、デバイス登録構成の日時を UTC として作成した日時</span><span class="sxs-lookup"><span data-stu-id="88604-147">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="88604-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88604-148">lastModifiedDateTime</span></span>|<span data-ttu-id="88604-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88604-149">DateTimeOffset</span></span>|<span data-ttu-id="88604-150">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の最終変更日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="88604-150">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="88604-151">version</span><span class="sxs-lookup"><span data-stu-id="88604-151">version</span></span>|<span data-ttu-id="88604-152">Int32</span><span class="sxs-lookup"><span data-stu-id="88604-152">Int32</span></span>|<span data-ttu-id="88604-153">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成のバージョン</span><span class="sxs-lookup"><span data-stu-id="88604-153">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="88604-154">limit</span><span class="sxs-lookup"><span data-stu-id="88604-154">limit</span></span>|<span data-ttu-id="88604-155">Int32</span><span class="sxs-lookup"><span data-stu-id="88604-155">Int32</span></span>|<span data-ttu-id="88604-156">ユーザーが登録できるデバイスの最大数</span><span class="sxs-lookup"><span data-stu-id="88604-156">The maximum number of devices that a user can enroll</span></span>|

## <a name="relationships"></a><span data-ttu-id="88604-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="88604-157">Relationships</span></span>
|<span data-ttu-id="88604-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="88604-158">Relationship</span></span>|<span data-ttu-id="88604-159">型</span><span class="sxs-lookup"><span data-stu-id="88604-159">Type</span></span>|<span data-ttu-id="88604-160">説明</span><span class="sxs-lookup"><span data-stu-id="88604-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88604-161">assignments</span><span class="sxs-lookup"><span data-stu-id="88604-161">assignments</span></span>|<span data-ttu-id="88604-162">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="88604-162">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="88604-163">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス構成プロファイルのグループ割り当ての一覧</span><span class="sxs-lookup"><span data-stu-id="88604-163">The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88604-164">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="88604-164">JSON Representation</span></span>
<span data-ttu-id="88604-165">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="88604-165">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentLimitConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "limit": 1024
}
```





