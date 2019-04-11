---
title: deviceComplianceSettingState リソース タイプ
description: 特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 22fe0611d4ad583200032b8721076184f168d3c2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31786176"
---
# <a name="devicecompliancesettingstate-resource-type"></a><span data-ttu-id="96a62-103">deviceComplianceSettingState リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="96a62-103">deviceComplianceSettingState resource type</span></span>

> <span data-ttu-id="96a62-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96a62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96a62-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="96a62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96a62-106">特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="96a62-106">Device compliance setting State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="96a62-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="96a62-107">Methods</span></span>
|<span data-ttu-id="96a62-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="96a62-108">Method</span></span>|<span data-ttu-id="96a62-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="96a62-109">Return Type</span></span>|<span data-ttu-id="96a62-110">説明</span><span class="sxs-lookup"><span data-stu-id="96a62-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="96a62-111">List deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="96a62-111">List deviceComplianceSettingStates</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|<span data-ttu-id="96a62-112">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="96a62-112">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="96a62-113">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="96a62-113">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="96a62-114">Get deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="96a62-114">Get deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[<span data-ttu-id="96a62-115">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="96a62-115">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="96a62-116">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="96a62-116">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="96a62-117">deviceComplianceSettingState の作成</span><span class="sxs-lookup"><span data-stu-id="96a62-117">Create deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[<span data-ttu-id="96a62-118">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="96a62-118">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="96a62-119">新しい [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="96a62-119">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="96a62-120">deviceComplianceSettingState の削除</span><span class="sxs-lookup"><span data-stu-id="96a62-120">Delete deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|<span data-ttu-id="96a62-121">なし</span><span class="sxs-lookup"><span data-stu-id="96a62-121">None</span></span>|<span data-ttu-id="96a62-122">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="96a62-122">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>|
|[<span data-ttu-id="96a62-123">deviceComplianceSettingState の更新</span><span class="sxs-lookup"><span data-stu-id="96a62-123">Update deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[<span data-ttu-id="96a62-124">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="96a62-124">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="96a62-125">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="96a62-125">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="96a62-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96a62-126">Properties</span></span>
|<span data-ttu-id="96a62-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96a62-127">Property</span></span>|<span data-ttu-id="96a62-128">型</span><span class="sxs-lookup"><span data-stu-id="96a62-128">Type</span></span>|<span data-ttu-id="96a62-129">説明</span><span class="sxs-lookup"><span data-stu-id="96a62-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96a62-130">id</span><span class="sxs-lookup"><span data-stu-id="96a62-130">id</span></span>|<span data-ttu-id="96a62-131">String</span><span class="sxs-lookup"><span data-stu-id="96a62-131">String</span></span>|<span data-ttu-id="96a62-132">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="96a62-132">Key of the entity</span></span>|
|<span data-ttu-id="96a62-133">platformType</span><span class="sxs-lookup"><span data-stu-id="96a62-133">platformType</span></span>|[<span data-ttu-id="96a62-134">deviceType</span><span class="sxs-lookup"><span data-stu-id="96a62-134">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="96a62-135">デバイスプラットフォームの種類。</span><span class="sxs-lookup"><span data-stu-id="96a62-135">Device platform type.</span></span> <span data-ttu-id="96a62-136">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="96a62-136">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="96a62-137">setting</span><span class="sxs-lookup"><span data-stu-id="96a62-137">setting</span></span>|<span data-ttu-id="96a62-138">文字列</span><span class="sxs-lookup"><span data-stu-id="96a62-138">String</span></span>|<span data-ttu-id="96a62-139">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="96a62-139">The setting class name and property name.</span></span>|
|<span data-ttu-id="96a62-140">settingName</span><span class="sxs-lookup"><span data-stu-id="96a62-140">settingName</span></span>|<span data-ttu-id="96a62-141">文字列</span><span class="sxs-lookup"><span data-stu-id="96a62-141">String</span></span>|<span data-ttu-id="96a62-142">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="96a62-142">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="96a62-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="96a62-143">deviceId</span></span>|<span data-ttu-id="96a62-144">文字列</span><span class="sxs-lookup"><span data-stu-id="96a62-144">String</span></span>|<span data-ttu-id="96a62-145">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="96a62-145">The Device Id that is being reported</span></span>|
|<span data-ttu-id="96a62-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="96a62-146">deviceName</span></span>|<span data-ttu-id="96a62-147">文字列</span><span class="sxs-lookup"><span data-stu-id="96a62-147">String</span></span>|<span data-ttu-id="96a62-148">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="96a62-148">The Device Name that is being reported</span></span>|
|<span data-ttu-id="96a62-149">userId</span><span class="sxs-lookup"><span data-stu-id="96a62-149">userId</span></span>|<span data-ttu-id="96a62-150">文字列</span><span class="sxs-lookup"><span data-stu-id="96a62-150">String</span></span>|<span data-ttu-id="96a62-151">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="96a62-151">The user Id that is being reported</span></span>|
|<span data-ttu-id="96a62-152">userEmail</span><span class="sxs-lookup"><span data-stu-id="96a62-152">userEmail</span></span>|<span data-ttu-id="96a62-153">String</span><span class="sxs-lookup"><span data-stu-id="96a62-153">String</span></span>|<span data-ttu-id="96a62-154">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="96a62-154">The User email address that is being reported</span></span>|
|<span data-ttu-id="96a62-155">userName</span><span class="sxs-lookup"><span data-stu-id="96a62-155">userName</span></span>|<span data-ttu-id="96a62-156">文字列</span><span class="sxs-lookup"><span data-stu-id="96a62-156">String</span></span>|<span data-ttu-id="96a62-157">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="96a62-157">The User Name that is being reported</span></span>|
|<span data-ttu-id="96a62-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="96a62-158">userPrincipalName</span></span>|<span data-ttu-id="96a62-159">String</span><span class="sxs-lookup"><span data-stu-id="96a62-159">String</span></span>|<span data-ttu-id="96a62-160">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="96a62-160">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="96a62-161">deviceModel</span><span class="sxs-lookup"><span data-stu-id="96a62-161">deviceModel</span></span>|<span data-ttu-id="96a62-162">文字列</span><span class="sxs-lookup"><span data-stu-id="96a62-162">String</span></span>|<span data-ttu-id="96a62-163">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="96a62-163">The device model that is being reported</span></span>|
|<span data-ttu-id="96a62-164">state</span><span class="sxs-lookup"><span data-stu-id="96a62-164">state</span></span>|[<span data-ttu-id="96a62-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="96a62-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="96a62-166">設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="96a62-166">The compliance state of the setting.</span></span> <span data-ttu-id="96a62-167">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="96a62-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="96a62-168">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="96a62-168">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="96a62-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96a62-169">DateTimeOffset</span></span>|<span data-ttu-id="96a62-170">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="96a62-170">The DateTime when device compliance grace period expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="96a62-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="96a62-171">Relationships</span></span>
<span data-ttu-id="96a62-172">なし</span><span class="sxs-lookup"><span data-stu-id="96a62-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96a62-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="96a62-173">JSON Representation</span></span>
<span data-ttu-id="96a62-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="96a62-174">Here is a JSON representation of the resource.</span></span>
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





