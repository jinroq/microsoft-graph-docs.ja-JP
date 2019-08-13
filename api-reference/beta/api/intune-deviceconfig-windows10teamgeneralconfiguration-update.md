---
title: Update windows10TeamGeneralConfiguration
description: windows10TeamGeneralConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 339c01600a4af2ce0a18c7fa62e13934b2f3ddf7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36344897"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="98275-103">Update windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="98275-103">Update windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="98275-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98275-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98275-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="98275-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98275-106">[windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="98275-106">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98275-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="98275-107">Prerequisites</span></span>
<span data-ttu-id="98275-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98275-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98275-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="98275-110">Permission type</span></span>|<span data-ttu-id="98275-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="98275-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98275-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="98275-112">Delegated (work or school account)</span></span>|<span data-ttu-id="98275-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98275-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="98275-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="98275-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98275-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98275-115">Not supported.</span></span>|
|<span data-ttu-id="98275-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="98275-116">Application</span></span>|<span data-ttu-id="98275-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98275-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98275-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="98275-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="98275-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="98275-119">Request headers</span></span>
|<span data-ttu-id="98275-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="98275-120">Header</span></span>|<span data-ttu-id="98275-121">値</span><span class="sxs-lookup"><span data-stu-id="98275-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98275-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="98275-122">Authorization</span></span>|<span data-ttu-id="98275-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="98275-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98275-124">承諾</span><span class="sxs-lookup"><span data-stu-id="98275-124">Accept</span></span>|<span data-ttu-id="98275-125">application/json</span><span class="sxs-lookup"><span data-stu-id="98275-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98275-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="98275-126">Request body</span></span>
<span data-ttu-id="98275-127">要求本文で、[windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="98275-127">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="98275-128">次の表に、[windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="98275-128">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="98275-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98275-129">Property</span></span>|<span data-ttu-id="98275-130">型</span><span class="sxs-lookup"><span data-stu-id="98275-130">Type</span></span>|<span data-ttu-id="98275-131">説明</span><span class="sxs-lookup"><span data-stu-id="98275-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98275-132">id</span><span class="sxs-lookup"><span data-stu-id="98275-132">id</span></span>|<span data-ttu-id="98275-133">文字列</span><span class="sxs-lookup"><span data-stu-id="98275-133">String</span></span>|<span data-ttu-id="98275-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="98275-134">Key of the entity.</span></span> <span data-ttu-id="98275-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98275-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98275-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="98275-136">lastModifiedDateTime</span></span>|<span data-ttu-id="98275-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98275-137">DateTimeOffset</span></span>|<span data-ttu-id="98275-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="98275-138">DateTime the object was last modified.</span></span> <span data-ttu-id="98275-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98275-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98275-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="98275-140">roleScopeTagIds</span></span>|<span data-ttu-id="98275-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="98275-141">String collection</span></span>|<span data-ttu-id="98275-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="98275-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="98275-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98275-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98275-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="98275-144">supportsScopeTags</span></span>|<span data-ttu-id="98275-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="98275-145">Boolean</span></span>|<span data-ttu-id="98275-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="98275-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="98275-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="98275-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="98275-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="98275-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="98275-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="98275-149">This property is read-only.</span></span> <span data-ttu-id="98275-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98275-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98275-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="98275-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="98275-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="98275-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="98275-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="98275-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="98275-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98275-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98275-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="98275-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="98275-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="98275-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="98275-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="98275-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="98275-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98275-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98275-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="98275-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="98275-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="98275-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="98275-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="98275-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="98275-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98275-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98275-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="98275-163">createdDateTime</span></span>|<span data-ttu-id="98275-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98275-164">DateTimeOffset</span></span>|<span data-ttu-id="98275-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="98275-165">DateTime the object was created.</span></span> <span data-ttu-id="98275-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98275-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98275-167">description</span><span class="sxs-lookup"><span data-stu-id="98275-167">description</span></span>|<span data-ttu-id="98275-168">String</span><span class="sxs-lookup"><span data-stu-id="98275-168">String</span></span>|<span data-ttu-id="98275-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="98275-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="98275-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98275-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98275-171">displayName</span><span class="sxs-lookup"><span data-stu-id="98275-171">displayName</span></span>|<span data-ttu-id="98275-172">String</span><span class="sxs-lookup"><span data-stu-id="98275-172">String</span></span>|<span data-ttu-id="98275-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="98275-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="98275-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98275-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98275-175">version</span><span class="sxs-lookup"><span data-stu-id="98275-175">version</span></span>|<span data-ttu-id="98275-176">Int32</span><span class="sxs-lookup"><span data-stu-id="98275-176">Int32</span></span>|<span data-ttu-id="98275-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="98275-177">Version of the device configuration.</span></span> <span data-ttu-id="98275-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="98275-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98275-179">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="98275-179">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="98275-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="98275-180">Boolean</span></span>|<span data-ttu-id="98275-181">Azure Operational Insights をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="98275-181">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="98275-182">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="98275-182">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="98275-183">String</span><span class="sxs-lookup"><span data-stu-id="98275-183">String</span></span>|<span data-ttu-id="98275-184">Azure Operational Insights のワークスペース ID。</span><span class="sxs-lookup"><span data-stu-id="98275-184">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="98275-185">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="98275-185">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="98275-186">String</span><span class="sxs-lookup"><span data-stu-id="98275-186">String</span></span>|<span data-ttu-id="98275-187">Azure Operational Insights のワークスペース キー。</span><span class="sxs-lookup"><span data-stu-id="98275-187">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="98275-188">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="98275-188">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="98275-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="98275-189">Boolean</span></span>|<span data-ttu-id="98275-190">投影を開始するたびに、接続アプリを自動的に起動するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="98275-190">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="98275-191">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="98275-191">maintenanceWindowBlocked</span></span>|<span data-ttu-id="98275-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="98275-192">Boolean</span></span>|<span data-ttu-id="98275-193">デバイス更新のメンテナンス ウィンドウの設定をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="98275-193">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="98275-194">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="98275-194">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="98275-195">Int32</span><span class="sxs-lookup"><span data-stu-id="98275-195">Int32</span></span>|<span data-ttu-id="98275-196">デバイス更新のためのメンテナンス期間の長さ (時間)。</span><span class="sxs-lookup"><span data-stu-id="98275-196">Maintenance window duration for device updates.</span></span> <span data-ttu-id="98275-197">有効な値は 0 から 5 までです</span><span class="sxs-lookup"><span data-stu-id="98275-197">Valid values 0 to 5</span></span>|
|<span data-ttu-id="98275-198">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="98275-198">maintenanceWindowStartTime</span></span>|<span data-ttu-id="98275-199">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="98275-199">TimeOfDay</span></span>|<span data-ttu-id="98275-200">デバイス更新のためのメンテナンス期間の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="98275-200">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="98275-201">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="98275-201">miracastChannel</span></span>|[<span data-ttu-id="98275-202">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="98275-202">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="98275-203">チャネル。</span><span class="sxs-lookup"><span data-stu-id="98275-203">The channel.</span></span> <span data-ttu-id="98275-204">可能な値は、`userDefined`、`one`、`two`、`three`、`four`、`five`、`six`、`seven`、`eight`、`nine`、`ten`、`eleven`、`thirtySix`、`forty`、`fortyFour`、`fortyEight`、`oneHundredFortyNine`、`oneHundredFiftyThree`、`oneHundredFiftySeven`、`oneHundredSixtyOne`、`oneHundredSixtyFive` です。</span><span class="sxs-lookup"><span data-stu-id="98275-204">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="98275-205">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="98275-205">miracastBlocked</span></span>|<span data-ttu-id="98275-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="98275-206">Boolean</span></span>|<span data-ttu-id="98275-207">ワイヤレス投影をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="98275-207">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="98275-208">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="98275-208">miracastRequirePin</span></span>|<span data-ttu-id="98275-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="98275-209">Boolean</span></span>|<span data-ttu-id="98275-210">ワイヤレス投影の pin が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="98275-210">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="98275-211">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="98275-211">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="98275-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="98275-212">Boolean</span></span>|<span data-ttu-id="98275-213">スタート メニューで [会議とファイル] 機能を無効にするかどうかを指定します。この機能は、サインイン ユーザーの会議とファイルを Office 365 から表示します。</span><span class="sxs-lookup"><span data-stu-id="98275-213">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="98275-214">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="98275-214">settingsBlockSessionResume</span></span>|<span data-ttu-id="98275-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="98275-215">Boolean</span></span>|<span data-ttu-id="98275-216">セッションがタイムアウトになった際にセッションを再開する機能を許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="98275-216">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="98275-217">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="98275-217">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="98275-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="98275-218">Boolean</span></span>|<span data-ttu-id="98275-219">スケジュールされている会議の招待者をサインイン ダイアログに自動入力する機能を無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="98275-219">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="98275-220">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="98275-220">settingsDefaultVolume</span></span>|<span data-ttu-id="98275-221">Int32</span><span class="sxs-lookup"><span data-stu-id="98275-221">Int32</span></span>|<span data-ttu-id="98275-222">新しいセッションの既定のボリューム値を指定します。</span><span class="sxs-lookup"><span data-stu-id="98275-222">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="98275-223">許可される値は、0 から 100 までです。</span><span class="sxs-lookup"><span data-stu-id="98275-223">Permitted values are 0-100.</span></span> <span data-ttu-id="98275-224">既定値は 45 です。</span><span class="sxs-lookup"><span data-stu-id="98275-224">The default is 45.</span></span> <span data-ttu-id="98275-225">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="98275-225">Valid values 0 to 100</span></span>|
|<span data-ttu-id="98275-226">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="98275-226">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="98275-227">Int32</span><span class="sxs-lookup"><span data-stu-id="98275-227">Int32</span></span>|<span data-ttu-id="98275-228">ハブ スクリーンがオフになるまでの分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="98275-228">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="98275-229">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="98275-229">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="98275-230">Int32</span><span class="sxs-lookup"><span data-stu-id="98275-230">Int32</span></span>|<span data-ttu-id="98275-231">セッションがタイムアウトになるまでの分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="98275-231">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="98275-232">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="98275-232">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="98275-233">Int32</span><span class="sxs-lookup"><span data-stu-id="98275-233">Int32</span></span>|<span data-ttu-id="98275-234">ハブがスリープ モードになるまでの分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="98275-234">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="98275-235">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="98275-235">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="98275-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="98275-236">Boolean</span></span>|<span data-ttu-id="98275-237">ユーザーが入室した際に、ようこそ画面が自動的に起動するのをブロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="98275-237">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="98275-238">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="98275-238">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="98275-239">String</span><span class="sxs-lookup"><span data-stu-id="98275-239">String</span></span>|<span data-ttu-id="98275-240">ようこそ画面の背景画像の URL。</span><span class="sxs-lookup"><span data-stu-id="98275-240">The welcome screen background image URL.</span></span> <span data-ttu-id="98275-241">URL は HTTPS プロトコルを使用し、PNG 画像を返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="98275-241">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="98275-242">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="98275-242">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="98275-243">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="98275-243">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="98275-244">表示される、ようこそ画面の会議情報。</span><span class="sxs-lookup"><span data-stu-id="98275-244">The welcome screen meeting information shown.</span></span> <span data-ttu-id="98275-245">可能な値は、`userDefined`、`showOrganizerAndTimeOnly`、`showOrganizerAndTimeAndSubject` です。</span><span class="sxs-lookup"><span data-stu-id="98275-245">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="98275-246">応答</span><span class="sxs-lookup"><span data-stu-id="98275-246">Response</span></span>
<span data-ttu-id="98275-247">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="98275-247">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98275-248">例</span><span class="sxs-lookup"><span data-stu-id="98275-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="98275-249">要求</span><span class="sxs-lookup"><span data-stu-id="98275-249">Request</span></span>
<span data-ttu-id="98275-250">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="98275-250">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2015

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```

### <a name="response"></a><span data-ttu-id="98275-251">応答</span><span class="sxs-lookup"><span data-stu-id="98275-251">Response</span></span>
<span data-ttu-id="98275-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="98275-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2187

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```






