---
title: deviceManagementScript リソースの種類
description: Intune は、登録済みの windows 10 Azure Active Directory 参加済みデバイスで Powershell スクリプトを実行する機能をお客様に提供します。 このスクリプトは、一度または定期的に実行できます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d3587bcf683662f64de95eeef435ca59381aa63c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999879"
---
# <a name="devicemanagementscript-resource-type"></a><span data-ttu-id="c082d-104">deviceManagementScript リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c082d-104">deviceManagementScript resource type</span></span>

> <span data-ttu-id="c082d-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c082d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c082d-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c082d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c082d-107">Intune は、登録済みの windows 10 Azure Active Directory 参加済みデバイスで Powershell スクリプトを実行する機能をお客様に提供します。</span><span class="sxs-lookup"><span data-stu-id="c082d-107">Intune will provide customer the ability to run their Powershell scripts on the enrolled windows 10 Azure Active Directory joined devices.</span></span> <span data-ttu-id="c082d-108">このスクリプトは、一度または定期的に実行できます。</span><span class="sxs-lookup"><span data-stu-id="c082d-108">The script can be run once or periodically.</span></span>

## <a name="methods"></a><span data-ttu-id="c082d-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c082d-109">Methods</span></span>
|<span data-ttu-id="c082d-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="c082d-110">Method</span></span>|<span data-ttu-id="c082d-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c082d-111">Return Type</span></span>|<span data-ttu-id="c082d-112">説明</span><span class="sxs-lookup"><span data-stu-id="c082d-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c082d-113">DeviceManagementScripts を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c082d-113">List deviceManagementScripts</span></span>](../api/intune-devices-devicemanagementscript-list.md)|<span data-ttu-id="c082d-114">[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c082d-114">[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) collection</span></span>|<span data-ttu-id="c082d-115">[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c082d-115">List properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects.</span></span>|
|[<span data-ttu-id="c082d-116">DeviceManagementScript の取得</span><span class="sxs-lookup"><span data-stu-id="c082d-116">Get deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-get.md)|[<span data-ttu-id="c082d-117">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="c082d-117">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="c082d-118">[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c082d-118">Read properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="c082d-119">DeviceManagementScript の作成</span><span class="sxs-lookup"><span data-stu-id="c082d-119">Create deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-create.md)|[<span data-ttu-id="c082d-120">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="c082d-120">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="c082d-121">新しい[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c082d-121">Create a new [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="c082d-122">DeviceManagementScript の削除</span><span class="sxs-lookup"><span data-stu-id="c082d-122">Delete deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-delete.md)|<span data-ttu-id="c082d-123">None</span><span class="sxs-lookup"><span data-stu-id="c082d-123">None</span></span>|<span data-ttu-id="c082d-124">[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="c082d-124">Deletes a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>|
|[<span data-ttu-id="c082d-125">DeviceManagementScript の更新</span><span class="sxs-lookup"><span data-stu-id="c082d-125">Update deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-update.md)|[<span data-ttu-id="c082d-126">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="c082d-126">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="c082d-127">[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c082d-127">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="c082d-128">assign アクション</span><span class="sxs-lookup"><span data-stu-id="c082d-128">assign action</span></span>](../api/intune-devices-devicemanagementscript-assign.md)|<span data-ttu-id="c082d-129">なし</span><span class="sxs-lookup"><span data-stu-id="c082d-129">None</span></span>|<span data-ttu-id="c082d-130">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c082d-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c082d-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c082d-131">Properties</span></span>
|<span data-ttu-id="c082d-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c082d-132">Property</span></span>|<span data-ttu-id="c082d-133">型</span><span class="sxs-lookup"><span data-stu-id="c082d-133">Type</span></span>|<span data-ttu-id="c082d-134">説明</span><span class="sxs-lookup"><span data-stu-id="c082d-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c082d-135">id</span><span class="sxs-lookup"><span data-stu-id="c082d-135">id</span></span>|<span data-ttu-id="c082d-136">文字列</span><span class="sxs-lookup"><span data-stu-id="c082d-136">String</span></span>|<span data-ttu-id="c082d-137">デバイス管理スクリプトの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="c082d-137">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="c082d-138">displayName</span><span class="sxs-lookup"><span data-stu-id="c082d-138">displayName</span></span>|<span data-ttu-id="c082d-139">String</span><span class="sxs-lookup"><span data-stu-id="c082d-139">String</span></span>|<span data-ttu-id="c082d-140">デバイス管理スクリプトの名前。</span><span class="sxs-lookup"><span data-stu-id="c082d-140">Name of the device management script.</span></span>|
|<span data-ttu-id="c082d-141">description</span><span class="sxs-lookup"><span data-stu-id="c082d-141">description</span></span>|<span data-ttu-id="c082d-142">String</span><span class="sxs-lookup"><span data-stu-id="c082d-142">String</span></span>|<span data-ttu-id="c082d-143">デバイス管理スクリプトの省略可能な説明です。</span><span class="sxs-lookup"><span data-stu-id="c082d-143">Optional description for the device management script.</span></span>|
|<span data-ttu-id="c082d-144">runSchedule</span><span class="sxs-lookup"><span data-stu-id="c082d-144">runSchedule</span></span>|[<span data-ttu-id="c082d-145">runSchedule</span><span class="sxs-lookup"><span data-stu-id="c082d-145">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="c082d-146">スクリプトを実行する間隔を指定します。</span><span class="sxs-lookup"><span data-stu-id="c082d-146">The interval for script to run.</span></span> <span data-ttu-id="c082d-147">定義されていない場合、スクリプトは1回だけ実行されます。</span><span class="sxs-lookup"><span data-stu-id="c082d-147">If not defined the script will run once</span></span>|
|<span data-ttu-id="c082d-148">scriptContent</span><span class="sxs-lookup"><span data-stu-id="c082d-148">scriptContent</span></span>|<span data-ttu-id="c082d-149">Binary</span><span class="sxs-lookup"><span data-stu-id="c082d-149">Binary</span></span>|<span data-ttu-id="c082d-150">スクリプトの内容。</span><span class="sxs-lookup"><span data-stu-id="c082d-150">The script content.</span></span>|
|<span data-ttu-id="c082d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c082d-151">createdDateTime</span></span>|<span data-ttu-id="c082d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c082d-152">DateTimeOffset</span></span>|<span data-ttu-id="c082d-153">デバイス管理スクリプトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="c082d-153">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="c082d-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c082d-154">lastModifiedDateTime</span></span>|<span data-ttu-id="c082d-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c082d-155">DateTimeOffset</span></span>|<span data-ttu-id="c082d-156">デバイス管理スクリプトが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="c082d-156">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="c082d-157">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="c082d-157">runAsAccount</span></span>|[<span data-ttu-id="c082d-158">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="c082d-158">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="c082d-159">実行コンテキストの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="c082d-159">Indicates the type of execution context.</span></span> <span data-ttu-id="c082d-160">可能な値は、`system`、`user` です。</span><span class="sxs-lookup"><span data-stu-id="c082d-160">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="c082d-161">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="c082d-161">enforceSignatureCheck</span></span>|<span data-ttu-id="c082d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c082d-162">Boolean</span></span>|<span data-ttu-id="c082d-163">スクリプト署名をチェックする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c082d-163">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="c082d-164">fileName</span><span class="sxs-lookup"><span data-stu-id="c082d-164">fileName</span></span>|<span data-ttu-id="c082d-165">String</span><span class="sxs-lookup"><span data-stu-id="c082d-165">String</span></span>|<span data-ttu-id="c082d-166">スクリプトファイル名。</span><span class="sxs-lookup"><span data-stu-id="c082d-166">Script file name.</span></span>|
|<span data-ttu-id="c082d-167">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c082d-167">roleScopeTagIds</span></span>|<span data-ttu-id="c082d-168">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="c082d-168">String collection</span></span>|<span data-ttu-id="c082d-169">この PowerShellScript インスタンスの範囲タグ Id のリスト。</span><span class="sxs-lookup"><span data-stu-id="c082d-169">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="c082d-170">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="c082d-170">runAs32Bit</span></span>|<span data-ttu-id="c082d-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="c082d-171">Boolean</span></span>|<span data-ttu-id="c082d-172">PowerShell スクリプトを32ビットとして実行する必要があるかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="c082d-172">A value indicating whether the PowerShell script should run as 32-bit</span></span>|

## <a name="relationships"></a><span data-ttu-id="c082d-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c082d-173">Relationships</span></span>
|<span data-ttu-id="c082d-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c082d-174">Relationship</span></span>|<span data-ttu-id="c082d-175">型</span><span class="sxs-lookup"><span data-stu-id="c082d-175">Type</span></span>|<span data-ttu-id="c082d-176">説明</span><span class="sxs-lookup"><span data-stu-id="c082d-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c082d-177">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="c082d-177">groupAssignments</span></span>|<span data-ttu-id="c082d-178">[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c082d-178">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="c082d-179">デバイス管理スクリプトのグループ割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="c082d-179">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="c082d-180">assignments</span><span class="sxs-lookup"><span data-stu-id="c082d-180">assignments</span></span>|<span data-ttu-id="c082d-181">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c082d-181">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="c082d-182">デバイス管理スクリプトのグループ割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="c082d-182">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="c082d-183">runSummary</span><span class="sxs-lookup"><span data-stu-id="c082d-183">runSummary</span></span>|[<span data-ttu-id="c082d-184">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="c082d-184">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="c082d-185">デバイス管理スクリプトのサマリーを実行します。</span><span class="sxs-lookup"><span data-stu-id="c082d-185">Run summary for device management script.</span></span>|
|<span data-ttu-id="c082d-186">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="c082d-186">deviceRunStates</span></span>|<span data-ttu-id="c082d-187">[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c082d-187">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="c082d-188">すべてのデバイスでこのスクリプトの実行状態のリスト。</span><span class="sxs-lookup"><span data-stu-id="c082d-188">List of run states for this script across all devices.</span></span>|
|<span data-ttu-id="c082d-189">userRunStates</span><span class="sxs-lookup"><span data-stu-id="c082d-189">userRunStates</span></span>|<span data-ttu-id="c082d-190">[Devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c082d-190">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="c082d-191">すべてのユーザーにわたるこのスクリプトの実行状態のリスト。</span><span class="sxs-lookup"><span data-stu-id="c082d-191">List of run states for this script across all users.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c082d-192">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c082d-192">JSON Representation</span></span>
<span data-ttu-id="c082d-193">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c082d-193">Here is a JSON representation of the resource.</span></span>
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





