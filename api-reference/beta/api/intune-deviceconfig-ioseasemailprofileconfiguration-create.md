---
title: IosEasEmailProfileConfiguration を作成します。
description: 新しい iosEasEmailProfileConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b325d251d65df5b76562d12d331d12bf388b9a39
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955423"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="d2127-103">IosEasEmailProfileConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="d2127-103">Create iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="d2127-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d2127-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2127-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2127-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2127-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d2127-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2127-107">新しい[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d2127-107">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d2127-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d2127-108">Prerequisites</span></span>
<span data-ttu-id="d2127-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2127-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2127-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2127-111">Permission type</span></span>|<span data-ttu-id="d2127-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2127-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2127-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d2127-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2127-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2127-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d2127-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2127-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2127-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2127-116">Not supported.</span></span>|
|<span data-ttu-id="d2127-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2127-117">Application</span></span>|<span data-ttu-id="d2127-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2127-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2127-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2127-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d2127-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2127-120">Request headers</span></span>
|<span data-ttu-id="d2127-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2127-121">Header</span></span>|<span data-ttu-id="d2127-122">値</span><span class="sxs-lookup"><span data-stu-id="d2127-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2127-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2127-123">Authorization</span></span>|<span data-ttu-id="d2127-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d2127-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2127-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d2127-125">Accept</span></span>|<span data-ttu-id="d2127-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2127-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2127-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2127-127">Request body</span></span>
<span data-ttu-id="d2127-128">要求の本文に iosEasEmailProfileConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="d2127-128">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="d2127-129">次の表は、iosEasEmailProfileConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d2127-129">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="d2127-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2127-130">Property</span></span>|<span data-ttu-id="d2127-131">種類</span><span class="sxs-lookup"><span data-stu-id="d2127-131">Type</span></span>|<span data-ttu-id="d2127-132">説明</span><span class="sxs-lookup"><span data-stu-id="d2127-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2127-133">ID</span><span class="sxs-lookup"><span data-stu-id="d2127-133">id</span></span>|<span data-ttu-id="d2127-134">String</span><span class="sxs-lookup"><span data-stu-id="d2127-134">String</span></span>|<span data-ttu-id="d2127-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d2127-135">Key of the entity.</span></span> <span data-ttu-id="d2127-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2127-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2127-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2127-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d2127-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2127-138">DateTimeOffset</span></span>|<span data-ttu-id="d2127-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d2127-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d2127-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2127-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2127-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d2127-141">roleScopeTagIds</span></span>|<span data-ttu-id="d2127-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d2127-142">String collection</span></span>|<span data-ttu-id="d2127-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="d2127-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d2127-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2127-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2127-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d2127-145">supportsScopeTags</span></span>|<span data-ttu-id="d2127-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="d2127-146">Boolean</span></span>|<span data-ttu-id="d2127-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d2127-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d2127-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="d2127-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d2127-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="d2127-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d2127-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="d2127-150">This property is read-only.</span></span> <span data-ttu-id="d2127-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2127-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2127-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d2127-152">createdDateTime</span></span>|<span data-ttu-id="d2127-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2127-153">DateTimeOffset</span></span>|<span data-ttu-id="d2127-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d2127-154">DateTime the object was created.</span></span> <span data-ttu-id="d2127-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2127-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2127-156">説明</span><span class="sxs-lookup"><span data-stu-id="d2127-156">description</span></span>|<span data-ttu-id="d2127-157">String</span><span class="sxs-lookup"><span data-stu-id="d2127-157">String</span></span>|<span data-ttu-id="d2127-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="d2127-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d2127-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2127-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2127-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d2127-160">displayName</span></span>|<span data-ttu-id="d2127-161">String</span><span class="sxs-lookup"><span data-stu-id="d2127-161">String</span></span>|<span data-ttu-id="d2127-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="d2127-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d2127-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2127-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2127-164">version</span><span class="sxs-lookup"><span data-stu-id="d2127-164">version</span></span>|<span data-ttu-id="d2127-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d2127-165">Int32</span></span>|<span data-ttu-id="d2127-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d2127-166">Version of the device configuration.</span></span> <span data-ttu-id="d2127-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2127-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2127-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="d2127-168">usernameSource</span></span>|[<span data-ttu-id="d2127-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="d2127-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="d2127-170">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー名の属性です。</span><span class="sxs-lookup"><span data-stu-id="d2127-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d2127-171">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="d2127-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="d2127-172">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="d2127-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="d2127-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="d2127-173">usernameAADSource</span></span>|[<span data-ttu-id="d2127-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="d2127-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="d2127-175">AAD フィールドには、電子メール プロファイルのユーザー名を取得するために使用するの名前です。</span><span class="sxs-lookup"><span data-stu-id="d2127-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="d2127-176">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="d2127-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="d2127-177">可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。</span><span class="sxs-lookup"><span data-stu-id="d2127-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="d2127-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="d2127-178">userDomainNameSource</span></span>|[<span data-ttu-id="d2127-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="d2127-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="d2127-180">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー ドメイン名属性です。</span><span class="sxs-lookup"><span data-stu-id="d2127-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d2127-181">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="d2127-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="d2127-182">使用可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="d2127-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="d2127-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="d2127-183">customDomainName</span></span>|<span data-ttu-id="d2127-184">String</span><span class="sxs-lookup"><span data-stu-id="d2127-184">String</span></span>|<span data-ttu-id="d2127-185">カスタム ドメイン名の値は、デバイスにインストールする前に、電子メール プロファイルを生成する際に使用します。</span><span class="sxs-lookup"><span data-stu-id="d2127-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="d2127-186">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="d2127-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="d2127-187">accountName</span><span class="sxs-lookup"><span data-stu-id="d2127-187">accountName</span></span>|<span data-ttu-id="d2127-188">String</span><span class="sxs-lookup"><span data-stu-id="d2127-188">String</span></span>|<span data-ttu-id="d2127-189">アカウントの名前です。</span><span class="sxs-lookup"><span data-stu-id="d2127-189">Account name.</span></span>|
|<span data-ttu-id="d2127-190">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d2127-190">authenticationMethod</span></span>|[<span data-ttu-id="d2127-191">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d2127-191">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="d2127-192">このメール プロファイルの認証方法です。</span><span class="sxs-lookup"><span data-stu-id="d2127-192">Authentication method for this Email profile.</span></span> <span data-ttu-id="d2127-193">使用可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="d2127-193">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="d2127-194">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="d2127-194">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="d2127-195">ブール型</span><span class="sxs-lookup"><span data-stu-id="d2127-195">Boolean</span></span>|<span data-ttu-id="d2127-196">他の電子メール アカウントにメッセージを移動をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d2127-196">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="d2127-197">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="d2127-197">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="d2127-198">ブール型</span><span class="sxs-lookup"><span data-stu-id="d2127-198">Boolean</span></span>|<span data-ttu-id="d2127-199">サード パーティ製アプリケーションから電子メールの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d2127-199">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="d2127-200">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="d2127-200">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="d2127-201">ブール型</span><span class="sxs-lookup"><span data-stu-id="d2127-201">Boolean</span></span>|<span data-ttu-id="d2127-202">新しい電子メールを作成するとき、同期中最近使用した電子メール アドレス、-をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d2127-202">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="d2127-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="d2127-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="d2127-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="d2127-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="d2127-205">戻る時の電子メールの継続時間を同期する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d2127-205">Duration of time email should be synced back to.</span></span> <span data-ttu-id="d2127-206">.</span><span class="sxs-lookup"><span data-stu-id="d2127-206"></span></span> <span data-ttu-id="d2127-207">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="d2127-207">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="d2127-208">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="d2127-208">emailAddressSource</span></span>|[<span data-ttu-id="d2127-209">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="d2127-209">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="d2127-210">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたメール属性です。</span><span class="sxs-lookup"><span data-stu-id="d2127-210">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d2127-211">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="d2127-211">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="d2127-212">hostName</span><span class="sxs-lookup"><span data-stu-id="d2127-212">hostName</span></span>|<span data-ttu-id="d2127-213">String</span><span class="sxs-lookup"><span data-stu-id="d2127-213">String</span></span>|<span data-ttu-id="d2127-214">場所 (URL) の交換、ネイティブのメール アプリケーションに接続します。</span><span class="sxs-lookup"><span data-stu-id="d2127-214">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="d2127-215">requireSmime</span><span class="sxs-lookup"><span data-stu-id="d2127-215">requireSmime</span></span>|<span data-ttu-id="d2127-216">ブール型</span><span class="sxs-lookup"><span data-stu-id="d2127-216">Boolean</span></span>|<span data-ttu-id="d2127-217">S/MIME 証明書を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d2127-217">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="d2127-218">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="d2127-218">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="d2127-219">ブール型</span><span class="sxs-lookup"><span data-stu-id="d2127-219">Boolean</span></span>|<span data-ttu-id="d2127-220">暗号化されていない電子メールを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d2127-220">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="d2127-221">requireSsl</span><span class="sxs-lookup"><span data-stu-id="d2127-221">requireSsl</span></span>|<span data-ttu-id="d2127-222">ブール型</span><span class="sxs-lookup"><span data-stu-id="d2127-222">Boolean</span></span>|<span data-ttu-id="d2127-223">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d2127-223">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="d2127-224">useOAuth</span><span class="sxs-lookup"><span data-stu-id="d2127-224">useOAuth</span></span>|<span data-ttu-id="d2127-225">ブール型</span><span class="sxs-lookup"><span data-stu-id="d2127-225">Boolean</span></span>|<span data-ttu-id="d2127-226">接続が認証に OAuth を使用する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d2127-226">Specifies whether the connection should use OAuth for authentication.</span></span>|



## <a name="response"></a><span data-ttu-id="d2127-227">応答</span><span class="sxs-lookup"><span data-stu-id="d2127-227">Response</span></span>
<span data-ttu-id="d2127-228">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d2127-228">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2127-229">例</span><span class="sxs-lookup"><span data-stu-id="d2127-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="d2127-230">要求</span><span class="sxs-lookup"><span data-stu-id="d2127-230">Request</span></span>
<span data-ttu-id="d2127-231">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d2127-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 974

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
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

### <a name="response"></a><span data-ttu-id="d2127-232">応答</span><span class="sxs-lookup"><span data-stu-id="d2127-232">Response</span></span>
<span data-ttu-id="d2127-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d2127-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





