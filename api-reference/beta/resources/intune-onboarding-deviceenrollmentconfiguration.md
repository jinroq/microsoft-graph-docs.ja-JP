---
title: deviceEnrollmentConfiguration リソースの種類
description: デバイス登録構成の基本クラス
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d05914e1b25ac3712ac60274facf0904c91d4224
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940457"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a><span data-ttu-id="38761-103">deviceEnrollmentConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="38761-103">deviceEnrollmentConfiguration resource type</span></span>

> <span data-ttu-id="38761-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38761-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38761-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="38761-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38761-106">デバイス登録構成の基本クラス</span><span class="sxs-lookup"><span data-stu-id="38761-106">The Base Class of Device Enrollment Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="38761-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="38761-107">Methods</span></span>
|<span data-ttu-id="38761-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="38761-108">Method</span></span>|<span data-ttu-id="38761-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="38761-109">Return Type</span></span>|<span data-ttu-id="38761-110">説明</span><span class="sxs-lookup"><span data-stu-id="38761-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="38761-111">List deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="38761-111">List deviceEnrollmentConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-list.md)|<span data-ttu-id="38761-112">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="38761-112">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="38761-113">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="38761-113">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="38761-114">Get deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="38761-114">Get deviceEnrollmentConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-get.md)|[<span data-ttu-id="38761-115">deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="38761-115">deviceEnrollmentConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|<span data-ttu-id="38761-116">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="38761-116">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) object.</span></span>|
|[<span data-ttu-id="38761-117">setPriority アクション</span><span class="sxs-lookup"><span data-stu-id="38761-117">setPriority action</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-setpriority.md)|<span data-ttu-id="38761-118">なし</span><span class="sxs-lookup"><span data-stu-id="38761-118">None</span></span>|<span data-ttu-id="38761-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="38761-119">Not yet documented</span></span>|
|[<span data-ttu-id="38761-120">assign アクション</span><span class="sxs-lookup"><span data-stu-id="38761-120">assign action</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-assign.md)|<span data-ttu-id="38761-121">なし</span><span class="sxs-lookup"><span data-stu-id="38761-121">None</span></span>|<span data-ttu-id="38761-122">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="38761-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="38761-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38761-123">Properties</span></span>
|<span data-ttu-id="38761-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38761-124">Property</span></span>|<span data-ttu-id="38761-125">種類</span><span class="sxs-lookup"><span data-stu-id="38761-125">Type</span></span>|<span data-ttu-id="38761-126">説明</span><span class="sxs-lookup"><span data-stu-id="38761-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38761-127">id</span><span class="sxs-lookup"><span data-stu-id="38761-127">id</span></span>|<span data-ttu-id="38761-128">文字列</span><span class="sxs-lookup"><span data-stu-id="38761-128">String</span></span>|<span data-ttu-id="38761-129">アカウントの一意識別子</span><span class="sxs-lookup"><span data-stu-id="38761-129">Unique Identifier for the account</span></span>|
|<span data-ttu-id="38761-130">displayName</span><span class="sxs-lookup"><span data-stu-id="38761-130">displayName</span></span>|<span data-ttu-id="38761-131">String</span><span class="sxs-lookup"><span data-stu-id="38761-131">String</span></span>|<span data-ttu-id="38761-132">デバイス登録構成の表示名</span><span class="sxs-lookup"><span data-stu-id="38761-132">The display name of the device enrollment configuration</span></span>|
|<span data-ttu-id="38761-133">description</span><span class="sxs-lookup"><span data-stu-id="38761-133">description</span></span>|<span data-ttu-id="38761-134">String</span><span class="sxs-lookup"><span data-stu-id="38761-134">String</span></span>|<span data-ttu-id="38761-135">デバイス登録構成の説明</span><span class="sxs-lookup"><span data-stu-id="38761-135">The description of the device enrollment configuration</span></span>|
|<span data-ttu-id="38761-136">priority</span><span class="sxs-lookup"><span data-stu-id="38761-136">priority</span></span>|<span data-ttu-id="38761-137">Int32</span><span class="sxs-lookup"><span data-stu-id="38761-137">Int32</span></span>|<span data-ttu-id="38761-138">優先度は、登録構成が割り当てられている複数のグループにユーザーが存在するときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="38761-138">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="38761-139">ユーザーは、優先度の低い値を持つ構成のみに適用されます。</span><span class="sxs-lookup"><span data-stu-id="38761-139">Users are subject only to the configuration with the lowest priority value.</span></span>|
|<span data-ttu-id="38761-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38761-140">createdDateTime</span></span>|<span data-ttu-id="38761-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38761-141">DateTimeOffset</span></span>|<span data-ttu-id="38761-142">デバイス登録構成の UTC 時間で作成された日時</span><span class="sxs-lookup"><span data-stu-id="38761-142">Created date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="38761-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38761-143">lastModifiedDateTime</span></span>|<span data-ttu-id="38761-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38761-144">DateTimeOffset</span></span>|<span data-ttu-id="38761-145">デバイス登録構成の最終変更日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="38761-145">Last modified date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="38761-146">version</span><span class="sxs-lookup"><span data-stu-id="38761-146">version</span></span>|<span data-ttu-id="38761-147">Int32</span><span class="sxs-lookup"><span data-stu-id="38761-147">Int32</span></span>|<span data-ttu-id="38761-148">デバイス登録構成のバージョン</span><span class="sxs-lookup"><span data-stu-id="38761-148">The version of the device enrollment configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="38761-149">関係</span><span class="sxs-lookup"><span data-stu-id="38761-149">Relationships</span></span>
|<span data-ttu-id="38761-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="38761-150">Relationship</span></span>|<span data-ttu-id="38761-151">型</span><span class="sxs-lookup"><span data-stu-id="38761-151">Type</span></span>|<span data-ttu-id="38761-152">説明</span><span class="sxs-lookup"><span data-stu-id="38761-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38761-153">assignments</span><span class="sxs-lookup"><span data-stu-id="38761-153">assignments</span></span>|<span data-ttu-id="38761-154">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="38761-154">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="38761-155">デバイス構成プロファイルのグループ割り当ての一覧</span><span class="sxs-lookup"><span data-stu-id="38761-155">The list of group assignments for the device configuration profile</span></span>|

## <a name="json-representation"></a><span data-ttu-id="38761-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="38761-156">JSON Representation</span></span>
<span data-ttu-id="38761-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="38761-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024
}
```




