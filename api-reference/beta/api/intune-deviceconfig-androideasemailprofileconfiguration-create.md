---
title: AndroidEasEmailProfileConfiguration 作成
description: Androide Asemailprofil/新しいオブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a1c5b7c12e306f0ac718f86cb129e158cff50da1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34971263"
---
# <a name="create-androideasemailprofileconfiguration"></a><span data-ttu-id="6dc22-103">AndroidEasEmailProfileConfiguration 作成</span><span class="sxs-lookup"><span data-stu-id="6dc22-103">Create androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="6dc22-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6dc22-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6dc22-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6dc22-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dc22-106">[Androide Asemailprofil/](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)新しいオブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6dc22-106">Create a new [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6dc22-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6dc22-107">Prerequisites</span></span>
<span data-ttu-id="6dc22-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6dc22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dc22-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6dc22-110">Permission type</span></span>|<span data-ttu-id="6dc22-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6dc22-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dc22-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6dc22-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6dc22-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dc22-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6dc22-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6dc22-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dc22-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6dc22-115">Not supported.</span></span>|
|<span data-ttu-id="6dc22-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6dc22-116">Application</span></span>|<span data-ttu-id="6dc22-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6dc22-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dc22-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6dc22-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6dc22-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6dc22-119">Request headers</span></span>
|<span data-ttu-id="6dc22-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6dc22-120">Header</span></span>|<span data-ttu-id="6dc22-121">値</span><span class="sxs-lookup"><span data-stu-id="6dc22-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dc22-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dc22-122">Authorization</span></span>|<span data-ttu-id="6dc22-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6dc22-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dc22-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6dc22-124">Accept</span></span>|<span data-ttu-id="6dc22-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6dc22-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dc22-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6dc22-126">Request body</span></span>
<span data-ttu-id="6dc22-127">要求本文で、Androide Asemailprofil//スキーマオブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6dc22-127">In the request body, supply a JSON representation for the androidEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="6dc22-128">次の表に、Androide Asemailprofilの作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6dc22-128">The following table shows the properties that are required when you create the androidEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="6dc22-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6dc22-129">Property</span></span>|<span data-ttu-id="6dc22-130">型</span><span class="sxs-lookup"><span data-stu-id="6dc22-130">Type</span></span>|<span data-ttu-id="6dc22-131">説明</span><span class="sxs-lookup"><span data-stu-id="6dc22-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dc22-132">id</span><span class="sxs-lookup"><span data-stu-id="6dc22-132">id</span></span>|<span data-ttu-id="6dc22-133">文字列</span><span class="sxs-lookup"><span data-stu-id="6dc22-133">String</span></span>|<span data-ttu-id="6dc22-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6dc22-134">Key of the entity.</span></span> <span data-ttu-id="6dc22-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6dc22-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dc22-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6dc22-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6dc22-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6dc22-137">DateTimeOffset</span></span>|<span data-ttu-id="6dc22-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="6dc22-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6dc22-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6dc22-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dc22-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6dc22-140">roleScopeTagIds</span></span>|<span data-ttu-id="6dc22-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="6dc22-141">String collection</span></span>|<span data-ttu-id="6dc22-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="6dc22-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6dc22-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6dc22-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dc22-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6dc22-144">supportsScopeTags</span></span>|<span data-ttu-id="6dc22-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6dc22-145">Boolean</span></span>|<span data-ttu-id="6dc22-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6dc22-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6dc22-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="6dc22-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6dc22-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="6dc22-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6dc22-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="6dc22-149">This property is read-only.</span></span> <span data-ttu-id="6dc22-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6dc22-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dc22-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6dc22-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6dc22-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6dc22-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6dc22-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="6dc22-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6dc22-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6dc22-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dc22-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6dc22-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6dc22-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6dc22-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6dc22-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="6dc22-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6dc22-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6dc22-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dc22-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="6dc22-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6dc22-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="6dc22-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6dc22-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="6dc22-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6dc22-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6dc22-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dc22-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6dc22-163">createdDateTime</span></span>|<span data-ttu-id="6dc22-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6dc22-164">DateTimeOffset</span></span>|<span data-ttu-id="6dc22-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6dc22-165">DateTime the object was created.</span></span> <span data-ttu-id="6dc22-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6dc22-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dc22-167">description</span><span class="sxs-lookup"><span data-stu-id="6dc22-167">description</span></span>|<span data-ttu-id="6dc22-168">String</span><span class="sxs-lookup"><span data-stu-id="6dc22-168">String</span></span>|<span data-ttu-id="6dc22-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="6dc22-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6dc22-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6dc22-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dc22-171">displayName</span><span class="sxs-lookup"><span data-stu-id="6dc22-171">displayName</span></span>|<span data-ttu-id="6dc22-172">String</span><span class="sxs-lookup"><span data-stu-id="6dc22-172">String</span></span>|<span data-ttu-id="6dc22-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="6dc22-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6dc22-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6dc22-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dc22-175">version</span><span class="sxs-lookup"><span data-stu-id="6dc22-175">version</span></span>|<span data-ttu-id="6dc22-176">Int32</span><span class="sxs-lookup"><span data-stu-id="6dc22-176">Int32</span></span>|<span data-ttu-id="6dc22-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="6dc22-177">Version of the device configuration.</span></span> <span data-ttu-id="6dc22-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6dc22-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dc22-179">accountName</span><span class="sxs-lookup"><span data-stu-id="6dc22-179">accountName</span></span>|<span data-ttu-id="6dc22-180">String</span><span class="sxs-lookup"><span data-stu-id="6dc22-180">String</span></span>|<span data-ttu-id="6dc22-181">ユーザーに EA (この) プロファイルの名前として表示される Exchange ActiveSync アカウント名。</span><span class="sxs-lookup"><span data-stu-id="6dc22-181">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="6dc22-182">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6dc22-182">authenticationMethod</span></span>|[<span data-ttu-id="6dc22-183">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6dc22-183">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="6dc22-184">Exchange ActiveSync の認証方法。</span><span class="sxs-lookup"><span data-stu-id="6dc22-184">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="6dc22-185">可能な値は、`usernameAndPassword`、`certificate`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="6dc22-185">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="6dc22-186">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="6dc22-186">syncCalendar</span></span>|<span data-ttu-id="6dc22-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="6dc22-187">Boolean</span></span>|<span data-ttu-id="6dc22-188">予定表の同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="6dc22-188">Toggles syncing the calendar.</span></span> <span data-ttu-id="6dc22-189">False カレンダーに設定すると、デバイスで無効になります。</span><span class="sxs-lookup"><span data-stu-id="6dc22-189">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="6dc22-190">syncContacts</span><span class="sxs-lookup"><span data-stu-id="6dc22-190">syncContacts</span></span>|<span data-ttu-id="6dc22-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="6dc22-191">Boolean</span></span>|<span data-ttu-id="6dc22-192">連絡先の同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="6dc22-192">Toggles syncing contacts.</span></span> <span data-ttu-id="6dc22-193">False に設定すると、デバイスで [連絡先] がオフになります。</span><span class="sxs-lookup"><span data-stu-id="6dc22-193">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="6dc22-194">syncTasks</span><span class="sxs-lookup"><span data-stu-id="6dc22-194">syncTasks</span></span>|<span data-ttu-id="6dc22-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="6dc22-195">Boolean</span></span>|<span data-ttu-id="6dc22-196">タスクの同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="6dc22-196">Toggles syncing tasks.</span></span> <span data-ttu-id="6dc22-197">False タスクに設定した場合は、デバイスで無効になります。</span><span class="sxs-lookup"><span data-stu-id="6dc22-197">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="6dc22-198">syncNotes</span><span class="sxs-lookup"><span data-stu-id="6dc22-198">syncNotes</span></span>|<span data-ttu-id="6dc22-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="6dc22-199">Boolean</span></span>|<span data-ttu-id="6dc22-200">メモの同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="6dc22-200">Toggles syncing notes.</span></span> <span data-ttu-id="6dc22-201">False に設定すると、デバイスでは、メモがオフになります。</span><span class="sxs-lookup"><span data-stu-id="6dc22-201">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="6dc22-202">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="6dc22-202">durationOfEmailToSync</span></span>|[<span data-ttu-id="6dc22-203">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="6dc22-203">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="6dc22-204">電子メールを同期する時間の長さ。</span><span class="sxs-lookup"><span data-stu-id="6dc22-204">Duration of time email should be synced to.</span></span> <span data-ttu-id="6dc22-205">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="6dc22-205">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="6dc22-206">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="6dc22-206">emailAddressSource</span></span>|[<span data-ttu-id="6dc22-207">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="6dc22-207">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="6dc22-208">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="6dc22-208">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6dc22-209">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="6dc22-209">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="6dc22-210">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="6dc22-210">emailSyncSchedule</span></span>|[<span data-ttu-id="6dc22-211">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="6dc22-211">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="6dc22-212">電子メール同期スケジュール。</span><span class="sxs-lookup"><span data-stu-id="6dc22-212">Email sync schedule.</span></span> <span data-ttu-id="6dc22-213">可能な値は、`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage` です。</span><span class="sxs-lookup"><span data-stu-id="6dc22-213">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="6dc22-214">hostName</span><span class="sxs-lookup"><span data-stu-id="6dc22-214">hostName</span></span>|<span data-ttu-id="6dc22-215">String</span><span class="sxs-lookup"><span data-stu-id="6dc22-215">String</span></span>|<span data-ttu-id="6dc22-216">ネイティブメールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="6dc22-216">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="6dc22-217">requireSmime</span><span class="sxs-lookup"><span data-stu-id="6dc22-217">requireSmime</span></span>|<span data-ttu-id="6dc22-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="6dc22-218">Boolean</span></span>|<span data-ttu-id="6dc22-219">S/MIME 証明書を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6dc22-219">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="6dc22-220">requireSsl</span><span class="sxs-lookup"><span data-stu-id="6dc22-220">requireSsl</span></span>|<span data-ttu-id="6dc22-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="6dc22-221">Boolean</span></span>|<span data-ttu-id="6dc22-222">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6dc22-222">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="6dc22-223">usernameSource</span><span class="sxs-lookup"><span data-stu-id="6dc22-223">usernameSource</span></span>|[<span data-ttu-id="6dc22-224">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="6dc22-224">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="6dc22-225">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="6dc22-225">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6dc22-226">使用可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="6dc22-226">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="6dc22-227">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="6dc22-227">userDomainNameSource</span></span>|[<span data-ttu-id="6dc22-228">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="6dc22-228">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="6dc22-229">UserDomainname 属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="6dc22-229">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6dc22-230">可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="6dc22-230">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="6dc22-231">customDomainName</span><span class="sxs-lookup"><span data-stu-id="6dc22-231">customDomainName</span></span>|<span data-ttu-id="6dc22-232">String</span><span class="sxs-lookup"><span data-stu-id="6dc22-232">String</span></span>|<span data-ttu-id="6dc22-233">デバイスにインストールする前に電子メールプロファイルを生成するときに使用するカスタムドメイン名の値。</span><span class="sxs-lookup"><span data-stu-id="6dc22-233">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="6dc22-234">応答</span><span class="sxs-lookup"><span data-stu-id="6dc22-234">Response</span></span>
<span data-ttu-id="6dc22-235">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Androide asemailprofil/](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) "オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6dc22-235">If successful, this method returns a `201 Created` response code and a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dc22-236">例</span><span class="sxs-lookup"><span data-stu-id="6dc22-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="6dc22-237">要求</span><span class="sxs-lookup"><span data-stu-id="6dc22-237">Request</span></span>
<span data-ttu-id="6dc22-238">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6dc22-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1566

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
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
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value"
}
```

### <a name="response"></a><span data-ttu-id="6dc22-239">応答</span><span class="sxs-lookup"><span data-stu-id="6dc22-239">Response</span></span>
<span data-ttu-id="6dc22-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6dc22-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1738

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "id": "ee5e5610-5610-ee5e-1056-5eee10565eee",
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
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value"
}
```





