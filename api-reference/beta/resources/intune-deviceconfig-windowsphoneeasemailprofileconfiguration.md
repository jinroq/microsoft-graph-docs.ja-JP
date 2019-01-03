---
title: windowsPhoneEASEmailProfileConfiguration リソースの種類
description: このプロファイルの構成を提供することによって、Exchange サーバーと通信し、電子メール、連絡先、カレンダー、およびタスクを取得する Windows Phone 上のネイティブの電子メール クライアントに指示できます。 さらに、同期とデバイスを同期する必要がありますどのくらいの頻度にどのくらいのメールを指定することもできます。
ms.openlocfilehash: 262371cd3cfc9b94002fd8275be90ec6177cdb00
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073201"
---
# <a name="windowsphoneeasemailprofileconfiguration-resource-type"></a><span data-ttu-id="8a2bb-104">windowsPhoneEASEmailProfileConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8a2bb-104">windowsPhoneEASEmailProfileConfiguration resource type</span></span>

> <span data-ttu-id="8a2bb-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a2bb-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a2bb-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a2bb-108">このプロファイルの構成を提供することによって、Exchange サーバーと通信し、電子メール、連絡先、カレンダー、およびタスクを取得する Windows Phone 上のネイティブの電子メール クライアントに指示できます。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-108">By providing configurations in this profile you can instruct the native email client on Windows Phone to communicate with an Exchange server and get email, contacts, calendar, and tasks.</span></span> <span data-ttu-id="8a2bb-109">さらに、同期とデバイスを同期する必要がありますどのくらいの頻度にどのくらいのメールを指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-109">Furthermore, you can also specify how much email to sync and how often the device should sync.</span></span>

<span data-ttu-id="8a2bb-110">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-110">Inherits from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>

