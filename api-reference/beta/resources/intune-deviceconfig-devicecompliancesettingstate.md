---
title: deviceComplianceSettingState リソース タイプ
description: 特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。
author: tfitzmac
ms.openlocfilehash: 4fe74d529d0768f773652ce0bbc6aa37f221db9e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326496"
---
# <a name="devicecompliancesettingstate-resource-type"></a><span data-ttu-id="49564-103">deviceComplianceSettingState リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="49564-103">deviceComplianceSettingState resource type</span></span>

> <span data-ttu-id="49564-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="49564-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49564-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49564-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49564-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="49564-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49564-107">特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="49564-107">Device compliance setting State for a given device.</span></span>
## <a name="methods"></a><span data-ttu-id="49564-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="49564-108">Methods</span></span>
|<span data-ttu-id="49564-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="49564-109">Method</span></span>|<span data-ttu-id="49564-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="49564-110">Return Type</span></span>|<span data-ttu-id="49564-111">説明</span><span class="sxs-lookup"><span data-stu-id="49564-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="49564-112">List deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="49564-112">List deviceComplianceSettingStates</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|<span data-ttu-id="49564-113">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="49564-113">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="49564-114">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="49564-114">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="49564-115">Get deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="49564-115">Get deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[<span data-ttu-id="49564-116">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="49564-116">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="49564-117">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="49564-117">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="49564-118">Create deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="49564-118">Create deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[<span data-ttu-id="49564-119">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="49564-119">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="49564-120">新しい [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="49564-120">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="49564-121">Delete deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="49564-121">Delete deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|<span data-ttu-id="49564-122">なし</span><span class="sxs-lookup"><span data-stu-id="49564-122">None</span></span>|<span data-ttu-id="49564-123">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="49564-123">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>|
|[<span data-ttu-id="49564-124">Update deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="49564-124">Update deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[<span data-ttu-id="49564-125">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="49564-125">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="49564-126">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="49564-126">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="49564-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49564-127">Properties</span></span>
|<span data-ttu-id="49564-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49564-128">Property</span></span>|<span data-ttu-id="49564-129">種類</span><span class="sxs-lookup"><span data-stu-id="49564-129">Type</span></span>|<span data-ttu-id="49564-130">説明</span><span class="sxs-lookup"><span data-stu-id="49564-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49564-131">ID</span><span class="sxs-lookup"><span data-stu-id="49564-131">id</span></span>|<span data-ttu-id="49564-132">String</span><span class="sxs-lookup"><span data-stu-id="49564-132">String</span></span>|<span data-ttu-id="49564-133">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="49564-133">Key of the entity</span></span>|
|<span data-ttu-id="49564-134">platformType</span><span class="sxs-lookup"><span data-stu-id="49564-134">platformType</span></span>|[<span data-ttu-id="49564-135">deviceType</span><span class="sxs-lookup"><span data-stu-id="49564-135">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="49564-136">デバイス プラットフォームのタイプです。</span><span class="sxs-lookup"><span data-stu-id="49564-136">Device platform type.</span></span> <span data-ttu-id="49564-137">使用可能な値: `desktop`、 `windowsRT`、 `winMO6`、 `nokia`、 `windowsPhone`、 `mac`、 `winCE`、 `winEmbedded`、 `iPhone`、 `iPad`、 `iPod`、 `android`、 `iSocConsumer`、 `unix`、 `macMDM`、 `holoLens`、 `surfaceHub`、 `androidForWork`、 `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="49564-137">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="49564-138">setting</span><span class="sxs-lookup"><span data-stu-id="49564-138">setting</span></span>|<span data-ttu-id="49564-139">String</span><span class="sxs-lookup"><span data-stu-id="49564-139">String</span></span>|<span data-ttu-id="49564-140">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="49564-140">The setting class name and property name.</span></span>|
|<span data-ttu-id="49564-141">settingName</span><span class="sxs-lookup"><span data-stu-id="49564-141">settingName</span></span>|<span data-ttu-id="49564-142">String</span><span class="sxs-lookup"><span data-stu-id="49564-142">String</span></span>|<span data-ttu-id="49564-143">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="49564-143">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="49564-144">deviceId</span><span class="sxs-lookup"><span data-stu-id="49564-144">deviceId</span></span>|<span data-ttu-id="49564-145">String</span><span class="sxs-lookup"><span data-stu-id="49564-145">String</span></span>|<span data-ttu-id="49564-146">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="49564-146">The Device Id that is being reported</span></span>|
|<span data-ttu-id="49564-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="49564-147">deviceName</span></span>|<span data-ttu-id="49564-148">String</span><span class="sxs-lookup"><span data-stu-id="49564-148">String</span></span>|<span data-ttu-id="49564-149">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="49564-149">The Device Name that is being reported</span></span>|
|<span data-ttu-id="49564-150">userId</span><span class="sxs-lookup"><span data-stu-id="49564-150">userId</span></span>|<span data-ttu-id="49564-151">String</span><span class="sxs-lookup"><span data-stu-id="49564-151">String</span></span>|<span data-ttu-id="49564-152">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="49564-152">The user Id that is being reported</span></span>|
|<span data-ttu-id="49564-153">userEmail</span><span class="sxs-lookup"><span data-stu-id="49564-153">userEmail</span></span>|<span data-ttu-id="49564-154">String</span><span class="sxs-lookup"><span data-stu-id="49564-154">String</span></span>|<span data-ttu-id="49564-155">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="49564-155">The User email address that is being reported</span></span>|
|<span data-ttu-id="49564-156">userName</span><span class="sxs-lookup"><span data-stu-id="49564-156">userName</span></span>|<span data-ttu-id="49564-157">String</span><span class="sxs-lookup"><span data-stu-id="49564-157">String</span></span>|<span data-ttu-id="49564-158">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="49564-158">The User Name that is being reported</span></span>|
|<span data-ttu-id="49564-159">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="49564-159">userPrincipalName</span></span>|<span data-ttu-id="49564-160">String</span><span class="sxs-lookup"><span data-stu-id="49564-160">String</span></span>|<span data-ttu-id="49564-161">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="49564-161">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="49564-162">deviceModel</span><span class="sxs-lookup"><span data-stu-id="49564-162">deviceModel</span></span>|<span data-ttu-id="49564-163">String</span><span class="sxs-lookup"><span data-stu-id="49564-163">String</span></span>|<span data-ttu-id="49564-164">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="49564-164">The device model that is being reported</span></span>|
|<span data-ttu-id="49564-165">state</span><span class="sxs-lookup"><span data-stu-id="49564-165">state</span></span>|[<span data-ttu-id="49564-166">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="49564-166">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="49564-167">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="49564-167">The compliance state of the setting.</span></span> <span data-ttu-id="49564-168">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="49564-168">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="49564-169">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="49564-169">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="49564-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49564-170">DateTimeOffset</span></span>|<span data-ttu-id="49564-171">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="49564-171">The DateTime when device compliance grace period expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="49564-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="49564-172">Relationships</span></span>
<span data-ttu-id="49564-173">なし</span><span class="sxs-lookup"><span data-stu-id="49564-173">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="49564-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="49564-174">JSON Representation</span></span>
<span data-ttu-id="49564-175">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="49564-175">Here is a JSON representation of the resource.</span></span>
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





