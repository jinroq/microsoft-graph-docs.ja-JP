---
title: windows10TeamGeneralConfiguration の作成
description: 新しい windows10TeamGeneralConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3ae4ff125219d470b4ae8bc8462f6b234adb0714
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985999"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="c02f4-103">windows10TeamGeneralConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="c02f4-103">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="c02f4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c02f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c02f4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c02f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c02f4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c02f4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c02f4-107">新しい [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c02f4-107">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c02f4-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c02f4-108">Prerequisites</span></span>
<span data-ttu-id="c02f4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c02f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c02f4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c02f4-111">Permission type</span></span>|<span data-ttu-id="c02f4-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c02f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c02f4-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c02f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c02f4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c02f4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c02f4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c02f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c02f4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c02f4-116">Not supported.</span></span>|
|<span data-ttu-id="c02f4-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c02f4-117">Application</span></span>|<span data-ttu-id="c02f4-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c02f4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c02f4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c02f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c02f4-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c02f4-120">Request headers</span></span>
|<span data-ttu-id="c02f4-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c02f4-121">Header</span></span>|<span data-ttu-id="c02f4-122">値</span><span class="sxs-lookup"><span data-stu-id="c02f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c02f4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c02f4-123">Authorization</span></span>|<span data-ttu-id="c02f4-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c02f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c02f4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c02f4-125">Accept</span></span>|<span data-ttu-id="c02f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c02f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c02f4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c02f4-127">Request body</span></span>
<span data-ttu-id="c02f4-128">要求本文で、windows10TeamGeneralConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c02f4-128">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="c02f4-129">次の表に、windows10TeamGeneralConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c02f4-129">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="c02f4-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c02f4-130">Property</span></span>|<span data-ttu-id="c02f4-131">型</span><span class="sxs-lookup"><span data-stu-id="c02f4-131">Type</span></span>|<span data-ttu-id="c02f4-132">説明</span><span class="sxs-lookup"><span data-stu-id="c02f4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c02f4-133">id</span><span class="sxs-lookup"><span data-stu-id="c02f4-133">id</span></span>|<span data-ttu-id="c02f4-134">String</span><span class="sxs-lookup"><span data-stu-id="c02f4-134">String</span></span>|<span data-ttu-id="c02f4-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c02f4-135">Key of the entity.</span></span> <span data-ttu-id="c02f4-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c02f4-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c02f4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c02f4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c02f4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c02f4-138">DateTimeOffset</span></span>|<span data-ttu-id="c02f4-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c02f4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c02f4-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c02f4-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c02f4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c02f4-141">roleScopeTagIds</span></span>|<span data-ttu-id="c02f4-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c02f4-142">String collection</span></span>|<span data-ttu-id="c02f4-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="c02f4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c02f4-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c02f4-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c02f4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c02f4-145">supportsScopeTags</span></span>|<span data-ttu-id="c02f4-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="c02f4-146">Boolean</span></span>|<span data-ttu-id="c02f4-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c02f4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c02f4-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="c02f4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c02f4-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="c02f4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c02f4-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="c02f4-150">This property is read-only.</span></span> <span data-ttu-id="c02f4-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c02f4-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c02f4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c02f4-152">createdDateTime</span></span>|<span data-ttu-id="c02f4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c02f4-153">DateTimeOffset</span></span>|<span data-ttu-id="c02f4-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c02f4-154">DateTime the object was created.</span></span> <span data-ttu-id="c02f4-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c02f4-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c02f4-156">説明</span><span class="sxs-lookup"><span data-stu-id="c02f4-156">description</span></span>|<span data-ttu-id="c02f4-157">String</span><span class="sxs-lookup"><span data-stu-id="c02f4-157">String</span></span>|<span data-ttu-id="c02f4-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="c02f4-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c02f4-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c02f4-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c02f4-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c02f4-160">displayName</span></span>|<span data-ttu-id="c02f4-161">String</span><span class="sxs-lookup"><span data-stu-id="c02f4-161">String</span></span>|<span data-ttu-id="c02f4-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="c02f4-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c02f4-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c02f4-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c02f4-164">version</span><span class="sxs-lookup"><span data-stu-id="c02f4-164">version</span></span>|<span data-ttu-id="c02f4-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c02f4-165">Int32</span></span>|<span data-ttu-id="c02f4-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="c02f4-166">Version of the device configuration.</span></span> <span data-ttu-id="c02f4-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c02f4-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c02f4-168">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="c02f4-168">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="c02f4-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="c02f4-169">Boolean</span></span>|<span data-ttu-id="c02f4-170">Azure Operational Insights をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c02f4-170">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="c02f4-171">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="c02f4-171">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="c02f4-172">String</span><span class="sxs-lookup"><span data-stu-id="c02f4-172">String</span></span>|<span data-ttu-id="c02f4-173">Azure Operational Insights のワークスペース ID。</span><span class="sxs-lookup"><span data-stu-id="c02f4-173">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="c02f4-174">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="c02f4-174">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="c02f4-175">String</span><span class="sxs-lookup"><span data-stu-id="c02f4-175">String</span></span>|<span data-ttu-id="c02f4-176">Azure Operational Insights のワークスペース キー。</span><span class="sxs-lookup"><span data-stu-id="c02f4-176">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="c02f4-177">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="c02f4-177">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="c02f4-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="c02f4-178">Boolean</span></span>|<span data-ttu-id="c02f4-179">投影を開始するたびに、接続アプリを自動的に起動するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c02f4-179">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="c02f4-180">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="c02f4-180">maintenanceWindowBlocked</span></span>|<span data-ttu-id="c02f4-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="c02f4-181">Boolean</span></span>|<span data-ttu-id="c02f4-182">デバイス更新のメンテナンス ウィンドウの設定をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c02f4-182">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="c02f4-183">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="c02f4-183">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="c02f4-184">Int32</span><span class="sxs-lookup"><span data-stu-id="c02f4-184">Int32</span></span>|<span data-ttu-id="c02f4-185">デバイス更新のためのメンテナンス ウインドウの期間。</span><span class="sxs-lookup"><span data-stu-id="c02f4-185">Maintenance window duration for device updates.</span></span> <span data-ttu-id="c02f4-186">有効な値は 0 から 5 までです</span><span class="sxs-lookup"><span data-stu-id="c02f4-186">Valid values 0 to 5</span></span>|
|<span data-ttu-id="c02f4-187">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="c02f4-187">maintenanceWindowStartTime</span></span>|<span data-ttu-id="c02f4-188">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c02f4-188">TimeOfDay</span></span>|<span data-ttu-id="c02f4-189">デバイス更新のためのメンテナンス ウィンドウの開始時刻。</span><span class="sxs-lookup"><span data-stu-id="c02f4-189">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="c02f4-190">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="c02f4-190">miracastChannel</span></span>|[<span data-ttu-id="c02f4-191">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="c02f4-191">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="c02f4-192">チャネル。</span><span class="sxs-lookup"><span data-stu-id="c02f4-192">The channel.</span></span> <span data-ttu-id="c02f4-193">可能な値は、`userDefined`、`one`、`two`、`three`、`four`、`five`、`six`、`seven`、`eight`、`nine`、`ten`、`eleven`、`thirtySix`、`forty`、`fortyFour`、`fortyEight`、`oneHundredFortyNine`、`oneHundredFiftyThree`、`oneHundredFiftySeven`、`oneHundredSixtyOne`、`oneHundredSixtyFive` です。</span><span class="sxs-lookup"><span data-stu-id="c02f4-193">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="c02f4-194">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="c02f4-194">miracastBlocked</span></span>|<span data-ttu-id="c02f4-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c02f4-195">Boolean</span></span>|<span data-ttu-id="c02f4-196">ワイヤレス投影をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c02f4-196">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="c02f4-197">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="c02f4-197">miracastRequirePin</span></span>|<span data-ttu-id="c02f4-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="c02f4-198">Boolean</span></span>|<span data-ttu-id="c02f4-199">ワイヤレス投影の pin が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c02f4-199">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="c02f4-200">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="c02f4-200">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="c02f4-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="c02f4-201">Boolean</span></span>|<span data-ttu-id="c02f4-202">スタート メニューで [会議とファイル] 機能を無効にするかどうかを指定します。この機能は、サインイン ユーザーの会議とファイルを Office 365 から表示します。</span><span class="sxs-lookup"><span data-stu-id="c02f4-202">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="c02f4-203">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="c02f4-203">settingsBlockSessionResume</span></span>|<span data-ttu-id="c02f4-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="c02f4-204">Boolean</span></span>|<span data-ttu-id="c02f4-205">セッションがタイムアウトになった際にセッションを再開する機能を許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c02f4-205">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="c02f4-206">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="c02f4-206">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="c02f4-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="c02f4-207">Boolean</span></span>|<span data-ttu-id="c02f4-208">スケジュールされている会議の招待者をサインイン ダイアログに自動入力する機能を無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c02f4-208">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="c02f4-209">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="c02f4-209">settingsDefaultVolume</span></span>|<span data-ttu-id="c02f4-210">Int32</span><span class="sxs-lookup"><span data-stu-id="c02f4-210">Int32</span></span>|<span data-ttu-id="c02f4-211">新しいセッションの既定のボリューム値を指定します。</span><span class="sxs-lookup"><span data-stu-id="c02f4-211">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="c02f4-212">許可される値は、0 から 100 までです。</span><span class="sxs-lookup"><span data-stu-id="c02f4-212">Permitted values are 0-100.</span></span> <span data-ttu-id="c02f4-213">既定値は 45 です。</span><span class="sxs-lookup"><span data-stu-id="c02f4-213">The default is 45.</span></span> <span data-ttu-id="c02f4-214">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="c02f4-214">Valid values 0 to 100</span></span>|
|<span data-ttu-id="c02f4-215">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="c02f4-215">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="c02f4-216">Int32</span><span class="sxs-lookup"><span data-stu-id="c02f4-216">Int32</span></span>|<span data-ttu-id="c02f4-217">ハブ スクリーンがオフになるまでの分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="c02f4-217">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="c02f4-218">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="c02f4-218">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="c02f4-219">Int32</span><span class="sxs-lookup"><span data-stu-id="c02f4-219">Int32</span></span>|<span data-ttu-id="c02f4-220">セッションがタイムアウトになるまでの分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="c02f4-220">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="c02f4-221">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="c02f4-221">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="c02f4-222">Int32</span><span class="sxs-lookup"><span data-stu-id="c02f4-222">Int32</span></span>|<span data-ttu-id="c02f4-223">ハブがスリープ モードになるまでの分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="c02f4-223">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="c02f4-224">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="c02f4-224">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="c02f4-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="c02f4-225">Boolean</span></span>|<span data-ttu-id="c02f4-226">ユーザーが入室した際に、ようこそ画面が自動的に起動するのをブロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c02f4-226">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="c02f4-227">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="c02f4-227">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="c02f4-228">String</span><span class="sxs-lookup"><span data-stu-id="c02f4-228">String</span></span>|<span data-ttu-id="c02f4-229">ようこそ画面の背景画像の URL。</span><span class="sxs-lookup"><span data-stu-id="c02f4-229">The welcome screen background image URL.</span></span> <span data-ttu-id="c02f4-230">URL は HTTPS プロトコルを使用し、PNG 画像を返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="c02f4-230">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="c02f4-231">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="c02f4-231">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="c02f4-232">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="c02f4-232">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="c02f4-233">表示される、ようこそ画面の会議情報。</span><span class="sxs-lookup"><span data-stu-id="c02f4-233">The welcome screen meeting information shown.</span></span> <span data-ttu-id="c02f4-234">可能な値は、`userDefined`、`showOrganizerAndTimeOnly`、`showOrganizerAndTimeAndSubject` です。</span><span class="sxs-lookup"><span data-stu-id="c02f4-234">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="c02f4-235">応答</span><span class="sxs-lookup"><span data-stu-id="c02f4-235">Response</span></span>
<span data-ttu-id="c02f4-236">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c02f4-236">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c02f4-237">例</span><span class="sxs-lookup"><span data-stu-id="c02f4-237">Example</span></span>
### <a name="request"></a><span data-ttu-id="c02f4-238">要求</span><span class="sxs-lookup"><span data-stu-id="c02f4-238">Request</span></span>
<span data-ttu-id="c02f4-239">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c02f4-239">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1306

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
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

### <a name="response"></a><span data-ttu-id="c02f4-240">応答</span><span class="sxs-lookup"><span data-stu-id="c02f4-240">Response</span></span>
<span data-ttu-id="c02f4-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c02f4-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





