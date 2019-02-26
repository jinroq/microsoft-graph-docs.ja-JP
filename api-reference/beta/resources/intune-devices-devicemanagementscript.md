---
title: devicemanagementscript リソースの種類
description: Intune は、登録済みの windows 10 Azure Active Directory 参加済みデバイスで Powershell スクリプトを実行する機能をお客様に提供します。 このスクリプトは、一度または定期的に実行できます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3fffd6bec8866066824725f1477e6de0e71ebf9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164065"
---
# <a name="devicemanagementscript-resource-type"></a><span data-ttu-id="52b64-104">devicemanagementscript リソースの種類</span><span class="sxs-lookup"><span data-stu-id="52b64-104">deviceManagementScript resource type</span></span>

> <span data-ttu-id="52b64-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52b64-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52b64-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="52b64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52b64-107">Intune は、登録済みの windows 10 Azure Active Directory 参加済みデバイスで Powershell スクリプトを実行する機能をお客様に提供します。</span><span class="sxs-lookup"><span data-stu-id="52b64-107">Intune will provide customer the ability to run their Powershell scripts on the enrolled windows 10 Azure Active Directory joined devices.</span></span> <span data-ttu-id="52b64-108">このスクリプトは、一度または定期的に実行できます。</span><span class="sxs-lookup"><span data-stu-id="52b64-108">The script can be run once or periodically.</span></span>

