---
title: IosEasEmailProfileConfiguration 更新
description: IosEasEmailProfileConfiguration プロパティオブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6bd71c5db6f634e0ce333818c709c9c55316ba8c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923631"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="adf9b-103">IosEasEmailProfileConfiguration 更新</span><span class="sxs-lookup"><span data-stu-id="adf9b-103">Update iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="adf9b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="adf9b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="adf9b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="adf9b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adf9b-106">[Ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)プロパティオブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="adf9b-106">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="adf9b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="adf9b-107">Prerequisites</span></span>
<span data-ttu-id="adf9b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="adf9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adf9b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="adf9b-110">Permission type</span></span>|<span data-ttu-id="adf9b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="adf9b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adf9b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="adf9b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="adf9b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adf9b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="adf9b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="adf9b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adf9b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="adf9b-115">Not supported.</span></span>|
|<span data-ttu-id="adf9b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="adf9b-116">Application</span></span>|<span data-ttu-id="adf9b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="adf9b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="adf9b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="adf9b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="adf9b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="adf9b-119">Request headers</span></span>
|<span data-ttu-id="adf9b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="adf9b-120">Header</span></span>|<span data-ttu-id="adf9b-121">値</span><span class="sxs-lookup"><span data-stu-id="adf9b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adf9b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="adf9b-122">Authorization</span></span>|<span data-ttu-id="adf9b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="adf9b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adf9b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="adf9b-124">Accept</span></span>|<span data-ttu-id="adf9b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="adf9b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adf9b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="adf9b-126">Request body</span></span>
<span data-ttu-id="adf9b-127">要求本文で、 [Ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)このオブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="adf9b-127">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="adf9b-128">次の表に、 [Ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="adf9b-128">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="adf9b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="adf9b-129">Property</span></span>|<span data-ttu-id="adf9b-130">型</span><span class="sxs-lookup"><span data-stu-id="adf9b-130">Type</span></span>|<span data-ttu-id="adf9b-131">説明</span><span class="sxs-lookup"><span data-stu-id="adf9b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adf9b-132">id</span><span class="sxs-lookup"><span data-stu-id="adf9b-132">id</span></span>|<span data-ttu-id="adf9b-133">文字列</span><span class="sxs-lookup"><span data-stu-id="adf9b-133">String</span></span>|<span data-ttu-id="adf9b-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="adf9b-134">Key of the entity.</span></span> <span data-ttu-id="adf9b-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="adf9b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adf9b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="adf9b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="adf9b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adf9b-137">DateTimeOffset</span></span>|<span data-ttu-id="adf9b-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="adf9b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="adf9b-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="adf9b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adf9b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="adf9b-140">roleScopeTagIds</span></span>|<span data-ttu-id="adf9b-141">String collection</span><span class="sxs-lookup"><span data-stu-id="adf9b-141">String collection</span></span>|<span data-ttu-id="adf9b-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="adf9b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="adf9b-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="adf9b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adf9b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="adf9b-144">supportsScopeTags</span></span>|<span data-ttu-id="adf9b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="adf9b-145">Boolean</span></span>|<span data-ttu-id="adf9b-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="adf9b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="adf9b-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="adf9b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="adf9b-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="adf9b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="adf9b-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="adf9b-149">This property is read-only.</span></span> <span data-ttu-id="adf9b-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="adf9b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adf9b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="adf9b-151">createdDateTime</span></span>|<span data-ttu-id="adf9b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adf9b-152">DateTimeOffset</span></span>|<span data-ttu-id="adf9b-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="adf9b-153">DateTime the object was created.</span></span> <span data-ttu-id="adf9b-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="adf9b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adf9b-155">description</span><span class="sxs-lookup"><span data-stu-id="adf9b-155">description</span></span>|<span data-ttu-id="adf9b-156">String</span><span class="sxs-lookup"><span data-stu-id="adf9b-156">String</span></span>|<span data-ttu-id="adf9b-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="adf9b-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="adf9b-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="adf9b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adf9b-159">displayName</span><span class="sxs-lookup"><span data-stu-id="adf9b-159">displayName</span></span>|<span data-ttu-id="adf9b-160">String</span><span class="sxs-lookup"><span data-stu-id="adf9b-160">String</span></span>|<span data-ttu-id="adf9b-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="adf9b-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="adf9b-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="adf9b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adf9b-163">version</span><span class="sxs-lookup"><span data-stu-id="adf9b-163">version</span></span>|<span data-ttu-id="adf9b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="adf9b-164">Int32</span></span>|<span data-ttu-id="adf9b-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="adf9b-165">Version of the device configuration.</span></span> <span data-ttu-id="adf9b-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="adf9b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adf9b-167">usernameSource</span><span class="sxs-lookup"><span data-stu-id="adf9b-167">usernameSource</span></span>|[<span data-ttu-id="adf9b-168">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="adf9b-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="adf9b-169">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="adf9b-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="adf9b-170">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="adf9b-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="adf9b-171">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="adf9b-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="adf9b-172">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="adf9b-172">usernameAADSource</span></span>|[<span data-ttu-id="adf9b-173">usernameSource</span><span class="sxs-lookup"><span data-stu-id="adf9b-173">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="adf9b-174">メールプロファイルのユーザー名を取得するために使用される AAD フィールドの名前。</span><span class="sxs-lookup"><span data-stu-id="adf9b-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="adf9b-175">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="adf9b-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="adf9b-176">可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。</span><span class="sxs-lookup"><span data-stu-id="adf9b-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="adf9b-177">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="adf9b-177">userDomainNameSource</span></span>|[<span data-ttu-id="adf9b-178">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="adf9b-178">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="adf9b-179">UserDomainname 属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="adf9b-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="adf9b-180">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="adf9b-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="adf9b-181">可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="adf9b-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="adf9b-182">customDomainName</span><span class="sxs-lookup"><span data-stu-id="adf9b-182">customDomainName</span></span>|<span data-ttu-id="adf9b-183">String</span><span class="sxs-lookup"><span data-stu-id="adf9b-183">String</span></span>|<span data-ttu-id="adf9b-184">デバイスにインストールする前に電子メールプロファイルを生成するときに使用するカスタムドメイン名の値。</span><span class="sxs-lookup"><span data-stu-id="adf9b-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="adf9b-185">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="adf9b-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="adf9b-186">accountName</span><span class="sxs-lookup"><span data-stu-id="adf9b-186">accountName</span></span>|<span data-ttu-id="adf9b-187">String</span><span class="sxs-lookup"><span data-stu-id="adf9b-187">String</span></span>|<span data-ttu-id="adf9b-188">アカウント名。</span><span class="sxs-lookup"><span data-stu-id="adf9b-188">Account name.</span></span>|
|<span data-ttu-id="adf9b-189">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="adf9b-189">authenticationMethod</span></span>|[<span data-ttu-id="adf9b-190">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="adf9b-190">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="adf9b-191">この電子メールプロファイルの認証方法。</span><span class="sxs-lookup"><span data-stu-id="adf9b-191">Authentication method for this Email profile.</span></span> <span data-ttu-id="adf9b-192">可能な値は、`usernameAndPassword`、`certificate`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="adf9b-192">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="adf9b-193">Blockmovingmessagestooruncommand/電子メールアカウント</span><span class="sxs-lookup"><span data-stu-id="adf9b-193">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="adf9b-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="adf9b-194">Boolean</span></span>|<span data-ttu-id="adf9b-195">他の電子メールアカウントへのメッセージの移動をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="adf9b-195">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="adf9b-196">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="adf9b-196">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="adf9b-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="adf9b-197">Boolean</span></span>|<span data-ttu-id="adf9b-198">サードパーティ製アプリからの電子メールの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="adf9b-198">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="adf9b-199">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="adf9b-199">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="adf9b-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="adf9b-200">Boolean</span></span>|<span data-ttu-id="adf9b-201">最近使用した電子メールアドレスの同期をブロックするかどうかを示します (たとえば、新しい電子メールを作成する場合)。</span><span class="sxs-lookup"><span data-stu-id="adf9b-201">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="adf9b-202">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="adf9b-202">durationOfEmailToSync</span></span>|[<span data-ttu-id="adf9b-203">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="adf9b-203">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="adf9b-204">電子メールを同期する時間。</span><span class="sxs-lookup"><span data-stu-id="adf9b-204">Duration of time email should be synced back to.</span></span> <span data-ttu-id="adf9b-205">.</span><span class="sxs-lookup"><span data-stu-id="adf9b-205"></span></span> <span data-ttu-id="adf9b-206">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="adf9b-206">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="adf9b-207">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="adf9b-207">emailAddressSource</span></span>|[<span data-ttu-id="adf9b-208">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="adf9b-208">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="adf9b-209">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="adf9b-209">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="adf9b-210">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="adf9b-210">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="adf9b-211">hostName</span><span class="sxs-lookup"><span data-stu-id="adf9b-211">hostName</span></span>|<span data-ttu-id="adf9b-212">String</span><span class="sxs-lookup"><span data-stu-id="adf9b-212">String</span></span>|<span data-ttu-id="adf9b-213">ネイティブメールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="adf9b-213">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="adf9b-214">requireSmime</span><span class="sxs-lookup"><span data-stu-id="adf9b-214">requireSmime</span></span>|<span data-ttu-id="adf9b-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="adf9b-215">Boolean</span></span>|<span data-ttu-id="adf9b-216">S/MIME 証明書を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="adf9b-216">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="adf9b-217">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="adf9b-217">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="adf9b-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="adf9b-218">Boolean</span></span>|<span data-ttu-id="adf9b-219">暗号化されていない電子メールを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="adf9b-219">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="adf9b-220">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="adf9b-220">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="adf9b-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="adf9b-221">Boolean</span></span>|<span data-ttu-id="adf9b-222">True S/MIME 暗号化に設定すると、既定で有効になります。</span><span class="sxs-lookup"><span data-stu-id="adf9b-222">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="adf9b-223">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="adf9b-223">smimeSigningEnabled</span></span>|<span data-ttu-id="adf9b-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="adf9b-224">Boolean</span></span>|<span data-ttu-id="adf9b-225">このアカウントに対して true S/MIME 署名を有効に設定した場合</span><span class="sxs-lookup"><span data-stu-id="adf9b-225">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="adf9b-226">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="adf9b-226">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="adf9b-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="adf9b-227">Boolean</span></span>|<span data-ttu-id="adf9b-228">True に設定されている場合、ユーザーは S/MIME の署名のオンとオフを切り替えることができます。</span><span class="sxs-lookup"><span data-stu-id="adf9b-228">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="adf9b-229">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="adf9b-229">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="adf9b-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="adf9b-230">Boolean</span></span>|<span data-ttu-id="adf9b-231">True に設定されている場合、ユーザーは既定の設定で暗号化を切り替えることができます。</span><span class="sxs-lookup"><span data-stu-id="adf9b-231">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="adf9b-232">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="adf9b-232">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="adf9b-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="adf9b-233">Boolean</span></span>|<span data-ttu-id="adf9b-234">True に設定されている場合、ユーザーは署名 id を選択できます。</span><span class="sxs-lookup"><span data-stu-id="adf9b-234">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="adf9b-235">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="adf9b-235">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="adf9b-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="adf9b-236">Boolean</span></span>|<span data-ttu-id="adf9b-237">True に設定されている場合、ユーザーは S/MIME 暗号化 id を選択できます。</span><span class="sxs-lookup"><span data-stu-id="adf9b-237">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="adf9b-238">requireSsl</span><span class="sxs-lookup"><span data-stu-id="adf9b-238">requireSsl</span></span>|<span data-ttu-id="adf9b-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="adf9b-239">Boolean</span></span>|<span data-ttu-id="adf9b-240">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="adf9b-240">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="adf9b-241">useOAuth</span><span class="sxs-lookup"><span data-stu-id="adf9b-241">useOAuth</span></span>|<span data-ttu-id="adf9b-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="adf9b-242">Boolean</span></span>|<span data-ttu-id="adf9b-243">接続で認証に OAuth を使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="adf9b-243">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="adf9b-244">signingCertificateType</span><span class="sxs-lookup"><span data-stu-id="adf9b-244">signingCertificateType</span></span>|[<span data-ttu-id="adf9b-245">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="adf9b-245">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="adf9b-246">この電子メールプロファイルの署名証明書の種類。</span><span class="sxs-lookup"><span data-stu-id="adf9b-246">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="adf9b-247">可能な値は、`none`、`certificate`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="adf9b-247">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="adf9b-248">encryptionCertificateType</span><span class="sxs-lookup"><span data-stu-id="adf9b-248">encryptionCertificateType</span></span>|[<span data-ttu-id="adf9b-249">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="adf9b-249">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="adf9b-250">この電子メールプロファイルの暗号化証明書の種類。</span><span class="sxs-lookup"><span data-stu-id="adf9b-250">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="adf9b-251">可能な値は、`none`、`certificate`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="adf9b-251">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="adf9b-252">応答</span><span class="sxs-lookup"><span data-stu-id="adf9b-252">Response</span></span>
<span data-ttu-id="adf9b-253">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) "オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="adf9b-253">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adf9b-254">例</span><span class="sxs-lookup"><span data-stu-id="adf9b-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="adf9b-255">要求</span><span class="sxs-lookup"><span data-stu-id="adf9b-255">Request</span></span>
<span data-ttu-id="adf9b-256">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="adf9b-256">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1284

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true,
  "signingCertificateType": "certificate",
  "encryptionCertificateType": "certificate"
}
```

### <a name="response"></a><span data-ttu-id="adf9b-257">応答</span><span class="sxs-lookup"><span data-stu-id="adf9b-257">Response</span></span>
<span data-ttu-id="adf9b-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="adf9b-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1456

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "id": "e03086da-86da-e030-da86-30e0da8630e0",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true,
  "signingCertificateType": "certificate",
  "encryptionCertificateType": "certificate"
}
```




