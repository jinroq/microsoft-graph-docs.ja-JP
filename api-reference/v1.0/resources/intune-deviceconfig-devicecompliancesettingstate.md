---
title: deviceComplianceSettingState リソース タイプ
description: 特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63285c5b0d0c7d1b342d13478777ddd6e87ae17f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254073"
---
# <a name="devicecompliancesettingstate-resource-type"></a><span data-ttu-id="8068b-103">deviceComplianceSettingState リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="8068b-103">deviceComplianceSettingState resource type</span></span>

> <span data-ttu-id="8068b-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8068b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8068b-105">特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="8068b-105">Device compliance setting State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="8068b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="8068b-106">Methods</span></span>
|<span data-ttu-id="8068b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="8068b-107">Method</span></span>|<span data-ttu-id="8068b-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8068b-108">Return Type</span></span>|<span data-ttu-id="8068b-109">説明</span><span class="sxs-lookup"><span data-stu-id="8068b-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8068b-110">List deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="8068b-110">List deviceComplianceSettingStates</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|<span data-ttu-id="8068b-111">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8068b-111">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="8068b-112">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8068b-112">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="8068b-113">Get deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="8068b-113">Get deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[<span data-ttu-id="8068b-114">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="8068b-114">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="8068b-115">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8068b-115">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="8068b-116">Create deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="8068b-116">Create deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[<span data-ttu-id="8068b-117">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="8068b-117">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="8068b-118">新しい [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8068b-118">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="8068b-119">Delete deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="8068b-119">Delete deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|<span data-ttu-id="8068b-120">なし</span><span class="sxs-lookup"><span data-stu-id="8068b-120">None</span></span>|<span data-ttu-id="8068b-121">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="8068b-121">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>|
|[<span data-ttu-id="8068b-122">Update deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="8068b-122">Update deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[<span data-ttu-id="8068b-123">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="8068b-123">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="8068b-124">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8068b-124">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8068b-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8068b-125">Properties</span></span>
|<span data-ttu-id="8068b-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8068b-126">Property</span></span>|<span data-ttu-id="8068b-127">型</span><span class="sxs-lookup"><span data-stu-id="8068b-127">Type</span></span>|<span data-ttu-id="8068b-128">説明</span><span class="sxs-lookup"><span data-stu-id="8068b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8068b-129">id</span><span class="sxs-lookup"><span data-stu-id="8068b-129">id</span></span>|<span data-ttu-id="8068b-130">String</span><span class="sxs-lookup"><span data-stu-id="8068b-130">String</span></span>|<span data-ttu-id="8068b-131">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="8068b-131">Key of the entity</span></span>|
|<span data-ttu-id="8068b-132">setting</span><span class="sxs-lookup"><span data-stu-id="8068b-132">setting</span></span>|<span data-ttu-id="8068b-133">String</span><span class="sxs-lookup"><span data-stu-id="8068b-133">String</span></span>|<span data-ttu-id="8068b-134">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="8068b-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="8068b-135">settingName</span><span class="sxs-lookup"><span data-stu-id="8068b-135">settingName</span></span>|<span data-ttu-id="8068b-136">String</span><span class="sxs-lookup"><span data-stu-id="8068b-136">String</span></span>|<span data-ttu-id="8068b-137">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="8068b-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="8068b-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="8068b-138">deviceId</span></span>|<span data-ttu-id="8068b-139">String</span><span class="sxs-lookup"><span data-stu-id="8068b-139">String</span></span>|<span data-ttu-id="8068b-140">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="8068b-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="8068b-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="8068b-141">deviceName</span></span>|<span data-ttu-id="8068b-142">String</span><span class="sxs-lookup"><span data-stu-id="8068b-142">String</span></span>|<span data-ttu-id="8068b-143">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="8068b-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="8068b-144">userId</span><span class="sxs-lookup"><span data-stu-id="8068b-144">userId</span></span>|<span data-ttu-id="8068b-145">String</span><span class="sxs-lookup"><span data-stu-id="8068b-145">String</span></span>|<span data-ttu-id="8068b-146">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="8068b-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="8068b-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="8068b-147">userEmail</span></span>|<span data-ttu-id="8068b-148">String</span><span class="sxs-lookup"><span data-stu-id="8068b-148">String</span></span>|<span data-ttu-id="8068b-149">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="8068b-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="8068b-150">userName</span><span class="sxs-lookup"><span data-stu-id="8068b-150">userName</span></span>|<span data-ttu-id="8068b-151">String</span><span class="sxs-lookup"><span data-stu-id="8068b-151">String</span></span>|<span data-ttu-id="8068b-152">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="8068b-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="8068b-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8068b-153">userPrincipalName</span></span>|<span data-ttu-id="8068b-154">String</span><span class="sxs-lookup"><span data-stu-id="8068b-154">String</span></span>|<span data-ttu-id="8068b-155">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="8068b-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="8068b-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="8068b-156">deviceModel</span></span>|<span data-ttu-id="8068b-157">String</span><span class="sxs-lookup"><span data-stu-id="8068b-157">String</span></span>|<span data-ttu-id="8068b-158">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="8068b-158">The device model that is being reported</span></span>|
|<span data-ttu-id="8068b-159">state</span><span class="sxs-lookup"><span data-stu-id="8068b-159">state</span></span>|[<span data-ttu-id="8068b-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="8068b-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="8068b-161">設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="8068b-161">The compliance state of the setting.</span></span> <span data-ttu-id="8068b-162">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="8068b-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="8068b-163">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8068b-163">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="8068b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8068b-164">DateTimeOffset</span></span>|<span data-ttu-id="8068b-165">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="8068b-165">The DateTime when device compliance grace period expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="8068b-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8068b-166">Relationships</span></span>
<span data-ttu-id="8068b-167">なし</span><span class="sxs-lookup"><span data-stu-id="8068b-167">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8068b-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8068b-168">JSON Representation</span></span>
<span data-ttu-id="8068b-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8068b-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "String (identifier)",
  "setting": "String",
  "settingName": "String",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userEmail": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "deviceModel": "String",
  "state": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)"
}
```