## <a name="methods"></a><span data-ttu-id="8a2bb-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="8a2bb-111">Methods</span></span>
|<span data-ttu-id="8a2bb-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="8a2bb-112">Method</span></span>|<span data-ttu-id="8a2bb-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8a2bb-113">Return Type</span></span>|<span data-ttu-id="8a2bb-114">説明</span><span class="sxs-lookup"><span data-stu-id="8a2bb-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8a2bb-115">リスト windowsPhoneEASEmailProfileConfigurations</span><span class="sxs-lookup"><span data-stu-id="8a2bb-115">List windowsPhoneEASEmailProfileConfigurations</span></span>](../api/intune-deviceconfig-windowsphoneeasemailprofileconfiguration-list.md)|<span data-ttu-id="8a2bb-116">[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8a2bb-116">[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) collection</span></span>|<span data-ttu-id="8a2bb-117">[WindowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-117">List properties and relationships of the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="8a2bb-118">WindowsPhoneEASEmailProfileConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-118">Get windowsPhoneEASEmailProfileConfiguration</span></span>](../api/intune-deviceconfig-windowsphoneeasemailprofileconfiguration-get.md)|[<span data-ttu-id="8a2bb-119">windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="8a2bb-119">windowsPhoneEASEmailProfileConfiguration</span></span>](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)|<span data-ttu-id="8a2bb-120">[WindowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-120">Read properties and relationships of the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>|
|[<span data-ttu-id="8a2bb-121">WindowsPhoneEASEmailProfileConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-121">Create windowsPhoneEASEmailProfileConfiguration</span></span>](../api/intune-deviceconfig-windowsphoneeasemailprofileconfiguration-create.md)|[<span data-ttu-id="8a2bb-122">windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="8a2bb-122">windowsPhoneEASEmailProfileConfiguration</span></span>](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)|<span data-ttu-id="8a2bb-123">新しい[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-123">Create a new [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>|
|[<span data-ttu-id="8a2bb-124">WindowsPhoneEASEmailProfileConfiguration を削除します。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-124">Delete windowsPhoneEASEmailProfileConfiguration</span></span>](../api/intune-deviceconfig-windowsphoneeasemailprofileconfiguration-delete.md)|<span data-ttu-id="8a2bb-125">なし</span><span class="sxs-lookup"><span data-stu-id="8a2bb-125">None</span></span>|<span data-ttu-id="8a2bb-126">の[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-126">Deletes a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span></span>|
|[<span data-ttu-id="8a2bb-127">WindowsPhoneEASEmailProfileConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-127">Update windowsPhoneEASEmailProfileConfiguration</span></span>](../api/intune-deviceconfig-windowsphoneeasemailprofileconfiguration-update.md)|[<span data-ttu-id="8a2bb-128">windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="8a2bb-128">windowsPhoneEASEmailProfileConfiguration</span></span>](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)|<span data-ttu-id="8a2bb-129">[WindowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-129">Update the properties of a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8a2bb-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a2bb-130">Properties</span></span>
|<span data-ttu-id="8a2bb-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a2bb-131">Property</span></span>|<span data-ttu-id="8a2bb-132">型</span><span class="sxs-lookup"><span data-stu-id="8a2bb-132">Type</span></span>|<span data-ttu-id="8a2bb-133">説明</span><span class="sxs-lookup"><span data-stu-id="8a2bb-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a2bb-134">id</span><span class="sxs-lookup"><span data-stu-id="8a2bb-134">id</span></span>|<span data-ttu-id="8a2bb-135">String</span><span class="sxs-lookup"><span data-stu-id="8a2bb-135">String</span></span>|<span data-ttu-id="8a2bb-136">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-136">Key of the entity.</span></span> <span data-ttu-id="8a2bb-137">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a2bb-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a2bb-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a2bb-138">lastModifiedDateTime</span></span>|<span data-ttu-id="8a2bb-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a2bb-139">DateTimeOffset</span></span>|<span data-ttu-id="8a2bb-140">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-140">DateTime the object was last modified.</span></span> <span data-ttu-id="8a2bb-141">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a2bb-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a2bb-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8a2bb-142">roleScopeTagIds</span></span>|<span data-ttu-id="8a2bb-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8a2bb-143">String collection</span></span>|<span data-ttu-id="8a2bb-144">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-144">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8a2bb-145">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a2bb-145">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a2bb-146">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8a2bb-146">supportsScopeTags</span></span>|<span data-ttu-id="8a2bb-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a2bb-147">Boolean</span></span>|<span data-ttu-id="8a2bb-148">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-148">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8a2bb-149">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-149">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8a2bb-150">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-150">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8a2bb-151">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-151">This property is read-only.</span></span> <span data-ttu-id="8a2bb-152">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a2bb-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a2bb-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a2bb-153">createdDateTime</span></span>|<span data-ttu-id="8a2bb-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a2bb-154">DateTimeOffset</span></span>|<span data-ttu-id="8a2bb-155">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-155">DateTime the object was created.</span></span> <span data-ttu-id="8a2bb-156">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a2bb-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a2bb-157">説明</span><span class="sxs-lookup"><span data-stu-id="8a2bb-157">description</span></span>|<span data-ttu-id="8a2bb-158">String</span><span class="sxs-lookup"><span data-stu-id="8a2bb-158">String</span></span>|<span data-ttu-id="8a2bb-159">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8a2bb-160">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a2bb-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a2bb-161">displayName</span><span class="sxs-lookup"><span data-stu-id="8a2bb-161">displayName</span></span>|<span data-ttu-id="8a2bb-162">String</span><span class="sxs-lookup"><span data-stu-id="8a2bb-162">String</span></span>|<span data-ttu-id="8a2bb-163">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8a2bb-164">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a2bb-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a2bb-165">version</span><span class="sxs-lookup"><span data-stu-id="8a2bb-165">version</span></span>|<span data-ttu-id="8a2bb-166">Int32</span><span class="sxs-lookup"><span data-stu-id="8a2bb-166">Int32</span></span>|<span data-ttu-id="8a2bb-167">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-167">Version of the device configuration.</span></span> <span data-ttu-id="8a2bb-168">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a2bb-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a2bb-169">usernameSource</span><span class="sxs-lookup"><span data-stu-id="8a2bb-169">usernameSource</span></span>|[<span data-ttu-id="8a2bb-170">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="8a2bb-170">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="8a2bb-171">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー名の属性です。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-171">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="8a2bb-172">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-172">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="8a2bb-173">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-173">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="8a2bb-174">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="8a2bb-174">usernameAADSource</span></span>|[<span data-ttu-id="8a2bb-175">usernameSource</span><span class="sxs-lookup"><span data-stu-id="8a2bb-175">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="8a2bb-176">AAD フィールドには、電子メール プロファイルのユーザー名を取得するために使用するの名前です。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-176">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="8a2bb-177">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-177">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="8a2bb-178">可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-178">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="8a2bb-179">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="8a2bb-179">userDomainNameSource</span></span>|[<span data-ttu-id="8a2bb-180">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="8a2bb-180">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="8a2bb-181">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー ドメイン名属性です。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-181">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="8a2bb-182">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="8a2bb-183">使用可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-183">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="8a2bb-184">customDomainName</span><span class="sxs-lookup"><span data-stu-id="8a2bb-184">customDomainName</span></span>|<span data-ttu-id="8a2bb-185">String</span><span class="sxs-lookup"><span data-stu-id="8a2bb-185">String</span></span>|<span data-ttu-id="8a2bb-186">カスタム ドメイン名の値は、デバイスにインストールする前に、電子メール プロファイルを生成する際に使用します。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-186">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="8a2bb-187">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="8a2bb-188">accountName</span><span class="sxs-lookup"><span data-stu-id="8a2bb-188">accountName</span></span>|<span data-ttu-id="8a2bb-189">String</span><span class="sxs-lookup"><span data-stu-id="8a2bb-189">String</span></span>|<span data-ttu-id="8a2bb-190">アカウントの名前です。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-190">Account name.</span></span>|
|<span data-ttu-id="8a2bb-191">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="8a2bb-191">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="8a2bb-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a2bb-192">Boolean</span></span>|<span data-ttu-id="8a2bb-193">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-193">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="8a2bb-194">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-194">This property is read-only.</span></span>|
|<span data-ttu-id="8a2bb-195">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="8a2bb-195">syncCalendar</span></span>|<span data-ttu-id="8a2bb-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a2bb-196">Boolean</span></span>|<span data-ttu-id="8a2bb-197">予定表を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-197">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="8a2bb-198">syncContacts</span><span class="sxs-lookup"><span data-stu-id="8a2bb-198">syncContacts</span></span>|<span data-ttu-id="8a2bb-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a2bb-199">Boolean</span></span>|<span data-ttu-id="8a2bb-200">連絡先を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-200">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="8a2bb-201">syncTasks</span><span class="sxs-lookup"><span data-stu-id="8a2bb-201">syncTasks</span></span>|<span data-ttu-id="8a2bb-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a2bb-202">Boolean</span></span>|<span data-ttu-id="8a2bb-203">タスクを同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-203">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="8a2bb-204">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="8a2bb-204">durationOfEmailToSync</span></span>|[<span data-ttu-id="8a2bb-205">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="8a2bb-205">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="8a2bb-206">同期するメールの期間です。使用可能な値: `userDefined`、 `oneDay`、 `threeDays`、 `oneWeek`、 `twoWeeks`、 `oneMonth`、 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-206">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="8a2bb-207">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="8a2bb-207">emailAddressSource</span></span>|[<span data-ttu-id="8a2bb-208">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="8a2bb-208">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="8a2bb-209">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたメール属性です。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-209">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="8a2bb-210">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-210">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="8a2bb-211">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="8a2bb-211">emailSyncSchedule</span></span>|[<span data-ttu-id="8a2bb-212">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="8a2bb-212">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="8a2bb-213">電子メールの同期のスケジュールです。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-213">Email sync schedule.</span></span> <span data-ttu-id="8a2bb-214">可能な値は、`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage` です。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-214">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="8a2bb-215">hostName</span><span class="sxs-lookup"><span data-stu-id="8a2bb-215">hostName</span></span>|<span data-ttu-id="8a2bb-216">String</span><span class="sxs-lookup"><span data-stu-id="8a2bb-216">String</span></span>|<span data-ttu-id="8a2bb-217">場所 (URL) の交換、ネイティブのメール アプリケーションに接続します。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-217">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="8a2bb-218">requireSsl</span><span class="sxs-lookup"><span data-stu-id="8a2bb-218">requireSsl</span></span>|<span data-ttu-id="8a2bb-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a2bb-219">Boolean</span></span>|<span data-ttu-id="8a2bb-220">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-220">Indicates whether or not to use SSL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a2bb-221">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8a2bb-221">Relationships</span></span>
|<span data-ttu-id="8a2bb-222">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8a2bb-222">Relationship</span></span>|<span data-ttu-id="8a2bb-223">型</span><span class="sxs-lookup"><span data-stu-id="8a2bb-223">Type</span></span>|<span data-ttu-id="8a2bb-224">説明</span><span class="sxs-lookup"><span data-stu-id="8a2bb-224">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a2bb-225">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="8a2bb-225">groupAssignments</span></span>|<span data-ttu-id="8a2bb-226">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8a2bb-226">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="8a2bb-227">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-227">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="8a2bb-228">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a2bb-228">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a2bb-229">assignments</span><span class="sxs-lookup"><span data-stu-id="8a2bb-229">assignments</span></span>|<span data-ttu-id="8a2bb-230">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8a2bb-230">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="8a2bb-231">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-231">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="8a2bb-232">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a2bb-232">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a2bb-233">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="8a2bb-233">deviceStatuses</span></span>|<span data-ttu-id="8a2bb-234">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8a2bb-234">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="8a2bb-235">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-235">Device configuration installation status by device.</span></span> <span data-ttu-id="8a2bb-236">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a2bb-236">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a2bb-237">userStatuses</span><span class="sxs-lookup"><span data-stu-id="8a2bb-237">userStatuses</span></span>|<span data-ttu-id="8a2bb-238">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8a2bb-238">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="8a2bb-239">ユーザーごとのデバイス構成のインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-239">Device configuration installation status by user.</span></span> <span data-ttu-id="8a2bb-240">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8a2bb-240">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a2bb-241">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="8a2bb-241">deviceStatusOverview</span></span>|[<span data-ttu-id="8a2bb-242">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="8a2bb-242">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="8a2bb-243">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="8a2bb-243">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a2bb-244">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="8a2bb-244">userStatusOverview</span></span>|[<span data-ttu-id="8a2bb-245">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="8a2bb-245">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="8a2bb-246">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="8a2bb-246">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a2bb-247">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="8a2bb-247">deviceSettingStateSummaries</span></span>|<span data-ttu-id="8a2bb-248">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8a2bb-248">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="8a2bb-249">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="8a2bb-249">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a2bb-250">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8a2bb-250">JSON Representation</span></span>
<span data-ttu-id="8a2bb-251">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8a2bb-251">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPhoneEASEmailProfileConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
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
  "applyOnlyToWindowsPhone81": true,
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "emailSyncSchedule": "String",
  "hostName": "String",
  "requireSsl": true
}
```




