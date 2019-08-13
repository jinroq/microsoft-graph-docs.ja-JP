---
title: deviceEnrollmentLimitConfiguration リソースの種類
description: ユーザーが登録できるデバイスの数を制限するデバイスの登録構成
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f4b77ecaeeb23182be2fe867c73675a294528048
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374352"
---
# <a name="deviceenrollmentlimitconfiguration-resource-type"></a><span data-ttu-id="771c0-103">deviceEnrollmentLimitConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="771c0-103">deviceEnrollmentLimitConfiguration resource type</span></span>

> <span data-ttu-id="771c0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="771c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="771c0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="771c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="771c0-106">ユーザーが登録できるデバイスの数を制限するデバイスの登録構成</span><span class="sxs-lookup"><span data-stu-id="771c0-106">Device Enrollment Configuration that restricts the number of devices a user can enroll</span></span>


<span data-ttu-id="771c0-107">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="771c0-107">Inherits from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="771c0-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="771c0-108">Methods</span></span>
|<span data-ttu-id="771c0-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="771c0-109">Method</span></span>|<span data-ttu-id="771c0-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="771c0-110">Return Type</span></span>|<span data-ttu-id="771c0-111">説明</span><span class="sxs-lookup"><span data-stu-id="771c0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="771c0-112">List deviceEnrollmentLimitConfigurations</span><span class="sxs-lookup"><span data-stu-id="771c0-112">List deviceEnrollmentLimitConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-list.md)|<span data-ttu-id="771c0-113">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="771c0-113">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) collection</span></span>|<span data-ttu-id="771c0-114">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="771c0-114">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="771c0-115">Get deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="771c0-115">Get deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-get.md)|[<span data-ttu-id="771c0-116">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="771c0-116">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="771c0-117">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="771c0-117">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|
|[<span data-ttu-id="771c0-118">Create deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="771c0-118">Create deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-create.md)|[<span data-ttu-id="771c0-119">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="771c0-119">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="771c0-120">新しい [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="771c0-120">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|
|[<span data-ttu-id="771c0-121">Delete deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="771c0-121">Delete deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-delete.md)|<span data-ttu-id="771c0-122">なし</span><span class="sxs-lookup"><span data-stu-id="771c0-122">None</span></span>|<span data-ttu-id="771c0-123">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="771c0-123">Deletes a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>|
|[<span data-ttu-id="771c0-124">Update deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="771c0-124">Update deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-update.md)|[<span data-ttu-id="771c0-125">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="771c0-125">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="771c0-126">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="771c0-126">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="771c0-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="771c0-127">Properties</span></span>
|<span data-ttu-id="771c0-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="771c0-128">Property</span></span>|<span data-ttu-id="771c0-129">型</span><span class="sxs-lookup"><span data-stu-id="771c0-129">Type</span></span>|<span data-ttu-id="771c0-130">説明</span><span class="sxs-lookup"><span data-stu-id="771c0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="771c0-131">id</span><span class="sxs-lookup"><span data-stu-id="771c0-131">id</span></span>|<span data-ttu-id="771c0-132">文字列</span><span class="sxs-lookup"><span data-stu-id="771c0-132">String</span></span>|<span data-ttu-id="771c0-133">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたアカウントの一意識別子</span><span class="sxs-lookup"><span data-stu-id="771c0-133">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="771c0-134">displayName</span><span class="sxs-lookup"><span data-stu-id="771c0-134">displayName</span></span>|<span data-ttu-id="771c0-135">String</span><span class="sxs-lookup"><span data-stu-id="771c0-135">String</span></span>|<span data-ttu-id="771c0-136">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の表示名。</span><span class="sxs-lookup"><span data-stu-id="771c0-136">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="771c0-137">description</span><span class="sxs-lookup"><span data-stu-id="771c0-137">description</span></span>|<span data-ttu-id="771c0-138">String</span><span class="sxs-lookup"><span data-stu-id="771c0-138">String</span></span>|<span data-ttu-id="771c0-139">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の説明</span><span class="sxs-lookup"><span data-stu-id="771c0-139">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="771c0-140">priority</span><span class="sxs-lookup"><span data-stu-id="771c0-140">priority</span></span>|<span data-ttu-id="771c0-141">Int32</span><span class="sxs-lookup"><span data-stu-id="771c0-141">Int32</span></span>|<span data-ttu-id="771c0-142">優先度は、登録構成が割り当てられている複数のグループにユーザーが存在するときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="771c0-142">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="771c0-143">ユーザーは、優先度の低い値を持つ構成のみに適用されます。</span><span class="sxs-lookup"><span data-stu-id="771c0-143">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="771c0-144">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="771c0-144">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="771c0-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="771c0-145">createdDateTime</span></span>|<span data-ttu-id="771c0-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="771c0-146">DateTimeOffset</span></span>|<span data-ttu-id="771c0-147">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された、デバイス登録構成の日時を UTC として作成した日時</span><span class="sxs-lookup"><span data-stu-id="771c0-147">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="771c0-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="771c0-148">lastModifiedDateTime</span></span>|<span data-ttu-id="771c0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="771c0-149">DateTimeOffset</span></span>|<span data-ttu-id="771c0-150">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の最終変更日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="771c0-150">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="771c0-151">version</span><span class="sxs-lookup"><span data-stu-id="771c0-151">version</span></span>|<span data-ttu-id="771c0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="771c0-152">Int32</span></span>|<span data-ttu-id="771c0-153">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成のバージョン</span><span class="sxs-lookup"><span data-stu-id="771c0-153">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="771c0-154">limit</span><span class="sxs-lookup"><span data-stu-id="771c0-154">limit</span></span>|<span data-ttu-id="771c0-155">Int32</span><span class="sxs-lookup"><span data-stu-id="771c0-155">Int32</span></span>|<span data-ttu-id="771c0-156">ユーザーが登録できるデバイスの最大数</span><span class="sxs-lookup"><span data-stu-id="771c0-156">The maximum number of devices that a user can enroll</span></span>|

## <a name="relationships"></a><span data-ttu-id="771c0-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="771c0-157">Relationships</span></span>
|<span data-ttu-id="771c0-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="771c0-158">Relationship</span></span>|<span data-ttu-id="771c0-159">型</span><span class="sxs-lookup"><span data-stu-id="771c0-159">Type</span></span>|<span data-ttu-id="771c0-160">説明</span><span class="sxs-lookup"><span data-stu-id="771c0-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="771c0-161">assignments</span><span class="sxs-lookup"><span data-stu-id="771c0-161">assignments</span></span>|<span data-ttu-id="771c0-162">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="771c0-162">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="771c0-163">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス構成プロファイルのグループ割り当ての一覧</span><span class="sxs-lookup"><span data-stu-id="771c0-163">The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="771c0-164">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="771c0-164">JSON Representation</span></span>
<span data-ttu-id="771c0-165">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="771c0-165">Here is a JSON representation of the resource.</span></span>
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



