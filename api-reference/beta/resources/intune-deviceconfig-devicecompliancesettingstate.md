---
title: deviceComplianceSettingState リソース タイプ
description: 特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 96fa7bf9b93e64051b0f6271d04c1e08897c748e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333115"
---
# <a name="devicecompliancesettingstate-resource-type"></a><span data-ttu-id="78e86-103">deviceComplianceSettingState リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="78e86-103">deviceComplianceSettingState resource type</span></span>

> <span data-ttu-id="78e86-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78e86-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78e86-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="78e86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78e86-106">特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="78e86-106">Device compliance setting State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="78e86-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="78e86-107">Methods</span></span>
|<span data-ttu-id="78e86-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="78e86-108">Method</span></span>|<span data-ttu-id="78e86-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="78e86-109">Return Type</span></span>|<span data-ttu-id="78e86-110">説明</span><span class="sxs-lookup"><span data-stu-id="78e86-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="78e86-111">List deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="78e86-111">List deviceComplianceSettingStates</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|<span data-ttu-id="78e86-112">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="78e86-112">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="78e86-113">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="78e86-113">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="78e86-114">Get deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="78e86-114">Get deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[<span data-ttu-id="78e86-115">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="78e86-115">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="78e86-116">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="78e86-116">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="78e86-117">Create deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="78e86-117">Create deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[<span data-ttu-id="78e86-118">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="78e86-118">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="78e86-119">新しい [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="78e86-119">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="78e86-120">Delete deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="78e86-120">Delete deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|<span data-ttu-id="78e86-121">なし</span><span class="sxs-lookup"><span data-stu-id="78e86-121">None</span></span>|<span data-ttu-id="78e86-122">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="78e86-122">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>|
|[<span data-ttu-id="78e86-123">Update deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="78e86-123">Update deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[<span data-ttu-id="78e86-124">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="78e86-124">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="78e86-125">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="78e86-125">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="78e86-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78e86-126">Properties</span></span>
|<span data-ttu-id="78e86-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78e86-127">Property</span></span>|<span data-ttu-id="78e86-128">型</span><span class="sxs-lookup"><span data-stu-id="78e86-128">Type</span></span>|<span data-ttu-id="78e86-129">説明</span><span class="sxs-lookup"><span data-stu-id="78e86-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78e86-130">id</span><span class="sxs-lookup"><span data-stu-id="78e86-130">id</span></span>|<span data-ttu-id="78e86-131">文字列</span><span class="sxs-lookup"><span data-stu-id="78e86-131">String</span></span>|<span data-ttu-id="78e86-132">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="78e86-132">Key of the entity</span></span>|
|<span data-ttu-id="78e86-133">platformType</span><span class="sxs-lookup"><span data-stu-id="78e86-133">platformType</span></span>|[<span data-ttu-id="78e86-134">deviceType</span><span class="sxs-lookup"><span data-stu-id="78e86-134">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="78e86-135">デバイスプラットフォームの種類。</span><span class="sxs-lookup"><span data-stu-id="78e86-135">Device platform type.</span></span> <span data-ttu-id="78e86-136">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="78e86-136">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="78e86-137">setting</span><span class="sxs-lookup"><span data-stu-id="78e86-137">setting</span></span>|<span data-ttu-id="78e86-138">String</span><span class="sxs-lookup"><span data-stu-id="78e86-138">String</span></span>|<span data-ttu-id="78e86-139">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="78e86-139">The setting class name and property name.</span></span>|
|<span data-ttu-id="78e86-140">settingName</span><span class="sxs-lookup"><span data-stu-id="78e86-140">settingName</span></span>|<span data-ttu-id="78e86-141">String</span><span class="sxs-lookup"><span data-stu-id="78e86-141">String</span></span>|<span data-ttu-id="78e86-142">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="78e86-142">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="78e86-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="78e86-143">deviceId</span></span>|<span data-ttu-id="78e86-144">String</span><span class="sxs-lookup"><span data-stu-id="78e86-144">String</span></span>|<span data-ttu-id="78e86-145">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="78e86-145">The Device Id that is being reported</span></span>|
|<span data-ttu-id="78e86-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="78e86-146">deviceName</span></span>|<span data-ttu-id="78e86-147">String</span><span class="sxs-lookup"><span data-stu-id="78e86-147">String</span></span>|<span data-ttu-id="78e86-148">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="78e86-148">The Device Name that is being reported</span></span>|
|<span data-ttu-id="78e86-149">userId</span><span class="sxs-lookup"><span data-stu-id="78e86-149">userId</span></span>|<span data-ttu-id="78e86-150">String</span><span class="sxs-lookup"><span data-stu-id="78e86-150">String</span></span>|<span data-ttu-id="78e86-151">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="78e86-151">The user Id that is being reported</span></span>|
|<span data-ttu-id="78e86-152">userEmail</span><span class="sxs-lookup"><span data-stu-id="78e86-152">userEmail</span></span>|<span data-ttu-id="78e86-153">String</span><span class="sxs-lookup"><span data-stu-id="78e86-153">String</span></span>|<span data-ttu-id="78e86-154">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="78e86-154">The User email address that is being reported</span></span>|
|<span data-ttu-id="78e86-155">userName</span><span class="sxs-lookup"><span data-stu-id="78e86-155">userName</span></span>|<span data-ttu-id="78e86-156">String</span><span class="sxs-lookup"><span data-stu-id="78e86-156">String</span></span>|<span data-ttu-id="78e86-157">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="78e86-157">The User Name that is being reported</span></span>|
|<span data-ttu-id="78e86-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="78e86-158">userPrincipalName</span></span>|<span data-ttu-id="78e86-159">String</span><span class="sxs-lookup"><span data-stu-id="78e86-159">String</span></span>|<span data-ttu-id="78e86-160">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="78e86-160">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="78e86-161">deviceModel</span><span class="sxs-lookup"><span data-stu-id="78e86-161">deviceModel</span></span>|<span data-ttu-id="78e86-162">String</span><span class="sxs-lookup"><span data-stu-id="78e86-162">String</span></span>|<span data-ttu-id="78e86-163">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="78e86-163">The device model that is being reported</span></span>|
|<span data-ttu-id="78e86-164">state</span><span class="sxs-lookup"><span data-stu-id="78e86-164">state</span></span>|[<span data-ttu-id="78e86-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="78e86-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="78e86-166">設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="78e86-166">The compliance state of the setting.</span></span> <span data-ttu-id="78e86-167">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="78e86-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="78e86-168">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="78e86-168">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="78e86-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78e86-169">DateTimeOffset</span></span>|<span data-ttu-id="78e86-170">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="78e86-170">The DateTime when device compliance grace period expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="78e86-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="78e86-171">Relationships</span></span>
<span data-ttu-id="78e86-172">なし</span><span class="sxs-lookup"><span data-stu-id="78e86-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78e86-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="78e86-173">JSON Representation</span></span>
<span data-ttu-id="78e86-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="78e86-174">Here is a JSON representation of the resource.</span></span>
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
  "platformType": "String",
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



