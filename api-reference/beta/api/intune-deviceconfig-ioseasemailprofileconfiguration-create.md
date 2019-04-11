---
title: ioseasemailprofileconfiguration 作成
description: 新しい ioseasemailprofileconfiguration このオブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2ce4467b07bbebc79407e170813fe26fece86b5e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801611"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="65d74-103">ioseasemailprofileconfiguration 作成</span><span class="sxs-lookup"><span data-stu-id="65d74-103">Create iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="65d74-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65d74-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65d74-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="65d74-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65d74-106">新しい[ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)このオブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="65d74-106">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65d74-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="65d74-107">Prerequisites</span></span>
<span data-ttu-id="65d74-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65d74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65d74-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65d74-110">Permission type</span></span>|<span data-ttu-id="65d74-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="65d74-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65d74-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65d74-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65d74-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65d74-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65d74-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65d74-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65d74-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65d74-115">Not supported.</span></span>|
|<span data-ttu-id="65d74-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65d74-116">Application</span></span>|<span data-ttu-id="65d74-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65d74-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65d74-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65d74-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="65d74-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65d74-119">Request headers</span></span>
|<span data-ttu-id="65d74-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65d74-120">Header</span></span>|<span data-ttu-id="65d74-121">値</span><span class="sxs-lookup"><span data-stu-id="65d74-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65d74-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="65d74-122">Authorization</span></span>|<span data-ttu-id="65d74-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="65d74-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65d74-124">承諾</span><span class="sxs-lookup"><span data-stu-id="65d74-124">Accept</span></span>|<span data-ttu-id="65d74-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65d74-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65d74-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="65d74-126">Request body</span></span>
<span data-ttu-id="65d74-127">要求本文で、ioseasemailprofileconfiguration このオブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="65d74-127">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="65d74-128">次の表に、ioseasemailprofileconfiguration 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="65d74-128">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="65d74-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65d74-129">Property</span></span>|<span data-ttu-id="65d74-130">型</span><span class="sxs-lookup"><span data-stu-id="65d74-130">Type</span></span>|<span data-ttu-id="65d74-131">説明</span><span class="sxs-lookup"><span data-stu-id="65d74-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65d74-132">id</span><span class="sxs-lookup"><span data-stu-id="65d74-132">id</span></span>|<span data-ttu-id="65d74-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="65d74-133">String</span></span>|<span data-ttu-id="65d74-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="65d74-134">Key of the entity.</span></span> <span data-ttu-id="65d74-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="65d74-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65d74-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="65d74-136">lastModifiedDateTime</span></span>|<span data-ttu-id="65d74-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65d74-137">DateTimeOffset</span></span>|<span data-ttu-id="65d74-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="65d74-138">DateTime the object was last modified.</span></span> <span data-ttu-id="65d74-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="65d74-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65d74-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="65d74-140">roleScopeTagIds</span></span>|<span data-ttu-id="65d74-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="65d74-141">String collection</span></span>|<span data-ttu-id="65d74-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="65d74-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="65d74-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="65d74-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65d74-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="65d74-144">supportsScopeTags</span></span>|<span data-ttu-id="65d74-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="65d74-145">Boolean</span></span>|<span data-ttu-id="65d74-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="65d74-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="65d74-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="65d74-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="65d74-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="65d74-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="65d74-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="65d74-149">This property is read-only.</span></span> <span data-ttu-id="65d74-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="65d74-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65d74-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65d74-151">createdDateTime</span></span>|<span data-ttu-id="65d74-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65d74-152">DateTimeOffset</span></span>|<span data-ttu-id="65d74-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="65d74-153">DateTime the object was created.</span></span> <span data-ttu-id="65d74-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="65d74-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65d74-155">説明</span><span class="sxs-lookup"><span data-stu-id="65d74-155">description</span></span>|<span data-ttu-id="65d74-156">String</span><span class="sxs-lookup"><span data-stu-id="65d74-156">String</span></span>|<span data-ttu-id="65d74-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="65d74-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="65d74-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="65d74-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65d74-159">displayName</span><span class="sxs-lookup"><span data-stu-id="65d74-159">displayName</span></span>|<span data-ttu-id="65d74-160">String</span><span class="sxs-lookup"><span data-stu-id="65d74-160">String</span></span>|<span data-ttu-id="65d74-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="65d74-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="65d74-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="65d74-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65d74-163">version</span><span class="sxs-lookup"><span data-stu-id="65d74-163">version</span></span>|<span data-ttu-id="65d74-164">Int32</span><span class="sxs-lookup"><span data-stu-id="65d74-164">Int32</span></span>|<span data-ttu-id="65d74-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="65d74-165">Version of the device configuration.</span></span> <span data-ttu-id="65d74-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="65d74-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65d74-167">usernameSource</span><span class="sxs-lookup"><span data-stu-id="65d74-167">usernameSource</span></span>|[<span data-ttu-id="65d74-168">useremailsource</span><span class="sxs-lookup"><span data-stu-id="65d74-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="65d74-169">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="65d74-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="65d74-170">[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="65d74-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="65d74-171">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="65d74-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="65d74-172">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="65d74-172">usernameAADSource</span></span>|[<span data-ttu-id="65d74-173">usernameSource</span><span class="sxs-lookup"><span data-stu-id="65d74-173">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="65d74-174">メールプロファイルのユーザー名を取得するために使用される AAD フィールドの名前。</span><span class="sxs-lookup"><span data-stu-id="65d74-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="65d74-175">[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="65d74-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="65d74-176">使用可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。</span><span class="sxs-lookup"><span data-stu-id="65d74-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="65d74-177">userdomainnamesource</span><span class="sxs-lookup"><span data-stu-id="65d74-177">userDomainNameSource</span></span>|[<span data-ttu-id="65d74-178">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="65d74-178">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="65d74-179">userdomainname 属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="65d74-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="65d74-180">[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="65d74-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="65d74-181">可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="65d74-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="65d74-182">customdomainname</span><span class="sxs-lookup"><span data-stu-id="65d74-182">customDomainName</span></span>|<span data-ttu-id="65d74-183">文字列</span><span class="sxs-lookup"><span data-stu-id="65d74-183">String</span></span>|<span data-ttu-id="65d74-184">デバイスにインストールする前に電子メールプロファイルを生成するときに使用するカスタムドメイン名の値。</span><span class="sxs-lookup"><span data-stu-id="65d74-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="65d74-185">[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="65d74-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="65d74-186">アカウント</span><span class="sxs-lookup"><span data-stu-id="65d74-186">accountName</span></span>|<span data-ttu-id="65d74-187">文字列</span><span class="sxs-lookup"><span data-stu-id="65d74-187">String</span></span>|<span data-ttu-id="65d74-188">アカウント名。</span><span class="sxs-lookup"><span data-stu-id="65d74-188">Account name.</span></span>|
|<span data-ttu-id="65d74-189">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="65d74-189">authenticationMethod</span></span>|[<span data-ttu-id="65d74-190">easauthenticationmethod</span><span class="sxs-lookup"><span data-stu-id="65d74-190">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="65d74-191">この電子メールプロファイルの認証方法。</span><span class="sxs-lookup"><span data-stu-id="65d74-191">Authentication method for this Email profile.</span></span> <span data-ttu-id="65d74-192">可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="65d74-192">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="65d74-193">blockmovingmessagestooruncommand/電子メールアカウント</span><span class="sxs-lookup"><span data-stu-id="65d74-193">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="65d74-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="65d74-194">Boolean</span></span>|<span data-ttu-id="65d74-195">他の電子メールアカウントへのメッセージの移動をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="65d74-195">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="65d74-196">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="65d74-196">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="65d74-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="65d74-197">Boolean</span></span>|<span data-ttu-id="65d74-198">サードパーティ製アプリからの電子メールの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="65d74-198">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="65d74-199">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="65d74-199">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="65d74-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="65d74-200">Boolean</span></span>|<span data-ttu-id="65d74-201">最近使用した電子メールアドレスの同期をブロックするかどうかを示します (たとえば、新しい電子メールを作成する場合)。</span><span class="sxs-lookup"><span data-stu-id="65d74-201">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="65d74-202">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="65d74-202">durationOfEmailToSync</span></span>|[<span data-ttu-id="65d74-203">emailsyncduration</span><span class="sxs-lookup"><span data-stu-id="65d74-203">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="65d74-204">電子メールを同期する時間。</span><span class="sxs-lookup"><span data-stu-id="65d74-204">Duration of time email should be synced back to.</span></span> <span data-ttu-id="65d74-205">.</span><span class="sxs-lookup"><span data-stu-id="65d74-205"></span></span> <span data-ttu-id="65d74-206">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="65d74-206">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="65d74-207">emailaddresssource</span><span class="sxs-lookup"><span data-stu-id="65d74-207">emailAddressSource</span></span>|[<span data-ttu-id="65d74-208">useremailsource</span><span class="sxs-lookup"><span data-stu-id="65d74-208">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="65d74-209">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="65d74-209">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="65d74-210">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="65d74-210">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="65d74-211">hostName</span><span class="sxs-lookup"><span data-stu-id="65d74-211">hostName</span></span>|<span data-ttu-id="65d74-212">String</span><span class="sxs-lookup"><span data-stu-id="65d74-212">String</span></span>|<span data-ttu-id="65d74-213">ネイティブメールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="65d74-213">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="65d74-214">requireSmime</span><span class="sxs-lookup"><span data-stu-id="65d74-214">requireSmime</span></span>|<span data-ttu-id="65d74-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="65d74-215">Boolean</span></span>|<span data-ttu-id="65d74-216">S/MIME 証明書を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="65d74-216">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="65d74-217">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="65d74-217">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="65d74-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="65d74-218">Boolean</span></span>|<span data-ttu-id="65d74-219">暗号化されていない電子メールを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="65d74-219">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="65d74-220">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="65d74-220">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="65d74-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="65d74-221">Boolean</span></span>|<span data-ttu-id="65d74-222">true S/MIME 暗号化に設定すると、既定で有効になります。</span><span class="sxs-lookup"><span data-stu-id="65d74-222">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="65d74-223">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="65d74-223">smimeSigningEnabled</span></span>|<span data-ttu-id="65d74-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="65d74-224">Boolean</span></span>|<span data-ttu-id="65d74-225">このアカウントに対して true S/MIME 署名を有効に設定した場合</span><span class="sxs-lookup"><span data-stu-id="65d74-225">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="65d74-226">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="65d74-226">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="65d74-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="65d74-227">Boolean</span></span>|<span data-ttu-id="65d74-228">true に設定されている場合、ユーザーは S/MIME の署名のオンとオフを切り替えることができます。</span><span class="sxs-lookup"><span data-stu-id="65d74-228">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="65d74-229">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="65d74-229">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="65d74-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="65d74-230">Boolean</span></span>|<span data-ttu-id="65d74-231">true に設定されている場合、ユーザーは既定の設定で暗号化を切り替えることができます。</span><span class="sxs-lookup"><span data-stu-id="65d74-231">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="65d74-232">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="65d74-232">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="65d74-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="65d74-233">Boolean</span></span>|<span data-ttu-id="65d74-234">true に設定されている場合、ユーザーは署名 id を選択できます。</span><span class="sxs-lookup"><span data-stu-id="65d74-234">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="65d74-235">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="65d74-235">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="65d74-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="65d74-236">Boolean</span></span>|<span data-ttu-id="65d74-237">true に設定されている場合、ユーザーは S/MIME 暗号化 id を選択できます。</span><span class="sxs-lookup"><span data-stu-id="65d74-237">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="65d74-238">requireSsl</span><span class="sxs-lookup"><span data-stu-id="65d74-238">requireSsl</span></span>|<span data-ttu-id="65d74-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="65d74-239">Boolean</span></span>|<span data-ttu-id="65d74-240">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="65d74-240">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="65d74-241">useoauth</span><span class="sxs-lookup"><span data-stu-id="65d74-241">useOAuth</span></span>|<span data-ttu-id="65d74-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="65d74-242">Boolean</span></span>|<span data-ttu-id="65d74-243">接続で認証に OAuth を使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="65d74-243">Specifies whether the connection should use OAuth for authentication.</span></span>|



## <a name="response"></a><span data-ttu-id="65d74-244">応答</span><span class="sxs-lookup"><span data-stu-id="65d74-244">Response</span></span>
<span data-ttu-id="65d74-245">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) "オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="65d74-245">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65d74-246">例</span><span class="sxs-lookup"><span data-stu-id="65d74-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="65d74-247">要求</span><span class="sxs-lookup"><span data-stu-id="65d74-247">Request</span></span>
<span data-ttu-id="65d74-248">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="65d74-248">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1193

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
  "useOAuth": true
}
```

### <a name="response"></a><span data-ttu-id="65d74-249">応答</span><span class="sxs-lookup"><span data-stu-id="65d74-249">Response</span></span>
<span data-ttu-id="65d74-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="65d74-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1365

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
  "useOAuth": true
}
```





