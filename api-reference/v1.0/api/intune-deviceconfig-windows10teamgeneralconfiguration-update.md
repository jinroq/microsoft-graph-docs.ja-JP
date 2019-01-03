---
title: Update windows10TeamGeneralConfiguration
description: windows10TeamGeneralConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 283e7211c98899b1c8eb02007c9b0d9b889f8ce5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334490"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="83777-103">Update windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="83777-103">Update windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="83777-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="83777-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83777-105">[windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="83777-105">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83777-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="83777-106">Prerequisites</span></span>
<span data-ttu-id="83777-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83777-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83777-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="83777-109">Permission type</span></span>|<span data-ttu-id="83777-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="83777-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83777-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="83777-111">Delegated (work or school account)</span></span>|<span data-ttu-id="83777-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83777-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="83777-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="83777-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83777-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83777-114">Not supported.</span></span>|
|<span data-ttu-id="83777-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="83777-115">Application</span></span>|<span data-ttu-id="83777-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83777-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83777-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83777-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="83777-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83777-118">Request headers</span></span>
|<span data-ttu-id="83777-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83777-119">Header</span></span>|<span data-ttu-id="83777-120">値</span><span class="sxs-lookup"><span data-stu-id="83777-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83777-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="83777-121">Authorization</span></span>|<span data-ttu-id="83777-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="83777-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83777-123">Accept</span><span class="sxs-lookup"><span data-stu-id="83777-123">Accept</span></span>|<span data-ttu-id="83777-124">application/json</span><span class="sxs-lookup"><span data-stu-id="83777-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83777-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="83777-125">Request body</span></span>
<span data-ttu-id="83777-126">要求本文で、[windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="83777-126">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="83777-127">次の表に、[windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="83777-127">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="83777-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83777-128">Property</span></span>|<span data-ttu-id="83777-129">種類</span><span class="sxs-lookup"><span data-stu-id="83777-129">Type</span></span>|<span data-ttu-id="83777-130">説明</span><span class="sxs-lookup"><span data-stu-id="83777-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83777-131">ID</span><span class="sxs-lookup"><span data-stu-id="83777-131">id</span></span>|<span data-ttu-id="83777-132">String</span><span class="sxs-lookup"><span data-stu-id="83777-132">String</span></span>|<span data-ttu-id="83777-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="83777-133">Key of the entity.</span></span> <span data-ttu-id="83777-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83777-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83777-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83777-135">lastModifiedDateTime</span></span>|<span data-ttu-id="83777-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83777-136">DateTimeOffset</span></span>|<span data-ttu-id="83777-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="83777-137">DateTime the object was last modified.</span></span> <span data-ttu-id="83777-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83777-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83777-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83777-139">createdDateTime</span></span>|<span data-ttu-id="83777-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83777-140">DateTimeOffset</span></span>|<span data-ttu-id="83777-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="83777-141">DateTime the object was created.</span></span> <span data-ttu-id="83777-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83777-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83777-143">説明</span><span class="sxs-lookup"><span data-stu-id="83777-143">description</span></span>|<span data-ttu-id="83777-144">String</span><span class="sxs-lookup"><span data-stu-id="83777-144">String</span></span>|<span data-ttu-id="83777-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="83777-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="83777-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83777-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83777-147">displayName</span><span class="sxs-lookup"><span data-stu-id="83777-147">displayName</span></span>|<span data-ttu-id="83777-148">String</span><span class="sxs-lookup"><span data-stu-id="83777-148">String</span></span>|<span data-ttu-id="83777-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="83777-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="83777-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83777-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83777-151">version</span><span class="sxs-lookup"><span data-stu-id="83777-151">version</span></span>|<span data-ttu-id="83777-152">Int32</span><span class="sxs-lookup"><span data-stu-id="83777-152">Int32</span></span>|<span data-ttu-id="83777-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="83777-153">Version of the device configuration.</span></span> <span data-ttu-id="83777-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83777-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83777-155">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="83777-155">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="83777-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="83777-156">Boolean</span></span>|<span data-ttu-id="83777-157">Azure Operational Insights をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="83777-157">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="83777-158">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="83777-158">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="83777-159">String</span><span class="sxs-lookup"><span data-stu-id="83777-159">String</span></span>|<span data-ttu-id="83777-160">Azure Operational Insights のワークスペース ID。</span><span class="sxs-lookup"><span data-stu-id="83777-160">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="83777-161">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="83777-161">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="83777-162">String</span><span class="sxs-lookup"><span data-stu-id="83777-162">String</span></span>|<span data-ttu-id="83777-163">Azure Operational Insights のワークスペース キー。</span><span class="sxs-lookup"><span data-stu-id="83777-163">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="83777-164">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="83777-164">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="83777-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="83777-165">Boolean</span></span>|<span data-ttu-id="83777-166">投影を開始するたびに、接続アプリを自動的に起動するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="83777-166">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="83777-167">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="83777-167">maintenanceWindowBlocked</span></span>|<span data-ttu-id="83777-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="83777-168">Boolean</span></span>|<span data-ttu-id="83777-169">デバイス更新のメンテナンス ウィンドウの設定をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="83777-169">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="83777-170">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="83777-170">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="83777-171">Int32</span><span class="sxs-lookup"><span data-stu-id="83777-171">Int32</span></span>|<span data-ttu-id="83777-172">デバイス更新のためのメンテナンス ウインドウの期間。</span><span class="sxs-lookup"><span data-stu-id="83777-172">Maintenance window duration for device updates.</span></span> <span data-ttu-id="83777-173">有効な値は 0 から 5 までです</span><span class="sxs-lookup"><span data-stu-id="83777-173">Valid values 0 to 5</span></span>|
|<span data-ttu-id="83777-174">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="83777-174">maintenanceWindowStartTime</span></span>|<span data-ttu-id="83777-175">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="83777-175">TimeOfDay</span></span>|<span data-ttu-id="83777-176">デバイス更新のためのメンテナンス ウィンドウの開始時刻。</span><span class="sxs-lookup"><span data-stu-id="83777-176">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="83777-177">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="83777-177">miracastChannel</span></span>|[<span data-ttu-id="83777-178">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="83777-178">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="83777-179">チャネル。</span><span class="sxs-lookup"><span data-stu-id="83777-179">The channel.</span></span> <span data-ttu-id="83777-180">可能な値は、`userDefined`、`one`、`two`、`three`、`four`、`five`、`six`、`seven`、`eight`、`nine`、`ten`、`eleven`、`thirtySix`、`forty`、`fortyFour`、`fortyEight`、`oneHundredFortyNine`、`oneHundredFiftyThree`、`oneHundredFiftySeven`、`oneHundredSixtyOne`、`oneHundredSixtyFive` です。</span><span class="sxs-lookup"><span data-stu-id="83777-180">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="83777-181">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="83777-181">miracastBlocked</span></span>|<span data-ttu-id="83777-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="83777-182">Boolean</span></span>|<span data-ttu-id="83777-183">ワイヤレス投影をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="83777-183">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="83777-184">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="83777-184">miracastRequirePin</span></span>|<span data-ttu-id="83777-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="83777-185">Boolean</span></span>|<span data-ttu-id="83777-186">ワイヤレス投影の pin が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="83777-186">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="83777-187">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="83777-187">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="83777-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="83777-188">Boolean</span></span>|<span data-ttu-id="83777-189">スタート メニューで [会議とファイル] 機能を無効にするかどうかを指定します。この機能は、サインイン ユーザーの会議とファイルを Office 365 から表示します。</span><span class="sxs-lookup"><span data-stu-id="83777-189">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="83777-190">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="83777-190">settingsBlockSessionResume</span></span>|<span data-ttu-id="83777-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="83777-191">Boolean</span></span>|<span data-ttu-id="83777-192">セッションがタイムアウトになった際にセッションを再開する機能を許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="83777-192">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="83777-193">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="83777-193">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="83777-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="83777-194">Boolean</span></span>|<span data-ttu-id="83777-195">スケジュールされている会議の招待者をサインイン ダイアログに自動入力する機能を無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="83777-195">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="83777-196">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="83777-196">settingsDefaultVolume</span></span>|<span data-ttu-id="83777-197">Int32</span><span class="sxs-lookup"><span data-stu-id="83777-197">Int32</span></span>|<span data-ttu-id="83777-198">新しいセッションの既定のボリューム値を指定します。</span><span class="sxs-lookup"><span data-stu-id="83777-198">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="83777-199">許可される値は、0 から 100 までです。</span><span class="sxs-lookup"><span data-stu-id="83777-199">Permitted values are 0-100.</span></span> <span data-ttu-id="83777-200">既定値は 45 です。</span><span class="sxs-lookup"><span data-stu-id="83777-200">The default is 45.</span></span> <span data-ttu-id="83777-201">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="83777-201">Valid values 0 to 100</span></span>|
|<span data-ttu-id="83777-202">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="83777-202">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="83777-203">Int32</span><span class="sxs-lookup"><span data-stu-id="83777-203">Int32</span></span>|<span data-ttu-id="83777-204">ハブ スクリーンがオフになるまでの分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="83777-204">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="83777-205">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="83777-205">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="83777-206">Int32</span><span class="sxs-lookup"><span data-stu-id="83777-206">Int32</span></span>|<span data-ttu-id="83777-207">セッションがタイムアウトになるまでの分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="83777-207">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="83777-208">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="83777-208">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="83777-209">Int32</span><span class="sxs-lookup"><span data-stu-id="83777-209">Int32</span></span>|<span data-ttu-id="83777-210">ハブがスリープ モードになるまでの分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="83777-210">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="83777-211">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="83777-211">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="83777-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="83777-212">Boolean</span></span>|<span data-ttu-id="83777-213">ユーザーが入室した際に、ようこそ画面が自動的に起動するのをブロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="83777-213">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="83777-214">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="83777-214">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="83777-215">String</span><span class="sxs-lookup"><span data-stu-id="83777-215">String</span></span>|<span data-ttu-id="83777-216">ようこそ画面の背景画像の URL。</span><span class="sxs-lookup"><span data-stu-id="83777-216">The welcome screen background image URL.</span></span> <span data-ttu-id="83777-217">URL は HTTPS プロトコルを使用し、PNG 画像を返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="83777-217">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="83777-218">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="83777-218">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="83777-219">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="83777-219">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="83777-220">表示される、ようこそ画面の会議情報。</span><span class="sxs-lookup"><span data-stu-id="83777-220">The welcome screen meeting information shown.</span></span> <span data-ttu-id="83777-221">可能な値は、`userDefined`、`showOrganizerAndTimeOnly`、`showOrganizerAndTimeAndSubject` です。</span><span class="sxs-lookup"><span data-stu-id="83777-221">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="83777-222">応答</span><span class="sxs-lookup"><span data-stu-id="83777-222">Response</span></span>
<span data-ttu-id="83777-223">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="83777-223">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83777-224">例</span><span class="sxs-lookup"><span data-stu-id="83777-224">Example</span></span>
### <a name="request"></a><span data-ttu-id="83777-225">要求</span><span class="sxs-lookup"><span data-stu-id="83777-225">Request</span></span>
<span data-ttu-id="83777-226">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="83777-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1150

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
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

### <a name="response"></a><span data-ttu-id="83777-227">応答</span><span class="sxs-lookup"><span data-stu-id="83777-227">Response</span></span>
<span data-ttu-id="83777-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="83777-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1322

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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


