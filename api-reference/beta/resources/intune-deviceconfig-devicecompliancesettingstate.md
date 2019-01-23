---
title: deviceComplianceSettingState リソース タイプ
description: 特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d618356d115f437bccccee57f6c259a1cdbd14a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403036"
---
# <a name="devicecompliancesettingstate-resource-type"></a><span data-ttu-id="af7e0-103">deviceComplianceSettingState リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="af7e0-103">deviceComplianceSettingState resource type</span></span>

> <span data-ttu-id="af7e0-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="af7e0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="af7e0-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af7e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af7e0-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="af7e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af7e0-107">特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="af7e0-107">Device compliance setting State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="af7e0-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="af7e0-108">Methods</span></span>
|<span data-ttu-id="af7e0-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="af7e0-109">Method</span></span>|<span data-ttu-id="af7e0-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="af7e0-110">Return Type</span></span>|<span data-ttu-id="af7e0-111">説明</span><span class="sxs-lookup"><span data-stu-id="af7e0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="af7e0-112">List deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="af7e0-112">List deviceComplianceSettingStates</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|<span data-ttu-id="af7e0-113">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="af7e0-113">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="af7e0-114">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="af7e0-114">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="af7e0-115">Get deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="af7e0-115">Get deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[<span data-ttu-id="af7e0-116">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="af7e0-116">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="af7e0-117">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="af7e0-117">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="af7e0-118">Create deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="af7e0-118">Create deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[<span data-ttu-id="af7e0-119">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="af7e0-119">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="af7e0-120">新しい [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="af7e0-120">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="af7e0-121">Delete deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="af7e0-121">Delete deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|<span data-ttu-id="af7e0-122">なし</span><span class="sxs-lookup"><span data-stu-id="af7e0-122">None</span></span>|<span data-ttu-id="af7e0-123">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="af7e0-123">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>|
|[<span data-ttu-id="af7e0-124">Update deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="af7e0-124">Update deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[<span data-ttu-id="af7e0-125">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="af7e0-125">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="af7e0-126">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="af7e0-126">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="af7e0-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af7e0-127">Properties</span></span>
|<span data-ttu-id="af7e0-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af7e0-128">Property</span></span>|<span data-ttu-id="af7e0-129">型</span><span class="sxs-lookup"><span data-stu-id="af7e0-129">Type</span></span>|<span data-ttu-id="af7e0-130">説明</span><span class="sxs-lookup"><span data-stu-id="af7e0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af7e0-131">id</span><span class="sxs-lookup"><span data-stu-id="af7e0-131">id</span></span>|<span data-ttu-id="af7e0-132">String</span><span class="sxs-lookup"><span data-stu-id="af7e0-132">String</span></span>|<span data-ttu-id="af7e0-133">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="af7e0-133">Key of the entity</span></span>|
|<span data-ttu-id="af7e0-134">platformType</span><span class="sxs-lookup"><span data-stu-id="af7e0-134">platformType</span></span>|[<span data-ttu-id="af7e0-135">deviceType</span><span class="sxs-lookup"><span data-stu-id="af7e0-135">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="af7e0-136">デバイス プラットフォームのタイプです。</span><span class="sxs-lookup"><span data-stu-id="af7e0-136">Device platform type.</span></span> <span data-ttu-id="af7e0-137">使用可能な値: `desktop`、 `windowsRT`、 `winMO6`、 `nokia`、 `windowsPhone`、 `mac`、 `winCE`、 `winEmbedded`、 `iPhone`、 `iPad`、 `iPod`、 `android`、 `iSocConsumer`、 `unix`、 `macMDM`、 `holoLens`、 `surfaceHub`、 `androidForWork`、 `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="af7e0-137">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="af7e0-138">setting</span><span class="sxs-lookup"><span data-stu-id="af7e0-138">setting</span></span>|<span data-ttu-id="af7e0-139">String</span><span class="sxs-lookup"><span data-stu-id="af7e0-139">String</span></span>|<span data-ttu-id="af7e0-140">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="af7e0-140">The setting class name and property name.</span></span>|
|<span data-ttu-id="af7e0-141">settingName</span><span class="sxs-lookup"><span data-stu-id="af7e0-141">settingName</span></span>|<span data-ttu-id="af7e0-142">String</span><span class="sxs-lookup"><span data-stu-id="af7e0-142">String</span></span>|<span data-ttu-id="af7e0-143">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="af7e0-143">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="af7e0-144">deviceId</span><span class="sxs-lookup"><span data-stu-id="af7e0-144">deviceId</span></span>|<span data-ttu-id="af7e0-145">String</span><span class="sxs-lookup"><span data-stu-id="af7e0-145">String</span></span>|<span data-ttu-id="af7e0-146">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="af7e0-146">The Device Id that is being reported</span></span>|
|<span data-ttu-id="af7e0-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="af7e0-147">deviceName</span></span>|<span data-ttu-id="af7e0-148">String</span><span class="sxs-lookup"><span data-stu-id="af7e0-148">String</span></span>|<span data-ttu-id="af7e0-149">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="af7e0-149">The Device Name that is being reported</span></span>|
|<span data-ttu-id="af7e0-150">userId</span><span class="sxs-lookup"><span data-stu-id="af7e0-150">userId</span></span>|<span data-ttu-id="af7e0-151">String</span><span class="sxs-lookup"><span data-stu-id="af7e0-151">String</span></span>|<span data-ttu-id="af7e0-152">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="af7e0-152">The user Id that is being reported</span></span>|
|<span data-ttu-id="af7e0-153">userEmail</span><span class="sxs-lookup"><span data-stu-id="af7e0-153">userEmail</span></span>|<span data-ttu-id="af7e0-154">String</span><span class="sxs-lookup"><span data-stu-id="af7e0-154">String</span></span>|<span data-ttu-id="af7e0-155">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="af7e0-155">The User email address that is being reported</span></span>|
|<span data-ttu-id="af7e0-156">userName</span><span class="sxs-lookup"><span data-stu-id="af7e0-156">userName</span></span>|<span data-ttu-id="af7e0-157">String</span><span class="sxs-lookup"><span data-stu-id="af7e0-157">String</span></span>|<span data-ttu-id="af7e0-158">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="af7e0-158">The User Name that is being reported</span></span>|
|<span data-ttu-id="af7e0-159">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="af7e0-159">userPrincipalName</span></span>|<span data-ttu-id="af7e0-160">String</span><span class="sxs-lookup"><span data-stu-id="af7e0-160">String</span></span>|<span data-ttu-id="af7e0-161">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="af7e0-161">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="af7e0-162">deviceModel</span><span class="sxs-lookup"><span data-stu-id="af7e0-162">deviceModel</span></span>|<span data-ttu-id="af7e0-163">String</span><span class="sxs-lookup"><span data-stu-id="af7e0-163">String</span></span>|<span data-ttu-id="af7e0-164">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="af7e0-164">The device model that is being reported</span></span>|
|<span data-ttu-id="af7e0-165">state</span><span class="sxs-lookup"><span data-stu-id="af7e0-165">state</span></span>|[<span data-ttu-id="af7e0-166">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="af7e0-166">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="af7e0-167">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="af7e0-167">The compliance state of the setting.</span></span> <span data-ttu-id="af7e0-168">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="af7e0-168">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="af7e0-169">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="af7e0-169">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="af7e0-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af7e0-170">DateTimeOffset</span></span>|<span data-ttu-id="af7e0-171">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="af7e0-171">The DateTime when device compliance grace period expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="af7e0-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="af7e0-172">Relationships</span></span>
<span data-ttu-id="af7e0-173">なし</span><span class="sxs-lookup"><span data-stu-id="af7e0-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af7e0-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="af7e0-174">JSON Representation</span></span>
<span data-ttu-id="af7e0-175">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="af7e0-175">Here is a JSON representation of the resource.</span></span>
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