## <a name="methods"></a><span data-ttu-id="52b64-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="52b64-109">Methods</span></span>
|<span data-ttu-id="52b64-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="52b64-110">Method</span></span>|<span data-ttu-id="52b64-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="52b64-111">Return Type</span></span>|<span data-ttu-id="52b64-112">説明</span><span class="sxs-lookup"><span data-stu-id="52b64-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="52b64-113">devicemanagementscripts を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="52b64-113">List deviceManagementScripts</span></span>](../api/intune-devices-devicemanagementscript-list.md)|<span data-ttu-id="52b64-114">[devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="52b64-114">[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) collection</span></span>|<span data-ttu-id="52b64-115">[devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="52b64-115">List properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects.</span></span>|
|[<span data-ttu-id="52b64-116">devicemanagementscript の取得</span><span class="sxs-lookup"><span data-stu-id="52b64-116">Get deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-get.md)|[<span data-ttu-id="52b64-117">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="52b64-117">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="52b64-118">[devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="52b64-118">Read properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="52b64-119">devicemanagementscript の作成</span><span class="sxs-lookup"><span data-stu-id="52b64-119">Create deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-create.md)|[<span data-ttu-id="52b64-120">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="52b64-120">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="52b64-121">新しい[devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="52b64-121">Create a new [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="52b64-122">devicemanagementscript の削除</span><span class="sxs-lookup"><span data-stu-id="52b64-122">Delete deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-delete.md)|<span data-ttu-id="52b64-123">なし</span><span class="sxs-lookup"><span data-stu-id="52b64-123">None</span></span>|<span data-ttu-id="52b64-124">[devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="52b64-124">Deletes a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>|
|[<span data-ttu-id="52b64-125">devicemanagementscript の更新</span><span class="sxs-lookup"><span data-stu-id="52b64-125">Update deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-update.md)|[<span data-ttu-id="52b64-126">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="52b64-126">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="52b64-127">[devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="52b64-127">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="52b64-128">assign action</span><span class="sxs-lookup"><span data-stu-id="52b64-128">assign action</span></span>](../api/intune-devices-devicemanagementscript-assign.md)|<span data-ttu-id="52b64-129">なし</span><span class="sxs-lookup"><span data-stu-id="52b64-129">None</span></span>|<span data-ttu-id="52b64-130">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="52b64-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="52b64-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52b64-131">Properties</span></span>
|<span data-ttu-id="52b64-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52b64-132">Property</span></span>|<span data-ttu-id="52b64-133">型</span><span class="sxs-lookup"><span data-stu-id="52b64-133">Type</span></span>|<span data-ttu-id="52b64-134">説明</span><span class="sxs-lookup"><span data-stu-id="52b64-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52b64-135">id</span><span class="sxs-lookup"><span data-stu-id="52b64-135">id</span></span>|<span data-ttu-id="52b64-136">文字列</span><span class="sxs-lookup"><span data-stu-id="52b64-136">String</span></span>|<span data-ttu-id="52b64-137">デバイス管理スクリプトの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="52b64-137">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="52b64-138">displayName</span><span class="sxs-lookup"><span data-stu-id="52b64-138">displayName</span></span>|<span data-ttu-id="52b64-139">String</span><span class="sxs-lookup"><span data-stu-id="52b64-139">String</span></span>|<span data-ttu-id="52b64-140">デバイス管理スクリプトの名前。</span><span class="sxs-lookup"><span data-stu-id="52b64-140">Name of the device management script.</span></span>|
|<span data-ttu-id="52b64-141">説明</span><span class="sxs-lookup"><span data-stu-id="52b64-141">description</span></span>|<span data-ttu-id="52b64-142">文字列</span><span class="sxs-lookup"><span data-stu-id="52b64-142">String</span></span>|<span data-ttu-id="52b64-143">デバイス管理スクリプトの省略可能な説明です。</span><span class="sxs-lookup"><span data-stu-id="52b64-143">Optional description for the device management script.</span></span>|
|<span data-ttu-id="52b64-144">runSchedule</span><span class="sxs-lookup"><span data-stu-id="52b64-144">runSchedule</span></span>|[<span data-ttu-id="52b64-145">runSchedule</span><span class="sxs-lookup"><span data-stu-id="52b64-145">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="52b64-146">スクリプトを実行する間隔を指定します。</span><span class="sxs-lookup"><span data-stu-id="52b64-146">The interval for script to run.</span></span> <span data-ttu-id="52b64-147">定義されていない場合、スクリプトは1回だけ実行されます。</span><span class="sxs-lookup"><span data-stu-id="52b64-147">If not defined the script will run once</span></span>|
|<span data-ttu-id="52b64-148">scriptcontent</span><span class="sxs-lookup"><span data-stu-id="52b64-148">scriptContent</span></span>|<span data-ttu-id="52b64-149">Binary</span><span class="sxs-lookup"><span data-stu-id="52b64-149">Binary</span></span>|<span data-ttu-id="52b64-150">スクリプトの内容。</span><span class="sxs-lookup"><span data-stu-id="52b64-150">The script content.</span></span>|
|<span data-ttu-id="52b64-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="52b64-151">createdDateTime</span></span>|<span data-ttu-id="52b64-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52b64-152">DateTimeOffset</span></span>|<span data-ttu-id="52b64-153">デバイス管理スクリプトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="52b64-153">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="52b64-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="52b64-154">lastModifiedDateTime</span></span>|<span data-ttu-id="52b64-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52b64-155">DateTimeOffset</span></span>|<span data-ttu-id="52b64-156">デバイス管理スクリプトが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="52b64-156">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="52b64-157">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="52b64-157">runAsAccount</span></span>|[<span data-ttu-id="52b64-158">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="52b64-158">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="52b64-159">デバイス管理スクリプトを実行する実行コンテキストの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="52b64-159">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="52b64-160">使用可能な値は、`system`、`user` です。</span><span class="sxs-lookup"><span data-stu-id="52b64-160">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="52b64-161">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="52b64-161">enforceSignatureCheck</span></span>|<span data-ttu-id="52b64-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="52b64-162">Boolean</span></span>|<span data-ttu-id="52b64-163">スクリプト署名をチェックする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="52b64-163">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="52b64-164">fileName</span><span class="sxs-lookup"><span data-stu-id="52b64-164">fileName</span></span>|<span data-ttu-id="52b64-165">String</span><span class="sxs-lookup"><span data-stu-id="52b64-165">String</span></span>|<span data-ttu-id="52b64-166">スクリプトファイル名。</span><span class="sxs-lookup"><span data-stu-id="52b64-166">Script file name.</span></span>|
|<span data-ttu-id="52b64-167">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="52b64-167">roleScopeTagIds</span></span>|<span data-ttu-id="52b64-168">String コレクション</span><span class="sxs-lookup"><span data-stu-id="52b64-168">String collection</span></span>|<span data-ttu-id="52b64-169">この powershellscript インスタンスの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="52b64-169">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="52b64-170">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="52b64-170">runAs32Bit</span></span>|<span data-ttu-id="52b64-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="52b64-171">Boolean</span></span>|<span data-ttu-id="52b64-172">PowerShell スクリプトを32ビットとして実行する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="52b64-172">A value indicating whether the PowerShell script should run as 32-bit</span></span>|

## <a name="relationships"></a><span data-ttu-id="52b64-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="52b64-173">Relationships</span></span>
|<span data-ttu-id="52b64-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="52b64-174">Relationship</span></span>|<span data-ttu-id="52b64-175">型</span><span class="sxs-lookup"><span data-stu-id="52b64-175">Type</span></span>|<span data-ttu-id="52b64-176">説明</span><span class="sxs-lookup"><span data-stu-id="52b64-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52b64-177">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="52b64-177">groupAssignments</span></span>|<span data-ttu-id="52b64-178">[devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="52b64-178">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="52b64-179">デバイス管理スクリプトのグループ割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="52b64-179">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="52b64-180">assignments</span><span class="sxs-lookup"><span data-stu-id="52b64-180">assignments</span></span>|<span data-ttu-id="52b64-181">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="52b64-181">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="52b64-182">デバイス管理スクリプトのグループ割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="52b64-182">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="52b64-183">runSummary</span><span class="sxs-lookup"><span data-stu-id="52b64-183">runSummary</span></span>|[<span data-ttu-id="52b64-184">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="52b64-184">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="52b64-185">デバイス管理スクリプトのサマリーを実行します。</span><span class="sxs-lookup"><span data-stu-id="52b64-185">Run summary for device management script.</span></span>|
|<span data-ttu-id="52b64-186">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="52b64-186">deviceRunStates</span></span>|<span data-ttu-id="52b64-187">[devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="52b64-187">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="52b64-188">すべてのデバイスでこのスクリプトの実行状態のリスト。</span><span class="sxs-lookup"><span data-stu-id="52b64-188">List of run states for this script across all devices.</span></span>|
|<span data-ttu-id="52b64-189">userRunStates</span><span class="sxs-lookup"><span data-stu-id="52b64-189">userRunStates</span></span>|<span data-ttu-id="52b64-190">[devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="52b64-190">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="52b64-191">すべてのユーザーにわたるこのスクリプトの実行状態のリスト。</span><span class="sxs-lookup"><span data-stu-id="52b64-191">List of run states for this script across all users.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52b64-192">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="52b64-192">JSON Representation</span></span>
<span data-ttu-id="52b64-193">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="52b64-193">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "fileName": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "runAs32Bit": true
}
```




