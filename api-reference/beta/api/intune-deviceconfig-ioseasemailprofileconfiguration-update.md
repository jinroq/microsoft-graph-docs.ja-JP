---
title: IosEasEmailProfileConfiguration を更新します。
description: IosEasEmailProfileConfiguration オブジェクトのプロパティを更新します。
ms.openlocfilehash: e73b5e441d99831e8b89b897a09a5809dab6d1ea
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071767"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="2cb1c-103">IosEasEmailProfileConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-103">Update iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="2cb1c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2cb1c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2cb1c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2cb1c-107">[IosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-107">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2cb1c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2cb1c-108">Prerequisites</span></span>
<span data-ttu-id="2cb1c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cb1c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2cb1c-111">Permission type</span></span>|<span data-ttu-id="2cb1c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2cb1c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cb1c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2cb1c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2cb1c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cb1c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2cb1c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2cb1c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cb1c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-116">Not supported.</span></span>|
|<span data-ttu-id="2cb1c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2cb1c-117">Application</span></span>|<span data-ttu-id="2cb1c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cb1c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2cb1c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2cb1c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2cb1c-120">Request headers</span></span>
|<span data-ttu-id="2cb1c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2cb1c-121">Header</span></span>|<span data-ttu-id="2cb1c-122">値</span><span class="sxs-lookup"><span data-stu-id="2cb1c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cb1c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cb1c-123">Authorization</span></span>|<span data-ttu-id="2cb1c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cb1c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2cb1c-125">Accept</span></span>|<span data-ttu-id="2cb1c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2cb1c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cb1c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2cb1c-127">Request body</span></span>
<span data-ttu-id="2cb1c-128">要求の本文に[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-128">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="2cb1c-129">[IosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-129">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="2cb1c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2cb1c-130">Property</span></span>|<span data-ttu-id="2cb1c-131">型</span><span class="sxs-lookup"><span data-stu-id="2cb1c-131">Type</span></span>|<span data-ttu-id="2cb1c-132">説明</span><span class="sxs-lookup"><span data-stu-id="2cb1c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cb1c-133">id</span><span class="sxs-lookup"><span data-stu-id="2cb1c-133">id</span></span>|<span data-ttu-id="2cb1c-134">String</span><span class="sxs-lookup"><span data-stu-id="2cb1c-134">String</span></span>|<span data-ttu-id="2cb1c-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-135">Key of the entity.</span></span> <span data-ttu-id="2cb1c-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2cb1c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cb1c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2cb1c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2cb1c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cb1c-138">DateTimeOffset</span></span>|<span data-ttu-id="2cb1c-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2cb1c-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2cb1c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cb1c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2cb1c-141">roleScopeTagIds</span></span>|<span data-ttu-id="2cb1c-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="2cb1c-142">String collection</span></span>|<span data-ttu-id="2cb1c-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2cb1c-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2cb1c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cb1c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2cb1c-145">supportsScopeTags</span></span>|<span data-ttu-id="2cb1c-146">ブール値</span><span class="sxs-lookup"><span data-stu-id="2cb1c-146">Boolean</span></span>|<span data-ttu-id="2cb1c-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2cb1c-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2cb1c-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2cb1c-150">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-150">This property is read-only.</span></span> <span data-ttu-id="2cb1c-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2cb1c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cb1c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2cb1c-152">createdDateTime</span></span>|<span data-ttu-id="2cb1c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cb1c-153">DateTimeOffset</span></span>|<span data-ttu-id="2cb1c-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-154">DateTime the object was created.</span></span> <span data-ttu-id="2cb1c-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2cb1c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cb1c-156">説明</span><span class="sxs-lookup"><span data-stu-id="2cb1c-156">description</span></span>|<span data-ttu-id="2cb1c-157">String</span><span class="sxs-lookup"><span data-stu-id="2cb1c-157">String</span></span>|<span data-ttu-id="2cb1c-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2cb1c-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2cb1c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cb1c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="2cb1c-160">displayName</span></span>|<span data-ttu-id="2cb1c-161">String</span><span class="sxs-lookup"><span data-stu-id="2cb1c-161">String</span></span>|<span data-ttu-id="2cb1c-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2cb1c-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2cb1c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cb1c-164">version</span><span class="sxs-lookup"><span data-stu-id="2cb1c-164">version</span></span>|<span data-ttu-id="2cb1c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2cb1c-165">Int32</span></span>|<span data-ttu-id="2cb1c-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-166">Version of the device configuration.</span></span> <span data-ttu-id="2cb1c-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2cb1c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2cb1c-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="2cb1c-168">usernameSource</span></span>|[<span data-ttu-id="2cb1c-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="2cb1c-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="2cb1c-170">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー名の属性です。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2cb1c-171">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="2cb1c-172">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="2cb1c-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="2cb1c-173">usernameAADSource</span></span>|[<span data-ttu-id="2cb1c-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="2cb1c-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="2cb1c-175">AAD フィールドには、電子メール プロファイルのユーザー名を取得するために使用するの名前です。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="2cb1c-176">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="2cb1c-177">可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="2cb1c-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="2cb1c-178">userDomainNameSource</span></span>|[<span data-ttu-id="2cb1c-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="2cb1c-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="2cb1c-180">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー ドメイン名属性です。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2cb1c-181">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="2cb1c-182">使用可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="2cb1c-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="2cb1c-183">customDomainName</span></span>|<span data-ttu-id="2cb1c-184">String</span><span class="sxs-lookup"><span data-stu-id="2cb1c-184">String</span></span>|<span data-ttu-id="2cb1c-185">カスタム ドメイン名の値は、デバイスにインストールする前に、電子メール プロファイルを生成する際に使用します。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="2cb1c-186">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="2cb1c-187">accountName</span><span class="sxs-lookup"><span data-stu-id="2cb1c-187">accountName</span></span>|<span data-ttu-id="2cb1c-188">String</span><span class="sxs-lookup"><span data-stu-id="2cb1c-188">String</span></span>|<span data-ttu-id="2cb1c-189">アカウントの名前です。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-189">Account name.</span></span>|
|<span data-ttu-id="2cb1c-190">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2cb1c-190">authenticationMethod</span></span>|[<span data-ttu-id="2cb1c-191">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2cb1c-191">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="2cb1c-192">このメール プロファイルの認証方法です。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-192">Authentication method for this Email profile.</span></span> <span data-ttu-id="2cb1c-193">使用可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-193">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="2cb1c-194">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="2cb1c-194">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="2cb1c-195">ブール値</span><span class="sxs-lookup"><span data-stu-id="2cb1c-195">Boolean</span></span>|<span data-ttu-id="2cb1c-196">他の電子メール アカウントにメッセージを移動をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-196">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="2cb1c-197">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="2cb1c-197">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="2cb1c-198">ブール値</span><span class="sxs-lookup"><span data-stu-id="2cb1c-198">Boolean</span></span>|<span data-ttu-id="2cb1c-199">サード パーティ製アプリケーションから電子メールの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-199">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="2cb1c-200">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="2cb1c-200">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="2cb1c-201">ブール値</span><span class="sxs-lookup"><span data-stu-id="2cb1c-201">Boolean</span></span>|<span data-ttu-id="2cb1c-202">新しい電子メールを作成するとき、同期中最近使用した電子メール アドレス、-をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-202">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="2cb1c-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="2cb1c-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="2cb1c-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="2cb1c-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="2cb1c-205">戻る時の電子メールの継続時間を同期する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-205">Duration of time email should be synced back to.</span></span> <span data-ttu-id="2cb1c-206">.</span><span class="sxs-lookup"><span data-stu-id="2cb1c-206"></span></span> <span data-ttu-id="2cb1c-207">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-207">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="2cb1c-208">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="2cb1c-208">emailAddressSource</span></span>|[<span data-ttu-id="2cb1c-209">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="2cb1c-209">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="2cb1c-210">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたメール属性です。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-210">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2cb1c-211">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-211">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="2cb1c-212">hostName</span><span class="sxs-lookup"><span data-stu-id="2cb1c-212">hostName</span></span>|<span data-ttu-id="2cb1c-213">String</span><span class="sxs-lookup"><span data-stu-id="2cb1c-213">String</span></span>|<span data-ttu-id="2cb1c-214">場所 (URL) の交換、ネイティブのメール アプリケーションに接続します。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-214">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="2cb1c-215">requireSmime</span><span class="sxs-lookup"><span data-stu-id="2cb1c-215">requireSmime</span></span>|<span data-ttu-id="2cb1c-216">ブール値</span><span class="sxs-lookup"><span data-stu-id="2cb1c-216">Boolean</span></span>|<span data-ttu-id="2cb1c-217">S/MIME 証明書を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-217">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="2cb1c-218">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="2cb1c-218">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="2cb1c-219">ブール値</span><span class="sxs-lookup"><span data-stu-id="2cb1c-219">Boolean</span></span>|<span data-ttu-id="2cb1c-220">暗号化されていない電子メールを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-220">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="2cb1c-221">requireSsl</span><span class="sxs-lookup"><span data-stu-id="2cb1c-221">requireSsl</span></span>|<span data-ttu-id="2cb1c-222">ブール値</span><span class="sxs-lookup"><span data-stu-id="2cb1c-222">Boolean</span></span>|<span data-ttu-id="2cb1c-223">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-223">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="2cb1c-224">useOAuth</span><span class="sxs-lookup"><span data-stu-id="2cb1c-224">useOAuth</span></span>|<span data-ttu-id="2cb1c-225">ブール値</span><span class="sxs-lookup"><span data-stu-id="2cb1c-225">Boolean</span></span>|<span data-ttu-id="2cb1c-226">接続が認証に OAuth を使用する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-226">Specifies whether the connection should use OAuth for authentication.</span></span>|



## <a name="response"></a><span data-ttu-id="2cb1c-227">応答</span><span class="sxs-lookup"><span data-stu-id="2cb1c-227">Response</span></span>
<span data-ttu-id="2cb1c-228">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-228">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cb1c-229">例</span><span class="sxs-lookup"><span data-stu-id="2cb1c-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="2cb1c-230">要求</span><span class="sxs-lookup"><span data-stu-id="2cb1c-230">Request</span></span>
<span data-ttu-id="2cb1c-231">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 904

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "requireSsl": true,
  "useOAuth": true
}
```

### <a name="response"></a><span data-ttu-id="2cb1c-232">応答</span><span class="sxs-lookup"><span data-stu-id="2cb1c-232">Response</span></span>
<span data-ttu-id="2cb1c-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2cb1c-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1082

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
  "requireSsl": true,
  "useOAuth": true
}
```





