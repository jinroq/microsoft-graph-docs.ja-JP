---
title: deviceComplianceSettingState リソース タイプ
description: 特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9ad64ca5d89700fc5cb90ec7b548a396a9648035
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031725"
---
# <a name="devicecompliancesettingstate-resource-type"></a><span data-ttu-id="bca04-103">deviceComplianceSettingState リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="bca04-103">deviceComplianceSettingState resource type</span></span>

> <span data-ttu-id="bca04-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bca04-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bca04-105">特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="bca04-105">Device compliance setting State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="bca04-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="bca04-106">Methods</span></span>
|<span data-ttu-id="bca04-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="bca04-107">Method</span></span>|<span data-ttu-id="bca04-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bca04-108">Return Type</span></span>|<span data-ttu-id="bca04-109">説明</span><span class="sxs-lookup"><span data-stu-id="bca04-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bca04-110">List deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="bca04-110">List deviceComplianceSettingStates</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|<span data-ttu-id="bca04-111">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bca04-111">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="bca04-112">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="bca04-112">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="bca04-113">Get deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="bca04-113">Get deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[<span data-ttu-id="bca04-114">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="bca04-114">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="bca04-115">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bca04-115">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="bca04-116">Create deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="bca04-116">Create deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[<span data-ttu-id="bca04-117">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="bca04-117">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="bca04-118">新しい [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bca04-118">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="bca04-119">Delete deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="bca04-119">Delete deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|<span data-ttu-id="bca04-120">なし</span><span class="sxs-lookup"><span data-stu-id="bca04-120">None</span></span>|<span data-ttu-id="bca04-121">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="bca04-121">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>|
|[<span data-ttu-id="bca04-122">Update deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="bca04-122">Update deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[<span data-ttu-id="bca04-123">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="bca04-123">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="bca04-124">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bca04-124">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bca04-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bca04-125">Properties</span></span>
|<span data-ttu-id="bca04-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bca04-126">Property</span></span>|<span data-ttu-id="bca04-127">型</span><span class="sxs-lookup"><span data-stu-id="bca04-127">Type</span></span>|<span data-ttu-id="bca04-128">説明</span><span class="sxs-lookup"><span data-stu-id="bca04-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bca04-129">id</span><span class="sxs-lookup"><span data-stu-id="bca04-129">id</span></span>|<span data-ttu-id="bca04-130">文字列</span><span class="sxs-lookup"><span data-stu-id="bca04-130">String</span></span>|<span data-ttu-id="bca04-131">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="bca04-131">Key of the entity</span></span>|
|<span data-ttu-id="bca04-132">setting</span><span class="sxs-lookup"><span data-stu-id="bca04-132">setting</span></span>|<span data-ttu-id="bca04-133">String</span><span class="sxs-lookup"><span data-stu-id="bca04-133">String</span></span>|<span data-ttu-id="bca04-134">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="bca04-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="bca04-135">settingName</span><span class="sxs-lookup"><span data-stu-id="bca04-135">settingName</span></span>|<span data-ttu-id="bca04-136">String</span><span class="sxs-lookup"><span data-stu-id="bca04-136">String</span></span>|<span data-ttu-id="bca04-137">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="bca04-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="bca04-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="bca04-138">deviceId</span></span>|<span data-ttu-id="bca04-139">String</span><span class="sxs-lookup"><span data-stu-id="bca04-139">String</span></span>|<span data-ttu-id="bca04-140">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="bca04-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="bca04-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="bca04-141">deviceName</span></span>|<span data-ttu-id="bca04-142">String</span><span class="sxs-lookup"><span data-stu-id="bca04-142">String</span></span>|<span data-ttu-id="bca04-143">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="bca04-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="bca04-144">userId</span><span class="sxs-lookup"><span data-stu-id="bca04-144">userId</span></span>|<span data-ttu-id="bca04-145">String</span><span class="sxs-lookup"><span data-stu-id="bca04-145">String</span></span>|<span data-ttu-id="bca04-146">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="bca04-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="bca04-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="bca04-147">userEmail</span></span>|<span data-ttu-id="bca04-148">String</span><span class="sxs-lookup"><span data-stu-id="bca04-148">String</span></span>|<span data-ttu-id="bca04-149">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="bca04-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="bca04-150">userName</span><span class="sxs-lookup"><span data-stu-id="bca04-150">userName</span></span>|<span data-ttu-id="bca04-151">String</span><span class="sxs-lookup"><span data-stu-id="bca04-151">String</span></span>|<span data-ttu-id="bca04-152">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="bca04-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="bca04-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bca04-153">userPrincipalName</span></span>|<span data-ttu-id="bca04-154">String</span><span class="sxs-lookup"><span data-stu-id="bca04-154">String</span></span>|<span data-ttu-id="bca04-155">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="bca04-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="bca04-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="bca04-156">deviceModel</span></span>|<span data-ttu-id="bca04-157">String</span><span class="sxs-lookup"><span data-stu-id="bca04-157">String</span></span>|<span data-ttu-id="bca04-158">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="bca04-158">The device model that is being reported</span></span>|
|<span data-ttu-id="bca04-159">state</span><span class="sxs-lookup"><span data-stu-id="bca04-159">state</span></span>|[<span data-ttu-id="bca04-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="bca04-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="bca04-161">設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="bca04-161">The compliance state of the setting.</span></span> <span data-ttu-id="bca04-162">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="bca04-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="bca04-163">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bca04-163">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="bca04-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bca04-164">DateTimeOffset</span></span>|<span data-ttu-id="bca04-165">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="bca04-165">The DateTime when device compliance grace period expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="bca04-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bca04-166">Relationships</span></span>
<span data-ttu-id="bca04-167">なし</span><span class="sxs-lookup"><span data-stu-id="bca04-167">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bca04-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bca04-168">JSON Representation</span></span>
<span data-ttu-id="bca04-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bca04-169">Here is a JSON representation of the resource.</span></span>
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



