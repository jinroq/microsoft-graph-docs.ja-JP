---
title: deviceManagementScript リソースの種類
description: Intune は、10 の登録されている windows Azure Active Directory が参加しているデバイスで、Powershell スクリプトを実行する機能を顧客に提供します。 スクリプトは、1 回だけまたは定期的に実行できます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4fda826ec8033cd51ad4dd13dbc5b523a21e9e3a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412528"
---
# <a name="devicemanagementscript-resource-type"></a><span data-ttu-id="783af-104">deviceManagementScript リソースの種類</span><span class="sxs-lookup"><span data-stu-id="783af-104">deviceManagementScript resource type</span></span>

> <span data-ttu-id="783af-105">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="783af-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="783af-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="783af-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="783af-107">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="783af-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="783af-108">Intune は、10 の登録されている windows Azure Active Directory が参加しているデバイスで、Powershell スクリプトを実行する機能を顧客に提供します。</span><span class="sxs-lookup"><span data-stu-id="783af-108">Intune will provide customer the ability to run their Powershell scripts on the enrolled windows 10 Azure Active Directory joined devices.</span></span> <span data-ttu-id="783af-109">スクリプトは、1 回だけまたは定期的に実行できます。</span><span class="sxs-lookup"><span data-stu-id="783af-109">The script can be run once or periodically.</span></span>

