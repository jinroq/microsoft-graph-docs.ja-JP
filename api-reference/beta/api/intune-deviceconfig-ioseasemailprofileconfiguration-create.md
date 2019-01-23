---
title: IosEasEmailProfileConfiguration を作成します。
description: 新しい iosEasEmailProfileConfiguration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c7de248c21b0efebdcff07ebac804656dc8ebfde
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404450"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="162cf-103">IosEasEmailProfileConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="162cf-103">Create iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="162cf-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="162cf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="162cf-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="162cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="162cf-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="162cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="162cf-107">新しい[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="162cf-107">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="162cf-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="162cf-108">Prerequisites</span></span>
<span data-ttu-id="162cf-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="162cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="162cf-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="162cf-111">Permission type</span></span>|<span data-ttu-id="162cf-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="162cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="162cf-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="162cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="162cf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="162cf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="162cf-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="162cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="162cf-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="162cf-116">Not supported.</span></span>|
|<span data-ttu-id="162cf-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="162cf-117">Application</span></span>|<span data-ttu-id="162cf-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="162cf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="162cf-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="162cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="162cf-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="162cf-120">Request headers</span></span>
|<span data-ttu-id="162cf-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="162cf-121">Header</span></span>|<span data-ttu-id="162cf-122">値</span><span class="sxs-lookup"><span data-stu-id="162cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="162cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="162cf-123">Authorization</span></span>|<span data-ttu-id="162cf-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="162cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="162cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="162cf-125">Accept</span></span>|<span data-ttu-id="162cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="162cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="162cf-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="162cf-127">Request body</span></span>
<span data-ttu-id="162cf-128">要求の本文に iosEasEmailProfileConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="162cf-128">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="162cf-129">次の表は、iosEasEmailProfileConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="162cf-129">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="162cf-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="162cf-130">Property</span></span>|<span data-ttu-id="162cf-131">型</span><span class="sxs-lookup"><span data-stu-id="162cf-131">Type</span></span>|<span data-ttu-id="162cf-132">説明</span><span class="sxs-lookup"><span data-stu-id="162cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="162cf-133">id</span><span class="sxs-lookup"><span data-stu-id="162cf-133">id</span></span>|<span data-ttu-id="162cf-134">String</span><span class="sxs-lookup"><span data-stu-id="162cf-134">String</span></span>|<span data-ttu-id="162cf-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="162cf-135">Key of the entity.</span></span> <span data-ttu-id="162cf-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="162cf-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="162cf-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="162cf-137">lastModifiedDateTime</span></span>|<span data-ttu-id="162cf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="162cf-138">DateTimeOffset</span></span>|<span data-ttu-id="162cf-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="162cf-139">DateTime the object was last modified.</span></span> <span data-ttu-id="162cf-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="162cf-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="162cf-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="162cf-141">roleScopeTagIds</span></span>|<span data-ttu-id="162cf-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="162cf-142">String collection</span></span>|<span data-ttu-id="162cf-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="162cf-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="162cf-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="162cf-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="162cf-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="162cf-145">supportsScopeTags</span></span>|<span data-ttu-id="162cf-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="162cf-146">Boolean</span></span>|<span data-ttu-id="162cf-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="162cf-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="162cf-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="162cf-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="162cf-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="162cf-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="162cf-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="162cf-150">This property is read-only.</span></span> <span data-ttu-id="162cf-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="162cf-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="162cf-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="162cf-152">createdDateTime</span></span>|<span data-ttu-id="162cf-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="162cf-153">DateTimeOffset</span></span>|<span data-ttu-id="162cf-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="162cf-154">DateTime the object was created.</span></span> <span data-ttu-id="162cf-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="162cf-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="162cf-156">説明</span><span class="sxs-lookup"><span data-stu-id="162cf-156">description</span></span>|<span data-ttu-id="162cf-157">String</span><span class="sxs-lookup"><span data-stu-id="162cf-157">String</span></span>|<span data-ttu-id="162cf-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="162cf-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="162cf-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="162cf-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="162cf-160">displayName</span><span class="sxs-lookup"><span data-stu-id="162cf-160">displayName</span></span>|<span data-ttu-id="162cf-161">String</span><span class="sxs-lookup"><span data-stu-id="162cf-161">String</span></span>|<span data-ttu-id="162cf-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="162cf-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="162cf-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="162cf-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="162cf-164">version</span><span class="sxs-lookup"><span data-stu-id="162cf-164">version</span></span>|<span data-ttu-id="162cf-165">Int32</span><span class="sxs-lookup"><span data-stu-id="162cf-165">Int32</span></span>|<span data-ttu-id="162cf-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="162cf-166">Version of the device configuration.</span></span> <span data-ttu-id="162cf-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="162cf-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="162cf-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="162cf-168">usernameSource</span></span>|[<span data-ttu-id="162cf-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="162cf-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="162cf-170">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー名の属性です。</span><span class="sxs-lookup"><span data-stu-id="162cf-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="162cf-171">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="162cf-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="162cf-172">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="162cf-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="162cf-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="162cf-173">usernameAADSource</span></span>|[<span data-ttu-id="162cf-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="162cf-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="162cf-175">AAD フィールドには、電子メール プロファイルのユーザー名を取得するために使用するの名前です。</span><span class="sxs-lookup"><span data-stu-id="162cf-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="162cf-176">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="162cf-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="162cf-177">可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。</span><span class="sxs-lookup"><span data-stu-id="162cf-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="162cf-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="162cf-178">userDomainNameSource</span></span>|[<span data-ttu-id="162cf-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="162cf-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="162cf-180">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー ドメイン名属性です。</span><span class="sxs-lookup"><span data-stu-id="162cf-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="162cf-181">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="162cf-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="162cf-182">使用可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="162cf-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="162cf-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="162cf-183">customDomainName</span></span>|<span data-ttu-id="162cf-184">String</span><span class="sxs-lookup"><span data-stu-id="162cf-184">String</span></span>|<span data-ttu-id="162cf-185">カスタム ドメイン名の値は、デバイスにインストールする前に、電子メール プロファイルを生成する際に使用します。</span><span class="sxs-lookup"><span data-stu-id="162cf-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="162cf-186">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="162cf-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="162cf-187">accountName</span><span class="sxs-lookup"><span data-stu-id="162cf-187">accountName</span></span>|<span data-ttu-id="162cf-188">String</span><span class="sxs-lookup"><span data-stu-id="162cf-188">String</span></span>|<span data-ttu-id="162cf-189">アカウントの名前です。</span><span class="sxs-lookup"><span data-stu-id="162cf-189">Account name.</span></span>|
|<span data-ttu-id="162cf-190">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="162cf-190">authenticationMethod</span></span>|[<span data-ttu-id="162cf-191">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="162cf-191">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="162cf-192">このメール プロファイルの認証方法です。</span><span class="sxs-lookup"><span data-stu-id="162cf-192">Authentication method for this Email profile.</span></span> <span data-ttu-id="162cf-193">使用可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="162cf-193">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="162cf-194">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="162cf-194">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="162cf-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="162cf-195">Boolean</span></span>|<span data-ttu-id="162cf-196">他の電子メール アカウントにメッセージを移動をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="162cf-196">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="162cf-197">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="162cf-197">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="162cf-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="162cf-198">Boolean</span></span>|<span data-ttu-id="162cf-199">サード パーティ製アプリケーションから電子メールの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="162cf-199">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="162cf-200">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="162cf-200">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="162cf-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="162cf-201">Boolean</span></span>|<span data-ttu-id="162cf-202">新しい電子メールを作成するとき、同期中最近使用した電子メール アドレス、-をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="162cf-202">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="162cf-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="162cf-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="162cf-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="162cf-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="162cf-205">戻る時の電子メールの継続時間を同期する必要があります。</span><span class="sxs-lookup"><span data-stu-id="162cf-205">Duration of time email should be synced back to.</span></span> <span data-ttu-id="162cf-206">.</span><span class="sxs-lookup"><span data-stu-id="162cf-206"></span></span> <span data-ttu-id="162cf-207">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="162cf-207">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="162cf-208">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="162cf-208">emailAddressSource</span></span>|[<span data-ttu-id="162cf-209">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="162cf-209">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="162cf-210">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたメール属性です。</span><span class="sxs-lookup"><span data-stu-id="162cf-210">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="162cf-211">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="162cf-211">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="162cf-212">hostName</span><span class="sxs-lookup"><span data-stu-id="162cf-212">hostName</span></span>|<span data-ttu-id="162cf-213">String</span><span class="sxs-lookup"><span data-stu-id="162cf-213">String</span></span>|<span data-ttu-id="162cf-214">場所 (URL) の交換、ネイティブのメール アプリケーションに接続します。</span><span class="sxs-lookup"><span data-stu-id="162cf-214">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="162cf-215">requireSmime</span><span class="sxs-lookup"><span data-stu-id="162cf-215">requireSmime</span></span>|<span data-ttu-id="162cf-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="162cf-216">Boolean</span></span>|<span data-ttu-id="162cf-217">S/MIME 証明書を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="162cf-217">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="162cf-218">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="162cf-218">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="162cf-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="162cf-219">Boolean</span></span>|<span data-ttu-id="162cf-220">暗号化されていない電子メールを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="162cf-220">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="162cf-221">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="162cf-221">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="162cf-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="162cf-222">Boolean</span></span>|<span data-ttu-id="162cf-223">場合は、S/MIME 暗号化の場合は true に設定が既定で有効にします。</span><span class="sxs-lookup"><span data-stu-id="162cf-223">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="162cf-224">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="162cf-224">smimeSigningEnabled</span></span>|<span data-ttu-id="162cf-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="162cf-225">Boolean</span></span>|<span data-ttu-id="162cf-226">このアカウントの S/MIME 署名を true に設定が有効になっている場合</span><span class="sxs-lookup"><span data-stu-id="162cf-226">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="162cf-227">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="162cf-227">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="162cf-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="162cf-228">Boolean</span></span>|<span data-ttu-id="162cf-229">かどうか true の場合、ユーザーに設定が S/MIME 署名のオンとオフを切り替えることができます。</span><span class="sxs-lookup"><span data-stu-id="162cf-229">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="162cf-230">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="162cf-230">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="162cf-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="162cf-231">Boolean</span></span>|<span data-ttu-id="162cf-232">場合は true の場合、ユーザー設定が既定の設定で暗号化を切り替えることができます。</span><span class="sxs-lookup"><span data-stu-id="162cf-232">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="162cf-233">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="162cf-233">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="162cf-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="162cf-234">Boolean</span></span>|<span data-ttu-id="162cf-235">場合は true、ユーザーを設定するには、署名 id を選択できます。</span><span class="sxs-lookup"><span data-stu-id="162cf-235">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="162cf-236">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="162cf-236">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="162cf-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="162cf-237">Boolean</span></span>|<span data-ttu-id="162cf-238">場合は、ユーザーを true に設定するには、S/MIME 暗号化 id を選択できます。</span><span class="sxs-lookup"><span data-stu-id="162cf-238">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="162cf-239">requireSsl</span><span class="sxs-lookup"><span data-stu-id="162cf-239">requireSsl</span></span>|<span data-ttu-id="162cf-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="162cf-240">Boolean</span></span>|<span data-ttu-id="162cf-241">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="162cf-241">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="162cf-242">useOAuth</span><span class="sxs-lookup"><span data-stu-id="162cf-242">useOAuth</span></span>|<span data-ttu-id="162cf-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="162cf-243">Boolean</span></span>|<span data-ttu-id="162cf-244">接続が認証に OAuth を使用する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="162cf-244">Specifies whether the connection should use OAuth for authentication.</span></span>|



## <a name="response"></a><span data-ttu-id="162cf-245">応答</span><span class="sxs-lookup"><span data-stu-id="162cf-245">Response</span></span>
<span data-ttu-id="162cf-246">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="162cf-246">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="162cf-247">例</span><span class="sxs-lookup"><span data-stu-id="162cf-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="162cf-248">要求</span><span class="sxs-lookup"><span data-stu-id="162cf-248">Request</span></span>
<span data-ttu-id="162cf-249">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="162cf-249">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="162cf-250">応答</span><span class="sxs-lookup"><span data-stu-id="162cf-250">Response</span></span>
<span data-ttu-id="162cf-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="162cf-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




