---
title: windows10TeamGeneralConfiguration の作成
description: 新しい windows10TeamGeneralConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: df58cd9c0ee316743b876882cbda57495c8d1cda
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980538"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="3f375-103">windows10TeamGeneralConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="3f375-103">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="3f375-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f375-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f375-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3f375-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f375-106">新しい [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3f375-106">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f375-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3f375-107">Prerequisites</span></span>
<span data-ttu-id="3f375-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f375-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f375-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3f375-110">Permission type</span></span>|<span data-ttu-id="3f375-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3f375-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f375-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3f375-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3f375-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f375-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3f375-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3f375-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f375-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f375-115">Not supported.</span></span>|
|<span data-ttu-id="3f375-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3f375-116">Application</span></span>|<span data-ttu-id="3f375-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f375-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f375-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3f375-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3f375-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f375-119">Request headers</span></span>
|<span data-ttu-id="3f375-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f375-120">Header</span></span>|<span data-ttu-id="3f375-121">値</span><span class="sxs-lookup"><span data-stu-id="3f375-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f375-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f375-122">Authorization</span></span>|<span data-ttu-id="3f375-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3f375-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f375-124">承諾</span><span class="sxs-lookup"><span data-stu-id="3f375-124">Accept</span></span>|<span data-ttu-id="3f375-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3f375-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f375-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3f375-126">Request body</span></span>
<span data-ttu-id="3f375-127">要求本文で、windows10TeamGeneralConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3f375-127">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="3f375-128">次の表に、windows10TeamGeneralConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3f375-128">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="3f375-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f375-129">Property</span></span>|<span data-ttu-id="3f375-130">型</span><span class="sxs-lookup"><span data-stu-id="3f375-130">Type</span></span>|<span data-ttu-id="3f375-131">説明</span><span class="sxs-lookup"><span data-stu-id="3f375-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f375-132">id</span><span class="sxs-lookup"><span data-stu-id="3f375-132">id</span></span>|<span data-ttu-id="3f375-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3f375-133">String</span></span>|<span data-ttu-id="3f375-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3f375-134">Key of the entity.</span></span> <span data-ttu-id="3f375-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f375-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f375-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f375-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3f375-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f375-137">DateTimeOffset</span></span>|<span data-ttu-id="3f375-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="3f375-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3f375-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f375-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f375-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3f375-140">roleScopeTagIds</span></span>|<span data-ttu-id="3f375-141">String collection</span><span class="sxs-lookup"><span data-stu-id="3f375-141">String collection</span></span>|<span data-ttu-id="3f375-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="3f375-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3f375-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f375-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f375-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3f375-144">supportsScopeTags</span></span>|<span data-ttu-id="3f375-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f375-145">Boolean</span></span>|<span data-ttu-id="3f375-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3f375-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3f375-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="3f375-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3f375-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="3f375-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3f375-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="3f375-149">This property is read-only.</span></span> <span data-ttu-id="3f375-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f375-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f375-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f375-151">createdDateTime</span></span>|<span data-ttu-id="3f375-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f375-152">DateTimeOffset</span></span>|<span data-ttu-id="3f375-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="3f375-153">DateTime the object was created.</span></span> <span data-ttu-id="3f375-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f375-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f375-155">description</span><span class="sxs-lookup"><span data-stu-id="3f375-155">description</span></span>|<span data-ttu-id="3f375-156">String</span><span class="sxs-lookup"><span data-stu-id="3f375-156">String</span></span>|<span data-ttu-id="3f375-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="3f375-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3f375-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f375-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f375-159">displayName</span><span class="sxs-lookup"><span data-stu-id="3f375-159">displayName</span></span>|<span data-ttu-id="3f375-160">String</span><span class="sxs-lookup"><span data-stu-id="3f375-160">String</span></span>|<span data-ttu-id="3f375-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="3f375-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3f375-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f375-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f375-163">version</span><span class="sxs-lookup"><span data-stu-id="3f375-163">version</span></span>|<span data-ttu-id="3f375-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3f375-164">Int32</span></span>|<span data-ttu-id="3f375-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="3f375-165">Version of the device configuration.</span></span> <span data-ttu-id="3f375-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f375-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f375-167">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="3f375-167">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="3f375-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f375-168">Boolean</span></span>|<span data-ttu-id="3f375-169">Azure Operational Insights をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3f375-169">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="3f375-170">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="3f375-170">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="3f375-171">String</span><span class="sxs-lookup"><span data-stu-id="3f375-171">String</span></span>|<span data-ttu-id="3f375-172">Azure Operational Insights のワークスペース ID。</span><span class="sxs-lookup"><span data-stu-id="3f375-172">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="3f375-173">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="3f375-173">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="3f375-174">String</span><span class="sxs-lookup"><span data-stu-id="3f375-174">String</span></span>|<span data-ttu-id="3f375-175">Azure Operational Insights のワークスペース キー。</span><span class="sxs-lookup"><span data-stu-id="3f375-175">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="3f375-176">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="3f375-176">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="3f375-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f375-177">Boolean</span></span>|<span data-ttu-id="3f375-178">投影を開始するたびに、接続アプリを自動的に起動するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3f375-178">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="3f375-179">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="3f375-179">maintenanceWindowBlocked</span></span>|<span data-ttu-id="3f375-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f375-180">Boolean</span></span>|<span data-ttu-id="3f375-181">デバイス更新のメンテナンス ウィンドウの設定をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3f375-181">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="3f375-182">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="3f375-182">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="3f375-183">Int32</span><span class="sxs-lookup"><span data-stu-id="3f375-183">Int32</span></span>|<span data-ttu-id="3f375-184">デバイス更新のためのメンテナンス期間の長さ (時間)。</span><span class="sxs-lookup"><span data-stu-id="3f375-184">Maintenance window duration for device updates.</span></span> <span data-ttu-id="3f375-185">有効な値は 0 から 5 までです</span><span class="sxs-lookup"><span data-stu-id="3f375-185">Valid values 0 to 5</span></span>|
|<span data-ttu-id="3f375-186">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="3f375-186">maintenanceWindowStartTime</span></span>|<span data-ttu-id="3f375-187">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="3f375-187">TimeOfDay</span></span>|<span data-ttu-id="3f375-188">デバイス更新のためのメンテナンス期間の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="3f375-188">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="3f375-189">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="3f375-189">miracastChannel</span></span>|[<span data-ttu-id="3f375-190">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="3f375-190">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="3f375-191">チャネル。</span><span class="sxs-lookup"><span data-stu-id="3f375-191">The channel.</span></span> <span data-ttu-id="3f375-192">可能な値は、`userDefined`、`one`、`two`、`three`、`four`、`five`、`six`、`seven`、`eight`、`nine`、`ten`、`eleven`、`thirtySix`、`forty`、`fortyFour`、`fortyEight`、`oneHundredFortyNine`、`oneHundredFiftyThree`、`oneHundredFiftySeven`、`oneHundredSixtyOne`、`oneHundredSixtyFive` です。</span><span class="sxs-lookup"><span data-stu-id="3f375-192">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="3f375-193">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="3f375-193">miracastBlocked</span></span>|<span data-ttu-id="3f375-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f375-194">Boolean</span></span>|<span data-ttu-id="3f375-195">ワイヤレス投影をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3f375-195">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="3f375-196">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="3f375-196">miracastRequirePin</span></span>|<span data-ttu-id="3f375-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f375-197">Boolean</span></span>|<span data-ttu-id="3f375-198">ワイヤレス投影の pin が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3f375-198">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="3f375-199">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="3f375-199">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="3f375-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f375-200">Boolean</span></span>|<span data-ttu-id="3f375-201">スタート メニューで [会議とファイル] 機能を無効にするかどうかを指定します。この機能は、サインイン ユーザーの会議とファイルを Office 365 から表示します。</span><span class="sxs-lookup"><span data-stu-id="3f375-201">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="3f375-202">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="3f375-202">settingsBlockSessionResume</span></span>|<span data-ttu-id="3f375-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f375-203">Boolean</span></span>|<span data-ttu-id="3f375-204">セッションがタイムアウトになった際にセッションを再開する機能を許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3f375-204">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="3f375-205">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="3f375-205">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="3f375-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f375-206">Boolean</span></span>|<span data-ttu-id="3f375-207">スケジュールされている会議の招待者をサインイン ダイアログに自動入力する機能を無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3f375-207">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="3f375-208">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="3f375-208">settingsDefaultVolume</span></span>|<span data-ttu-id="3f375-209">Int32</span><span class="sxs-lookup"><span data-stu-id="3f375-209">Int32</span></span>|<span data-ttu-id="3f375-210">新しいセッションの既定のボリューム値を指定します。</span><span class="sxs-lookup"><span data-stu-id="3f375-210">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="3f375-211">許可される値は、0 から 100 までです。</span><span class="sxs-lookup"><span data-stu-id="3f375-211">Permitted values are 0-100.</span></span> <span data-ttu-id="3f375-212">既定値は 45 です。</span><span class="sxs-lookup"><span data-stu-id="3f375-212">The default is 45.</span></span> <span data-ttu-id="3f375-213">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="3f375-213">Valid values 0 to 100</span></span>|
|<span data-ttu-id="3f375-214">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="3f375-214">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="3f375-215">Int32</span><span class="sxs-lookup"><span data-stu-id="3f375-215">Int32</span></span>|<span data-ttu-id="3f375-216">ハブ スクリーンがオフになるまでの分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="3f375-216">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="3f375-217">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="3f375-217">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="3f375-218">Int32</span><span class="sxs-lookup"><span data-stu-id="3f375-218">Int32</span></span>|<span data-ttu-id="3f375-219">セッションがタイムアウトになるまでの分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="3f375-219">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="3f375-220">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="3f375-220">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="3f375-221">Int32</span><span class="sxs-lookup"><span data-stu-id="3f375-221">Int32</span></span>|<span data-ttu-id="3f375-222">ハブがスリープ モードになるまでの分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="3f375-222">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="3f375-223">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="3f375-223">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="3f375-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f375-224">Boolean</span></span>|<span data-ttu-id="3f375-225">ユーザーが入室した際に、ようこそ画面が自動的に起動するのをブロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3f375-225">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="3f375-226">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="3f375-226">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="3f375-227">String</span><span class="sxs-lookup"><span data-stu-id="3f375-227">String</span></span>|<span data-ttu-id="3f375-228">ようこそ画面の背景画像の URL。</span><span class="sxs-lookup"><span data-stu-id="3f375-228">The welcome screen background image URL.</span></span> <span data-ttu-id="3f375-229">URL は HTTPS プロトコルを使用し、PNG 画像を返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="3f375-229">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="3f375-230">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="3f375-230">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="3f375-231">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="3f375-231">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="3f375-232">表示される、ようこそ画面の会議情報。</span><span class="sxs-lookup"><span data-stu-id="3f375-232">The welcome screen meeting information shown.</span></span> <span data-ttu-id="3f375-233">可能な値は、`userDefined`、`showOrganizerAndTimeOnly`、`showOrganizerAndTimeAndSubject` です。</span><span class="sxs-lookup"><span data-stu-id="3f375-233">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="3f375-234">応答</span><span class="sxs-lookup"><span data-stu-id="3f375-234">Response</span></span>
<span data-ttu-id="3f375-235">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3f375-235">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f375-236">例</span><span class="sxs-lookup"><span data-stu-id="3f375-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f375-237">要求</span><span class="sxs-lookup"><span data-stu-id="3f375-237">Request</span></span>
<span data-ttu-id="3f375-238">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3f375-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1242

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
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

### <a name="response"></a><span data-ttu-id="3f375-239">応答</span><span class="sxs-lookup"><span data-stu-id="3f375-239">Response</span></span>
<span data-ttu-id="3f375-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3f375-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




