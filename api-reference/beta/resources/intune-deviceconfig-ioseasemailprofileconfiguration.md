---
title: iosEasEmailProfileConfiguration リソースの種類
description: このプロファイルの構成を提供することで Exchange サーバーと通信し、電子メール、連絡先、カレンダー、アラーム、およびメモに iOS デバイス上のネイティブの電子メール クライアントに指示できます。 さらに、同期とデバイスを同期する必要がありますどのくらいの頻度にどのくらいのメールを指定することもできます。
ms.openlocfilehash: 4ce93ed8963a6ee82775adbfc8edd14a15b4188d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067804"
---
# <a name="ioseasemailprofileconfiguration-resource-type"></a><span data-ttu-id="a923e-104">iosEasEmailProfileConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a923e-104">iosEasEmailProfileConfiguration resource type</span></span>

> <span data-ttu-id="a923e-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a923e-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a923e-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a923e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a923e-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a923e-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a923e-108">このプロファイルの構成を提供することで Exchange サーバーと通信し、電子メール、連絡先、カレンダー、アラーム、およびメモに iOS デバイス上のネイティブの電子メール クライアントに指示できます。</span><span class="sxs-lookup"><span data-stu-id="a923e-108">By providing configurations in this profile you can instruct the native email client on iOS devices to communicate with an Exchange server and get email, contacts, calendar, reminders, and notes.</span></span> <span data-ttu-id="a923e-109">さらに、同期とデバイスを同期する必要がありますどのくらいの頻度にどのくらいのメールを指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="a923e-109">Furthermore, you can also specify how much email to sync and how often the device should sync.</span></span>