## <a name="methods"></a><span data-ttu-id="783af-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="783af-110">Methods</span></span>
|<span data-ttu-id="783af-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="783af-111">Method</span></span>|<span data-ttu-id="783af-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="783af-112">Return Type</span></span>|<span data-ttu-id="783af-113">説明</span><span class="sxs-lookup"><span data-stu-id="783af-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="783af-114">リスト deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="783af-114">List deviceManagementScripts</span></span>](../api/intune-devices-devicemanagementscript-list.md)|<span data-ttu-id="783af-115">[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="783af-115">[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) collection</span></span>|<span data-ttu-id="783af-116">[DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="783af-116">List properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects.</span></span>|
|[<span data-ttu-id="783af-117">DeviceManagementScript を取得します。</span><span class="sxs-lookup"><span data-stu-id="783af-117">Get deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-get.md)|[<span data-ttu-id="783af-118">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="783af-118">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="783af-119">[DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="783af-119">Read properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="783af-120">DeviceManagementScript を作成します。</span><span class="sxs-lookup"><span data-stu-id="783af-120">Create deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-create.md)|[<span data-ttu-id="783af-121">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="783af-121">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="783af-122">新しい[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="783af-122">Create a new [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="783af-123">DeviceManagementScript を削除します。</span><span class="sxs-lookup"><span data-stu-id="783af-123">Delete deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-delete.md)|<span data-ttu-id="783af-124">なし</span><span class="sxs-lookup"><span data-stu-id="783af-124">None</span></span>|<span data-ttu-id="783af-125">の[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="783af-125">Deletes a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>|
|[<span data-ttu-id="783af-126">DeviceManagementScript を更新します。</span><span class="sxs-lookup"><span data-stu-id="783af-126">Update deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-update.md)|[<span data-ttu-id="783af-127">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="783af-127">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="783af-128">[DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="783af-128">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="783af-129">assign action</span><span class="sxs-lookup"><span data-stu-id="783af-129">assign action</span></span>](../api/intune-devices-devicemanagementscript-assign.md)|<span data-ttu-id="783af-130">なし</span><span class="sxs-lookup"><span data-stu-id="783af-130">None</span></span>|<span data-ttu-id="783af-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="783af-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="783af-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="783af-132">Properties</span></span>
|<span data-ttu-id="783af-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="783af-133">Property</span></span>|<span data-ttu-id="783af-134">型</span><span class="sxs-lookup"><span data-stu-id="783af-134">Type</span></span>|<span data-ttu-id="783af-135">説明</span><span class="sxs-lookup"><span data-stu-id="783af-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="783af-136">id</span><span class="sxs-lookup"><span data-stu-id="783af-136">id</span></span>|<span data-ttu-id="783af-137">String</span><span class="sxs-lookup"><span data-stu-id="783af-137">String</span></span>|<span data-ttu-id="783af-138">デバイス管理スクリプト用の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="783af-138">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="783af-139">displayName</span><span class="sxs-lookup"><span data-stu-id="783af-139">displayName</span></span>|<span data-ttu-id="783af-140">String</span><span class="sxs-lookup"><span data-stu-id="783af-140">String</span></span>|<span data-ttu-id="783af-141">デバイスの管理スクリプトの名前です。</span><span class="sxs-lookup"><span data-stu-id="783af-141">Name of the device management script.</span></span>|
|<span data-ttu-id="783af-142">説明</span><span class="sxs-lookup"><span data-stu-id="783af-142">description</span></span>|<span data-ttu-id="783af-143">String</span><span class="sxs-lookup"><span data-stu-id="783af-143">String</span></span>|<span data-ttu-id="783af-144">デバイスの管理スクリプトのオプションの説明です。</span><span class="sxs-lookup"><span data-stu-id="783af-144">Optional description for the device management script.</span></span>|
|<span data-ttu-id="783af-145">runSchedule</span><span class="sxs-lookup"><span data-stu-id="783af-145">runSchedule</span></span>|[<span data-ttu-id="783af-146">runSchedule</span><span class="sxs-lookup"><span data-stu-id="783af-146">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="783af-147">スクリプトを実行する間隔です。</span><span class="sxs-lookup"><span data-stu-id="783af-147">The interval for script to run.</span></span> <span data-ttu-id="783af-148">定義されていないスクリプトは実行 1 回</span><span class="sxs-lookup"><span data-stu-id="783af-148">If not defined the script will run once</span></span>|
|<span data-ttu-id="783af-149">scriptContent</span><span class="sxs-lookup"><span data-stu-id="783af-149">scriptContent</span></span>|<span data-ttu-id="783af-150">Binary</span><span class="sxs-lookup"><span data-stu-id="783af-150">Binary</span></span>|<span data-ttu-id="783af-151">スクリプトの内容。</span><span class="sxs-lookup"><span data-stu-id="783af-151">The script content.</span></span>|
|<span data-ttu-id="783af-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="783af-152">createdDateTime</span></span>|<span data-ttu-id="783af-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="783af-153">DateTimeOffset</span></span>|<span data-ttu-id="783af-154">デバイス管理スクリプトが作成された日時です。</span><span class="sxs-lookup"><span data-stu-id="783af-154">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="783af-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="783af-155">lastModifiedDateTime</span></span>|<span data-ttu-id="783af-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="783af-156">DateTimeOffset</span></span>|<span data-ttu-id="783af-157">日付と時刻、デバイス管理のスクリプトが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="783af-157">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="783af-158">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="783af-158">runAsAccount</span></span>|[<span data-ttu-id="783af-159">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="783af-159">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="783af-160">デバイス管理のスクリプトで実行される実行コンテキストの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="783af-160">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="783af-161">使用可能な値は、`system`、`user` です。</span><span class="sxs-lookup"><span data-stu-id="783af-161">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="783af-162">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="783af-162">enforceSignatureCheck</span></span>|<span data-ttu-id="783af-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="783af-163">Boolean</span></span>|<span data-ttu-id="783af-164">スクリプト署名をチェックする必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="783af-164">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="783af-165">fileName</span><span class="sxs-lookup"><span data-stu-id="783af-165">fileName</span></span>|<span data-ttu-id="783af-166">String</span><span class="sxs-lookup"><span data-stu-id="783af-166">String</span></span>|<span data-ttu-id="783af-167">スクリプト ファイルの名前です。</span><span class="sxs-lookup"><span data-stu-id="783af-167">Script file name.</span></span>|
|<span data-ttu-id="783af-168">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="783af-168">roleScopeTagIds</span></span>|<span data-ttu-id="783af-169">String コレクション</span><span class="sxs-lookup"><span data-stu-id="783af-169">String collection</span></span>|<span data-ttu-id="783af-170">この PowerShellScript インスタンスのスコープのタグ Id のリストです。</span><span class="sxs-lookup"><span data-stu-id="783af-170">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="783af-171">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="783af-171">runAs32Bit</span></span>|<span data-ttu-id="783af-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="783af-172">Boolean</span></span>|<span data-ttu-id="783af-173">PowerShell スクリプトが 32 ビットとして実行する必要があるかどうかを示す値</span><span class="sxs-lookup"><span data-stu-id="783af-173">A value indicating whether the PowerShell script should run as 32-bit</span></span>|

## <a name="relationships"></a><span data-ttu-id="783af-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="783af-174">Relationships</span></span>
|<span data-ttu-id="783af-175">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="783af-175">Relationship</span></span>|<span data-ttu-id="783af-176">型</span><span class="sxs-lookup"><span data-stu-id="783af-176">Type</span></span>|<span data-ttu-id="783af-177">説明</span><span class="sxs-lookup"><span data-stu-id="783af-177">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="783af-178">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="783af-178">groupAssignments</span></span>|<span data-ttu-id="783af-179">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="783af-179">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="783af-180">一連のデバイスの管理スクリプトの割り当てをグループ化します。</span><span class="sxs-lookup"><span data-stu-id="783af-180">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="783af-181">assignments</span><span class="sxs-lookup"><span data-stu-id="783af-181">assignments</span></span>|<span data-ttu-id="783af-182">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="783af-182">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="783af-183">一連のデバイスの管理スクリプトの割り当てをグループ化します。</span><span class="sxs-lookup"><span data-stu-id="783af-183">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="783af-184">runSummary</span><span class="sxs-lookup"><span data-stu-id="783af-184">runSummary</span></span>|[<span data-ttu-id="783af-185">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="783af-185">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="783af-186">概要デバイス管理のスクリプトを実行します。</span><span class="sxs-lookup"><span data-stu-id="783af-186">Run summary for device management script.</span></span>|
|<span data-ttu-id="783af-187">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="783af-187">deviceRunStates</span></span>|<span data-ttu-id="783af-188">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="783af-188">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="783af-189">すべてのデバイスでは、このスクリプトの実行状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="783af-189">List of run states for this script across all devices.</span></span>|
|<span data-ttu-id="783af-190">userRunStates</span><span class="sxs-lookup"><span data-stu-id="783af-190">userRunStates</span></span>|<span data-ttu-id="783af-191">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="783af-191">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="783af-192">すべてのユーザーにこのスクリプトの実行状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="783af-192">List of run states for this script across all users.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="783af-193">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="783af-193">JSON Representation</span></span>
<span data-ttu-id="783af-194">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="783af-194">Here is a JSON representation of the resource.</span></span>
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




