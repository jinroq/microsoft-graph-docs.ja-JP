---
title: devicemanagementintentdevicestate リソースの種類
description: 目的のデバイス状態を表すエンティティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1db6b0d5d7376b5c71b3be5753a777477c3b3850
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575794"
---
# <a name="devicemanagementintentdevicestate-resource-type"></a><span data-ttu-id="0a8a8-103">devicemanagementintentdevicestate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a8a8-103">deviceManagementIntentDeviceState resource type</span></span>

> <span data-ttu-id="0a8a8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a8a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a8a8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0a8a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a8a8-106">目的のデバイス状態を表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="0a8a8-106">Entity that represents device state for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="0a8a8-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0a8a8-107">Methods</span></span>
|<span data-ttu-id="0a8a8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0a8a8-108">Method</span></span>|<span data-ttu-id="0a8a8-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0a8a8-109">Return Type</span></span>|<span data-ttu-id="0a8a8-110">説明</span><span class="sxs-lookup"><span data-stu-id="0a8a8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0a8a8-111">リスト deviceManagementIntentDeviceStates</span><span class="sxs-lookup"><span data-stu-id="0a8a8-111">List deviceManagementIntentDeviceStates</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestate-list.md)|<span data-ttu-id="0a8a8-112">[devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0a8a8-112">[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) collection</span></span>|<span data-ttu-id="0a8a8-113">[devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0a8a8-113">List properties and relationships of the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="0a8a8-114">devicemanagementintentdevicestate の取得</span><span class="sxs-lookup"><span data-stu-id="0a8a8-114">Get deviceManagementIntentDeviceState</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestate-get.md)|[<span data-ttu-id="0a8a8-115">deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="0a8a8-115">deviceManagementIntentDeviceState</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|<span data-ttu-id="0a8a8-116">[devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0a8a8-116">Read properties and relationships of the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>|
|[<span data-ttu-id="0a8a8-117">devicemanagementintentdevicestate の作成</span><span class="sxs-lookup"><span data-stu-id="0a8a8-117">Create deviceManagementIntentDeviceState</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestate-create.md)|[<span data-ttu-id="0a8a8-118">deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="0a8a8-118">deviceManagementIntentDeviceState</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|<span data-ttu-id="0a8a8-119">新しい[devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0a8a8-119">Create a new [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>|
|[<span data-ttu-id="0a8a8-120">devicemanagementintentdevicestate の削除</span><span class="sxs-lookup"><span data-stu-id="0a8a8-120">Delete deviceManagementIntentDeviceState</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestate-delete.md)|<span data-ttu-id="0a8a8-121">なし</span><span class="sxs-lookup"><span data-stu-id="0a8a8-121">None</span></span>|<span data-ttu-id="0a8a8-122">[devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="0a8a8-122">Deletes a [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md).</span></span>|
|[<span data-ttu-id="0a8a8-123">devicemanagementintentdevicestate の更新</span><span class="sxs-lookup"><span data-stu-id="0a8a8-123">Update deviceManagementIntentDeviceState</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestate-update.md)|[<span data-ttu-id="0a8a8-124">deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="0a8a8-124">deviceManagementIntentDeviceState</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|<span data-ttu-id="0a8a8-125">[devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0a8a8-125">Update the properties of a [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0a8a8-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a8a8-126">Properties</span></span>
|<span data-ttu-id="0a8a8-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a8a8-127">Property</span></span>|<span data-ttu-id="0a8a8-128">型</span><span class="sxs-lookup"><span data-stu-id="0a8a8-128">Type</span></span>|<span data-ttu-id="0a8a8-129">説明</span><span class="sxs-lookup"><span data-stu-id="0a8a8-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a8a8-130">id</span><span class="sxs-lookup"><span data-stu-id="0a8a8-130">id</span></span>|<span data-ttu-id="0a8a8-131">String</span><span class="sxs-lookup"><span data-stu-id="0a8a8-131">String</span></span>|<span data-ttu-id="0a8a8-132">ID</span><span class="sxs-lookup"><span data-stu-id="0a8a8-132">The ID</span></span>|
|<span data-ttu-id="0a8a8-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0a8a8-133">userPrincipalName</span></span>|<span data-ttu-id="0a8a8-134">String</span><span class="sxs-lookup"><span data-stu-id="0a8a8-134">String</span></span>|<span data-ttu-id="0a8a8-135">デバイスで報告されているユーザープリンシパル名</span><span class="sxs-lookup"><span data-stu-id="0a8a8-135">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="0a8a8-136">userName</span><span class="sxs-lookup"><span data-stu-id="0a8a8-136">userName</span></span>|<span data-ttu-id="0a8a8-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0a8a8-137">String</span></span>|<span data-ttu-id="0a8a8-138">デバイスで報告されているユーザー名</span><span class="sxs-lookup"><span data-stu-id="0a8a8-138">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="0a8a8-139">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="0a8a8-139">deviceDisplayName</span></span>|<span data-ttu-id="0a8a8-140">String</span><span class="sxs-lookup"><span data-stu-id="0a8a8-140">String</span></span>|<span data-ttu-id="0a8a8-141">レポートされているデバイス名</span><span class="sxs-lookup"><span data-stu-id="0a8a8-141">Device name that is being reported</span></span>|
|<span data-ttu-id="0a8a8-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a8a8-142">lastReportedDateTime</span></span>|<span data-ttu-id="0a8a8-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a8a8-143">DateTimeOffset</span></span>|<span data-ttu-id="0a8a8-144">インテントレポートの最終更新日時</span><span class="sxs-lookup"><span data-stu-id="0a8a8-144">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="0a8a8-145">state</span><span class="sxs-lookup"><span data-stu-id="0a8a8-145">state</span></span>|[<span data-ttu-id="0a8a8-146">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="0a8a8-146">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="0a8a8-147">目的のデバイス状態。</span><span class="sxs-lookup"><span data-stu-id="0a8a8-147">Device state for an intent.</span></span> <span data-ttu-id="0a8a8-148">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="0a8a8-148">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="0a8a8-149">deviceId</span><span class="sxs-lookup"><span data-stu-id="0a8a8-149">deviceId</span></span>|<span data-ttu-id="0a8a8-150">String</span><span class="sxs-lookup"><span data-stu-id="0a8a8-150">String</span></span>|<span data-ttu-id="0a8a8-151">レポートされているデバイス id</span><span class="sxs-lookup"><span data-stu-id="0a8a8-151">Device id that is being reported</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a8a8-152">関係</span><span class="sxs-lookup"><span data-stu-id="0a8a8-152">Relationships</span></span>
<span data-ttu-id="0a8a8-153">なし</span><span class="sxs-lookup"><span data-stu-id="0a8a8-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a8a8-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a8a8-154">JSON Representation</span></span>
<span data-ttu-id="0a8a8-155">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0a8a8-155">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "userName": "String",
  "deviceDisplayName": "String",
  "lastReportedDateTime": "String (timestamp)",
  "state": "String",
  "deviceId": "String"
}
```