<span data-ttu-id="a923e-110">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a923e-110">Inherits from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a923e-111">Methods</span><span class="sxs-lookup"><span data-stu-id="a923e-111">Methods</span></span>
|<span data-ttu-id="a923e-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="a923e-112">Method</span></span>|<span data-ttu-id="a923e-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a923e-113">Return Type</span></span>|<span data-ttu-id="a923e-114">説明</span><span class="sxs-lookup"><span data-stu-id="a923e-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a923e-115">リスト iosEasEmailProfileConfigurations</span><span class="sxs-lookup"><span data-stu-id="a923e-115">List iosEasEmailProfileConfigurations</span></span>](../api/intune-deviceconfig-ioseasemailprofileconfiguration-list.md)|<span data-ttu-id="a923e-116">[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a923e-116">[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) collection</span></span>|<span data-ttu-id="a923e-117">[IosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="a923e-117">List properties and relationships of the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="a923e-118">IosEasEmailProfileConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="a923e-118">Get iosEasEmailProfileConfiguration</span></span>](../api/intune-deviceconfig-ioseasemailprofileconfiguration-get.md)|[<span data-ttu-id="a923e-119">iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="a923e-119">iosEasEmailProfileConfiguration</span></span>](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|<span data-ttu-id="a923e-120">[IosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a923e-120">Read properties and relationships of the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>|
|[<span data-ttu-id="a923e-121">IosEasEmailProfileConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="a923e-121">Create iosEasEmailProfileConfiguration</span></span>](../api/intune-deviceconfig-ioseasemailprofileconfiguration-create.md)|[<span data-ttu-id="a923e-122">iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="a923e-122">iosEasEmailProfileConfiguration</span></span>](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|<span data-ttu-id="a923e-123">新しい[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a923e-123">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>|
|[<span data-ttu-id="a923e-124">IosEasEmailProfileConfiguration を削除します。</span><span class="sxs-lookup"><span data-stu-id="a923e-124">Delete iosEasEmailProfileConfiguration</span></span>](../api/intune-deviceconfig-ioseasemailprofileconfiguration-delete.md)|<span data-ttu-id="a923e-125">なし</span><span class="sxs-lookup"><span data-stu-id="a923e-125">None</span></span>|<span data-ttu-id="a923e-126">の[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="a923e-126">Deletes a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>|
|[<span data-ttu-id="a923e-127">IosEasEmailProfileConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="a923e-127">Update iosEasEmailProfileConfiguration</span></span>](../api/intune-deviceconfig-ioseasemailprofileconfiguration-update.md)|[<span data-ttu-id="a923e-128">iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="a923e-128">iosEasEmailProfileConfiguration</span></span>](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|<span data-ttu-id="a923e-129">[IosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a923e-129">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a923e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a923e-130">Properties</span></span>
|<span data-ttu-id="a923e-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a923e-131">Property</span></span>|<span data-ttu-id="a923e-132">型</span><span class="sxs-lookup"><span data-stu-id="a923e-132">Type</span></span>|<span data-ttu-id="a923e-133">説明</span><span class="sxs-lookup"><span data-stu-id="a923e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a923e-134">id</span><span class="sxs-lookup"><span data-stu-id="a923e-134">id</span></span>|<span data-ttu-id="a923e-135">String</span><span class="sxs-lookup"><span data-stu-id="a923e-135">String</span></span>|<span data-ttu-id="a923e-136">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a923e-136">Key of the entity.</span></span> <span data-ttu-id="a923e-137">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a923e-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a923e-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a923e-138">lastModifiedDateTime</span></span>|<span data-ttu-id="a923e-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a923e-139">DateTimeOffset</span></span>|<span data-ttu-id="a923e-140">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a923e-140">DateTime the object was last modified.</span></span> <span data-ttu-id="a923e-141">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a923e-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a923e-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a923e-142">roleScopeTagIds</span></span>|<span data-ttu-id="a923e-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a923e-143">String collection</span></span>|<span data-ttu-id="a923e-144">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="a923e-144">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a923e-145">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a923e-145">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a923e-146">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a923e-146">supportsScopeTags</span></span>|<span data-ttu-id="a923e-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="a923e-147">Boolean</span></span>|<span data-ttu-id="a923e-148">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a923e-148">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a923e-149">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="a923e-149">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a923e-150">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="a923e-150">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a923e-151">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="a923e-151">This property is read-only.</span></span> <span data-ttu-id="a923e-152">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a923e-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a923e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a923e-153">createdDateTime</span></span>|<span data-ttu-id="a923e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a923e-154">DateTimeOffset</span></span>|<span data-ttu-id="a923e-155">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a923e-155">DateTime the object was created.</span></span> <span data-ttu-id="a923e-156">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a923e-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a923e-157">説明</span><span class="sxs-lookup"><span data-stu-id="a923e-157">description</span></span>|<span data-ttu-id="a923e-158">String</span><span class="sxs-lookup"><span data-stu-id="a923e-158">String</span></span>|<span data-ttu-id="a923e-159">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="a923e-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a923e-160">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a923e-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a923e-161">displayName</span><span class="sxs-lookup"><span data-stu-id="a923e-161">displayName</span></span>|<span data-ttu-id="a923e-162">String</span><span class="sxs-lookup"><span data-stu-id="a923e-162">String</span></span>|<span data-ttu-id="a923e-163">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="a923e-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a923e-164">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a923e-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a923e-165">version</span><span class="sxs-lookup"><span data-stu-id="a923e-165">version</span></span>|<span data-ttu-id="a923e-166">Int32</span><span class="sxs-lookup"><span data-stu-id="a923e-166">Int32</span></span>|<span data-ttu-id="a923e-167">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a923e-167">Version of the device configuration.</span></span> <span data-ttu-id="a923e-168">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a923e-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a923e-169">usernameSource</span><span class="sxs-lookup"><span data-stu-id="a923e-169">usernameSource</span></span>|[<span data-ttu-id="a923e-170">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="a923e-170">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="a923e-171">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー名の属性です。</span><span class="sxs-lookup"><span data-stu-id="a923e-171">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a923e-172">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a923e-172">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="a923e-173">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="a923e-173">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="a923e-174">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="a923e-174">usernameAADSource</span></span>|[<span data-ttu-id="a923e-175">usernameSource</span><span class="sxs-lookup"><span data-stu-id="a923e-175">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="a923e-176">AAD フィールドには、電子メール プロファイルのユーザー名を取得するために使用するの名前です。</span><span class="sxs-lookup"><span data-stu-id="a923e-176">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="a923e-177">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a923e-177">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="a923e-178">可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。</span><span class="sxs-lookup"><span data-stu-id="a923e-178">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="a923e-179">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="a923e-179">userDomainNameSource</span></span>|[<span data-ttu-id="a923e-180">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="a923e-180">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="a923e-181">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー ドメイン名属性です。</span><span class="sxs-lookup"><span data-stu-id="a923e-181">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a923e-182">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a923e-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="a923e-183">使用可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="a923e-183">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="a923e-184">customDomainName</span><span class="sxs-lookup"><span data-stu-id="a923e-184">customDomainName</span></span>|<span data-ttu-id="a923e-185">String</span><span class="sxs-lookup"><span data-stu-id="a923e-185">String</span></span>|<span data-ttu-id="a923e-186">カスタム ドメイン名の値は、デバイスにインストールする前に、電子メール プロファイルを生成する際に使用します。</span><span class="sxs-lookup"><span data-stu-id="a923e-186">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="a923e-187">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a923e-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="a923e-188">accountName</span><span class="sxs-lookup"><span data-stu-id="a923e-188">accountName</span></span>|<span data-ttu-id="a923e-189">String</span><span class="sxs-lookup"><span data-stu-id="a923e-189">String</span></span>|<span data-ttu-id="a923e-190">アカウントの名前です。</span><span class="sxs-lookup"><span data-stu-id="a923e-190">Account name.</span></span>|
|<span data-ttu-id="a923e-191">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a923e-191">authenticationMethod</span></span>|[<span data-ttu-id="a923e-192">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a923e-192">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="a923e-193">このメール プロファイルの認証方法です。</span><span class="sxs-lookup"><span data-stu-id="a923e-193">Authentication method for this Email profile.</span></span> <span data-ttu-id="a923e-194">使用可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="a923e-194">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="a923e-195">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="a923e-195">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="a923e-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="a923e-196">Boolean</span></span>|<span data-ttu-id="a923e-197">他の電子メール アカウントにメッセージを移動をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a923e-197">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="a923e-198">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="a923e-198">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="a923e-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="a923e-199">Boolean</span></span>|<span data-ttu-id="a923e-200">サード パーティ製アプリケーションから電子メールの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a923e-200">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="a923e-201">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="a923e-201">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="a923e-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="a923e-202">Boolean</span></span>|<span data-ttu-id="a923e-203">新しい電子メールを作成するとき、同期中最近使用した電子メール アドレス、-をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a923e-203">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="a923e-204">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="a923e-204">durationOfEmailToSync</span></span>|[<span data-ttu-id="a923e-205">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="a923e-205">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="a923e-206">戻る時の電子メールの継続時間を同期する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a923e-206">Duration of time email should be synced back to.</span></span> <span data-ttu-id="a923e-207">.</span><span class="sxs-lookup"><span data-stu-id="a923e-207"></span></span> <span data-ttu-id="a923e-208">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="a923e-208">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="a923e-209">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="a923e-209">emailAddressSource</span></span>|[<span data-ttu-id="a923e-210">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="a923e-210">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="a923e-211">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたメール属性です。</span><span class="sxs-lookup"><span data-stu-id="a923e-211">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a923e-212">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="a923e-212">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="a923e-213">hostName</span><span class="sxs-lookup"><span data-stu-id="a923e-213">hostName</span></span>|<span data-ttu-id="a923e-214">String</span><span class="sxs-lookup"><span data-stu-id="a923e-214">String</span></span>|<span data-ttu-id="a923e-215">場所 (URL) の交換、ネイティブのメール アプリケーションに接続します。</span><span class="sxs-lookup"><span data-stu-id="a923e-215">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="a923e-216">requireSmime</span><span class="sxs-lookup"><span data-stu-id="a923e-216">requireSmime</span></span>|<span data-ttu-id="a923e-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="a923e-217">Boolean</span></span>|<span data-ttu-id="a923e-218">S/MIME 証明書を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a923e-218">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="a923e-219">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="a923e-219">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="a923e-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="a923e-220">Boolean</span></span>|<span data-ttu-id="a923e-221">暗号化されていない電子メールを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a923e-221">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="a923e-222">requireSsl</span><span class="sxs-lookup"><span data-stu-id="a923e-222">requireSsl</span></span>|<span data-ttu-id="a923e-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="a923e-223">Boolean</span></span>|<span data-ttu-id="a923e-224">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a923e-224">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="a923e-225">useOAuth</span><span class="sxs-lookup"><span data-stu-id="a923e-225">useOAuth</span></span>|<span data-ttu-id="a923e-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="a923e-226">Boolean</span></span>|<span data-ttu-id="a923e-227">接続が認証に OAuth を使用する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="a923e-227">Specifies whether the connection should use OAuth for authentication.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a923e-228">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a923e-228">Relationships</span></span>
|<span data-ttu-id="a923e-229">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a923e-229">Relationship</span></span>|<span data-ttu-id="a923e-230">型</span><span class="sxs-lookup"><span data-stu-id="a923e-230">Type</span></span>|<span data-ttu-id="a923e-231">説明</span><span class="sxs-lookup"><span data-stu-id="a923e-231">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a923e-232">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="a923e-232">groupAssignments</span></span>|<span data-ttu-id="a923e-233">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a923e-233">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="a923e-234">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="a923e-234">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="a923e-235">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a923e-235">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a923e-236">assignments</span><span class="sxs-lookup"><span data-stu-id="a923e-236">assignments</span></span>|<span data-ttu-id="a923e-237">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a923e-237">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a923e-238">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="a923e-238">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="a923e-239">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a923e-239">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a923e-240">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="a923e-240">deviceStatuses</span></span>|<span data-ttu-id="a923e-241">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a923e-241">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="a923e-242">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="a923e-242">Device configuration installation status by device.</span></span> <span data-ttu-id="a923e-243">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a923e-243">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a923e-244">userStatuses</span><span class="sxs-lookup"><span data-stu-id="a923e-244">userStatuses</span></span>|<span data-ttu-id="a923e-245">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a923e-245">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="a923e-246">ユーザーごとのデバイス構成のインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="a923e-246">Device configuration installation status by user.</span></span> <span data-ttu-id="a923e-247">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a923e-247">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a923e-248">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a923e-248">deviceStatusOverview</span></span>|[<span data-ttu-id="a923e-249">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a923e-249">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="a923e-250">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a923e-250">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a923e-251">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a923e-251">userStatusOverview</span></span>|[<span data-ttu-id="a923e-252">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="a923e-252">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="a923e-253">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a923e-253">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a923e-254">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="a923e-254">deviceSettingStateSummaries</span></span>|<span data-ttu-id="a923e-255">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a923e-255">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="a923e-256">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="a923e-256">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a923e-257">identityCertificate</span><span class="sxs-lookup"><span data-stu-id="a923e-257">identityCertificate</span></span>|[<span data-ttu-id="a923e-258">iosCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="a923e-258">iosCertificateProfileBase</span></span>](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|<span data-ttu-id="a923e-259">Id の証明書です。</span><span class="sxs-lookup"><span data-stu-id="a923e-259">Identity certificate.</span></span>|
|<span data-ttu-id="a923e-260">smimeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="a923e-260">smimeSigningCertificate</span></span>|[<span data-ttu-id="a923e-261">iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="a923e-261">iosCertificateProfile</span></span>](../resources/intune-deviceconfig-ioscertificateprofile.md)|<span data-ttu-id="a923e-262">S/MIME 署名の証明書です。</span><span class="sxs-lookup"><span data-stu-id="a923e-262">S/MIME signing certificate.</span></span>|
|<span data-ttu-id="a923e-263">smimeEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="a923e-263">smimeEncryptionCertificate</span></span>|[<span data-ttu-id="a923e-264">iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="a923e-264">iosCertificateProfile</span></span>](../resources/intune-deviceconfig-ioscertificateprofile.md)|<span data-ttu-id="a923e-265">S/MIME 暗号化の証明書です。</span><span class="sxs-lookup"><span data-stu-id="a923e-265">S/MIME encryption certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a923e-266">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a923e-266">JSON Representation</span></span>
<span data-ttu-id="a923e-267">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a923e-267">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosEasEmailProfileConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "usernameSource": "String",
  "usernameAADSource": "String",
  "userDomainNameSource": "String",
  "customDomainName": "String",
  "accountName": "String",
  "authenticationMethod": "String",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "hostName": "String",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "requireSsl": true,
  "useOAuth": true
}
```




