---
title: Update windows10TeamGeneralConfiguration
description: windows10TeamGeneralConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 03b1c264207c79ccc06bcbd52b9b239fe0ed4f3a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329786"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="e0fc5-103">Update windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0fc5-103">Update windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="e0fc5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0fc5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0fc5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0fc5-107">[windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-107">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0fc5-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e0fc5-108">Prerequisites</span></span>
<span data-ttu-id="e0fc5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0fc5-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e0fc5-111">Permission type</span></span>|<span data-ttu-id="e0fc5-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e0fc5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0fc5-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e0fc5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0fc5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0fc5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e0fc5-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e0fc5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0fc5-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-116">Not supported.</span></span>|
|<span data-ttu-id="e0fc5-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e0fc5-117">Application</span></span>|<span data-ttu-id="e0fc5-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0fc5-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e0fc5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e0fc5-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0fc5-120">Request headers</span></span>
|<span data-ttu-id="e0fc5-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0fc5-121">Header</span></span>|<span data-ttu-id="e0fc5-122">値</span><span class="sxs-lookup"><span data-stu-id="e0fc5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0fc5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0fc5-123">Authorization</span></span>|<span data-ttu-id="e0fc5-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0fc5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e0fc5-125">Accept</span></span>|<span data-ttu-id="e0fc5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0fc5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0fc5-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e0fc5-127">Request body</span></span>
<span data-ttu-id="e0fc5-128">要求本文で、[windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-128">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="e0fc5-129">次の表に、[windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-129">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="e0fc5-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0fc5-130">Property</span></span>|<span data-ttu-id="e0fc5-131">種類</span><span class="sxs-lookup"><span data-stu-id="e0fc5-131">Type</span></span>|<span data-ttu-id="e0fc5-132">説明</span><span class="sxs-lookup"><span data-stu-id="e0fc5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0fc5-133">ID</span><span class="sxs-lookup"><span data-stu-id="e0fc5-133">id</span></span>|<span data-ttu-id="e0fc5-134">String</span><span class="sxs-lookup"><span data-stu-id="e0fc5-134">String</span></span>|<span data-ttu-id="e0fc5-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-135">Key of the entity.</span></span> <span data-ttu-id="e0fc5-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e0fc5-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0fc5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0fc5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e0fc5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0fc5-138">DateTimeOffset</span></span>|<span data-ttu-id="e0fc5-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e0fc5-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e0fc5-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0fc5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e0fc5-141">roleScopeTagIds</span></span>|<span data-ttu-id="e0fc5-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e0fc5-142">String collection</span></span>|<span data-ttu-id="e0fc5-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e0fc5-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e0fc5-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0fc5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e0fc5-145">supportsScopeTags</span></span>|<span data-ttu-id="e0fc5-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="e0fc5-146">Boolean</span></span>|<span data-ttu-id="e0fc5-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e0fc5-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e0fc5-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e0fc5-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-150">This property is read-only.</span></span> <span data-ttu-id="e0fc5-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e0fc5-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0fc5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0fc5-152">createdDateTime</span></span>|<span data-ttu-id="e0fc5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0fc5-153">DateTimeOffset</span></span>|<span data-ttu-id="e0fc5-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-154">DateTime the object was created.</span></span> <span data-ttu-id="e0fc5-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e0fc5-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0fc5-156">説明</span><span class="sxs-lookup"><span data-stu-id="e0fc5-156">description</span></span>|<span data-ttu-id="e0fc5-157">String</span><span class="sxs-lookup"><span data-stu-id="e0fc5-157">String</span></span>|<span data-ttu-id="e0fc5-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e0fc5-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e0fc5-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0fc5-160">displayName</span><span class="sxs-lookup"><span data-stu-id="e0fc5-160">displayName</span></span>|<span data-ttu-id="e0fc5-161">String</span><span class="sxs-lookup"><span data-stu-id="e0fc5-161">String</span></span>|<span data-ttu-id="e0fc5-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e0fc5-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e0fc5-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0fc5-164">version</span><span class="sxs-lookup"><span data-stu-id="e0fc5-164">version</span></span>|<span data-ttu-id="e0fc5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e0fc5-165">Int32</span></span>|<span data-ttu-id="e0fc5-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-166">Version of the device configuration.</span></span> <span data-ttu-id="e0fc5-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e0fc5-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0fc5-168">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="e0fc5-168">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="e0fc5-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0fc5-169">Boolean</span></span>|<span data-ttu-id="e0fc5-170">Azure Operational Insights をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-170">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="e0fc5-171">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="e0fc5-171">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="e0fc5-172">String</span><span class="sxs-lookup"><span data-stu-id="e0fc5-172">String</span></span>|<span data-ttu-id="e0fc5-173">Azure Operational Insights のワークスペース ID。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-173">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="e0fc5-174">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="e0fc5-174">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="e0fc5-175">String</span><span class="sxs-lookup"><span data-stu-id="e0fc5-175">String</span></span>|<span data-ttu-id="e0fc5-176">Azure Operational Insights のワークスペース キー。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-176">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="e0fc5-177">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="e0fc5-177">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="e0fc5-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0fc5-178">Boolean</span></span>|<span data-ttu-id="e0fc5-179">投影を開始するたびに、接続アプリを自動的に起動するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-179">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="e0fc5-180">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="e0fc5-180">maintenanceWindowBlocked</span></span>|<span data-ttu-id="e0fc5-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0fc5-181">Boolean</span></span>|<span data-ttu-id="e0fc5-182">デバイス更新のメンテナンス ウィンドウの設定をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-182">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="e0fc5-183">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="e0fc5-183">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="e0fc5-184">Int32</span><span class="sxs-lookup"><span data-stu-id="e0fc5-184">Int32</span></span>|<span data-ttu-id="e0fc5-185">デバイス更新のためのメンテナンス ウインドウの期間。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-185">Maintenance window duration for device updates.</span></span> <span data-ttu-id="e0fc5-186">有効な値は 0 から 5 までです</span><span class="sxs-lookup"><span data-stu-id="e0fc5-186">Valid values 0 to 5</span></span>|
|<span data-ttu-id="e0fc5-187">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="e0fc5-187">maintenanceWindowStartTime</span></span>|<span data-ttu-id="e0fc5-188">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="e0fc5-188">TimeOfDay</span></span>|<span data-ttu-id="e0fc5-189">デバイス更新のためのメンテナンス ウィンドウの開始時刻。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-189">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="e0fc5-190">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="e0fc5-190">miracastChannel</span></span>|[<span data-ttu-id="e0fc5-191">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="e0fc5-191">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="e0fc5-192">チャネル。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-192">The channel.</span></span> <span data-ttu-id="e0fc5-193">可能な値は、`userDefined`、`one`、`two`、`three`、`four`、`five`、`six`、`seven`、`eight`、`nine`、`ten`、`eleven`、`thirtySix`、`forty`、`fortyFour`、`fortyEight`、`oneHundredFortyNine`、`oneHundredFiftyThree`、`oneHundredFiftySeven`、`oneHundredSixtyOne`、`oneHundredSixtyFive` です。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-193">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="e0fc5-194">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="e0fc5-194">miracastBlocked</span></span>|<span data-ttu-id="e0fc5-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0fc5-195">Boolean</span></span>|<span data-ttu-id="e0fc5-196">ワイヤレス投影をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-196">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="e0fc5-197">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="e0fc5-197">miracastRequirePin</span></span>|<span data-ttu-id="e0fc5-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0fc5-198">Boolean</span></span>|<span data-ttu-id="e0fc5-199">ワイヤレス投影の pin が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-199">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="e0fc5-200">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="e0fc5-200">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="e0fc5-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0fc5-201">Boolean</span></span>|<span data-ttu-id="e0fc5-202">スタート メニューで [会議とファイル] 機能を無効にするかどうかを指定します。この機能は、サインイン ユーザーの会議とファイルを Office 365 から表示します。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-202">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="e0fc5-203">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="e0fc5-203">settingsBlockSessionResume</span></span>|<span data-ttu-id="e0fc5-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0fc5-204">Boolean</span></span>|<span data-ttu-id="e0fc5-205">セッションがタイムアウトになった際にセッションを再開する機能を許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-205">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="e0fc5-206">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="e0fc5-206">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="e0fc5-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0fc5-207">Boolean</span></span>|<span data-ttu-id="e0fc5-208">スケジュールされている会議の招待者をサインイン ダイアログに自動入力する機能を無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-208">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="e0fc5-209">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="e0fc5-209">settingsDefaultVolume</span></span>|<span data-ttu-id="e0fc5-210">Int32</span><span class="sxs-lookup"><span data-stu-id="e0fc5-210">Int32</span></span>|<span data-ttu-id="e0fc5-211">新しいセッションの既定のボリューム値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-211">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="e0fc5-212">許可される値は、0 から 100 までです。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-212">Permitted values are 0-100.</span></span> <span data-ttu-id="e0fc5-213">既定値は 45 です。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-213">The default is 45.</span></span> <span data-ttu-id="e0fc5-214">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="e0fc5-214">Valid values 0 to 100</span></span>|
|<span data-ttu-id="e0fc5-215">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="e0fc5-215">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="e0fc5-216">Int32</span><span class="sxs-lookup"><span data-stu-id="e0fc5-216">Int32</span></span>|<span data-ttu-id="e0fc5-217">ハブ スクリーンがオフになるまでの分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-217">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="e0fc5-218">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="e0fc5-218">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="e0fc5-219">Int32</span><span class="sxs-lookup"><span data-stu-id="e0fc5-219">Int32</span></span>|<span data-ttu-id="e0fc5-220">セッションがタイムアウトになるまでの分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-220">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="e0fc5-221">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="e0fc5-221">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="e0fc5-222">Int32</span><span class="sxs-lookup"><span data-stu-id="e0fc5-222">Int32</span></span>|<span data-ttu-id="e0fc5-223">ハブがスリープ モードになるまでの分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-223">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="e0fc5-224">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="e0fc5-224">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="e0fc5-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0fc5-225">Boolean</span></span>|<span data-ttu-id="e0fc5-226">ユーザーが入室した際に、ようこそ画面が自動的に起動するのをブロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-226">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="e0fc5-227">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="e0fc5-227">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="e0fc5-228">String</span><span class="sxs-lookup"><span data-stu-id="e0fc5-228">String</span></span>|<span data-ttu-id="e0fc5-229">ようこそ画面の背景画像の URL。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-229">The welcome screen background image URL.</span></span> <span data-ttu-id="e0fc5-230">URL は HTTPS プロトコルを使用し、PNG 画像を返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-230">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="e0fc5-231">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="e0fc5-231">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="e0fc5-232">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="e0fc5-232">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="e0fc5-233">表示される、ようこそ画面の会議情報。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-233">The welcome screen meeting information shown.</span></span> <span data-ttu-id="e0fc5-234">可能な値は、`userDefined`、`showOrganizerAndTimeOnly`、`showOrganizerAndTimeAndSubject` です。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-234">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="e0fc5-235">応答</span><span class="sxs-lookup"><span data-stu-id="e0fc5-235">Response</span></span>
<span data-ttu-id="e0fc5-236">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-236">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0fc5-237">例</span><span class="sxs-lookup"><span data-stu-id="e0fc5-237">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0fc5-238">要求</span><span class="sxs-lookup"><span data-stu-id="e0fc5-238">Request</span></span>
<span data-ttu-id="e0fc5-239">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1234

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="e0fc5-240">応答</span><span class="sxs-lookup"><span data-stu-id="e0fc5-240">Response</span></span>
<span data-ttu-id="e0fc5-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e0fc5-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1414

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




