---
title: Androidwork Profilの Maileasconfiguration の更新
description: Androidwork Profilな Maileasconfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 079bbe34d96a59e8de615f6b5b627d3649a56a93
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35950701"
---
# <a name="update-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="1abb1-103">Androidwork Profilの Maileasconfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="1abb1-103">Update androidWorkProfileGmailEasConfiguration</span></span>

> <span data-ttu-id="1abb1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1abb1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1abb1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1abb1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1abb1-106">[Androidwork Profilな Maileasconfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1abb1-106">Update the properties of a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1abb1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1abb1-107">Prerequisites</span></span>
<span data-ttu-id="1abb1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1abb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1abb1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1abb1-110">Permission type</span></span>|<span data-ttu-id="1abb1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1abb1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1abb1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1abb1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1abb1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1abb1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1abb1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1abb1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1abb1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1abb1-115">Not supported.</span></span>|
|<span data-ttu-id="1abb1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1abb1-116">Application</span></span>|<span data-ttu-id="1abb1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1abb1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1abb1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1abb1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1abb1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1abb1-119">Request headers</span></span>
|<span data-ttu-id="1abb1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1abb1-120">Header</span></span>|<span data-ttu-id="1abb1-121">値</span><span class="sxs-lookup"><span data-stu-id="1abb1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1abb1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1abb1-122">Authorization</span></span>|<span data-ttu-id="1abb1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1abb1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1abb1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1abb1-124">Accept</span></span>|<span data-ttu-id="1abb1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1abb1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1abb1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1abb1-126">Request body</span></span>
<span data-ttu-id="1abb1-127">要求本文で、 [Androidwork Profilな Maileasconfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1abb1-127">In the request body, supply a JSON representation for the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="1abb1-128">次の表に、 [Androidwork Profilare Maileasconfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1abb1-128">The following table shows the properties that are required when you create the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md).</span></span>

|<span data-ttu-id="1abb1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1abb1-129">Property</span></span>|<span data-ttu-id="1abb1-130">型</span><span class="sxs-lookup"><span data-stu-id="1abb1-130">Type</span></span>|<span data-ttu-id="1abb1-131">説明</span><span class="sxs-lookup"><span data-stu-id="1abb1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1abb1-132">id</span><span class="sxs-lookup"><span data-stu-id="1abb1-132">id</span></span>|<span data-ttu-id="1abb1-133">文字列</span><span class="sxs-lookup"><span data-stu-id="1abb1-133">String</span></span>|<span data-ttu-id="1abb1-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1abb1-134">Key of the entity.</span></span> <span data-ttu-id="1abb1-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1abb1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1abb1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1abb1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1abb1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1abb1-137">DateTimeOffset</span></span>|<span data-ttu-id="1abb1-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="1abb1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1abb1-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1abb1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1abb1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1abb1-140">roleScopeTagIds</span></span>|<span data-ttu-id="1abb1-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="1abb1-141">String collection</span></span>|<span data-ttu-id="1abb1-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="1abb1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1abb1-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1abb1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1abb1-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1abb1-144">supportsScopeTags</span></span>|<span data-ttu-id="1abb1-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1abb1-145">Boolean</span></span>|<span data-ttu-id="1abb1-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1abb1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1abb1-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="1abb1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1abb1-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="1abb1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1abb1-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="1abb1-149">This property is read-only.</span></span> <span data-ttu-id="1abb1-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1abb1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1abb1-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1abb1-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1abb1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1abb1-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1abb1-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="1abb1-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1abb1-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1abb1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1abb1-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1abb1-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1abb1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1abb1-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1abb1-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="1abb1-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1abb1-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1abb1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1abb1-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="1abb1-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1abb1-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="1abb1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1abb1-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="1abb1-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1abb1-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1abb1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1abb1-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1abb1-163">createdDateTime</span></span>|<span data-ttu-id="1abb1-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1abb1-164">DateTimeOffset</span></span>|<span data-ttu-id="1abb1-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1abb1-165">DateTime the object was created.</span></span> <span data-ttu-id="1abb1-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1abb1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1abb1-167">description</span><span class="sxs-lookup"><span data-stu-id="1abb1-167">description</span></span>|<span data-ttu-id="1abb1-168">String</span><span class="sxs-lookup"><span data-stu-id="1abb1-168">String</span></span>|<span data-ttu-id="1abb1-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="1abb1-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1abb1-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1abb1-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1abb1-171">displayName</span><span class="sxs-lookup"><span data-stu-id="1abb1-171">displayName</span></span>|<span data-ttu-id="1abb1-172">String</span><span class="sxs-lookup"><span data-stu-id="1abb1-172">String</span></span>|<span data-ttu-id="1abb1-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="1abb1-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1abb1-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1abb1-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1abb1-175">version</span><span class="sxs-lookup"><span data-stu-id="1abb1-175">version</span></span>|<span data-ttu-id="1abb1-176">Int32</span><span class="sxs-lookup"><span data-stu-id="1abb1-176">Int32</span></span>|<span data-ttu-id="1abb1-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1abb1-177">Version of the device configuration.</span></span> <span data-ttu-id="1abb1-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1abb1-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1abb1-179">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1abb1-179">authenticationMethod</span></span>|[<span data-ttu-id="1abb1-180">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1abb1-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="1abb1-181">Exchange ActiveSync の認証方法。</span><span class="sxs-lookup"><span data-stu-id="1abb1-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="1abb1-182">[Androidwork Profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1abb1-182">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="1abb1-183">可能な値は、`usernameAndPassword`、`certificate`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="1abb1-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="1abb1-184">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="1abb1-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="1abb1-185">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="1abb1-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="1abb1-186">電子メールを同期する時間の長さ。</span><span class="sxs-lookup"><span data-stu-id="1abb1-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="1abb1-187">[Androidwork Profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1abb1-187">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="1abb1-188">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="1abb1-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="1abb1-189">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="1abb1-189">emailAddressSource</span></span>|[<span data-ttu-id="1abb1-190">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="1abb1-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="1abb1-191">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="1abb1-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="1abb1-192">[Androidwork Profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1abb1-192">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="1abb1-193">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="1abb1-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="1abb1-194">hostName</span><span class="sxs-lookup"><span data-stu-id="1abb1-194">hostName</span></span>|<span data-ttu-id="1abb1-195">String</span><span class="sxs-lookup"><span data-stu-id="1abb1-195">String</span></span>|<span data-ttu-id="1abb1-196">メールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="1abb1-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="1abb1-197">[Androidwork Profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="1abb1-197">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="1abb1-198">requireSsl</span><span class="sxs-lookup"><span data-stu-id="1abb1-198">requireSsl</span></span>|<span data-ttu-id="1abb1-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="1abb1-199">Boolean</span></span>|<span data-ttu-id="1abb1-200">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1abb1-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="1abb1-201">[Androidwork Profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="1abb1-201">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="1abb1-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="1abb1-202">usernameSource</span></span>|[<span data-ttu-id="1abb1-203">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="1abb1-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="1abb1-204">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="1abb1-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="1abb1-205">[Androidwork Profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1abb1-205">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="1abb1-206">可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="1abb1-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="1abb1-207">応答</span><span class="sxs-lookup"><span data-stu-id="1abb1-207">Response</span></span>
<span data-ttu-id="1abb1-208">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Androidwork Profilな maileasconfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1abb1-208">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1abb1-209">例</span><span class="sxs-lookup"><span data-stu-id="1abb1-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="1abb1-210">要求</span><span class="sxs-lookup"><span data-stu-id="1abb1-210">Request</span></span>
<span data-ttu-id="1abb1-211">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1abb1-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1268

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
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
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName"
}
```

### <a name="response"></a><span data-ttu-id="1abb1-212">応答</span><span class="sxs-lookup"><span data-stu-id="1abb1-212">Response</span></span>
<span data-ttu-id="1abb1-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1abb1-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1440

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
  "id": "a4a44bb5-4bb5-a4a4-b54b-a4a4b54ba4a4",
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
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName"
}
```





