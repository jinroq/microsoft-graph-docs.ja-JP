---
title: WindowsPhoneEASEmailProfileConfiguration を作成します。
description: 新しい windowsPhoneEASEmailProfileConfiguration オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 13de3b6a81ee18e170c88e1811d9dd02223eb579
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329940"
---
# <a name="create-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="36920-103">WindowsPhoneEASEmailProfileConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="36920-103">Create windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="36920-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="36920-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36920-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36920-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36920-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="36920-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36920-107">新しい[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="36920-107">Create a new [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36920-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="36920-108">Prerequisites</span></span>
<span data-ttu-id="36920-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36920-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36920-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="36920-111">Permission type</span></span>|<span data-ttu-id="36920-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="36920-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36920-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="36920-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36920-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36920-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="36920-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="36920-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36920-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36920-116">Not supported.</span></span>|
|<span data-ttu-id="36920-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="36920-117">Application</span></span>|<span data-ttu-id="36920-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36920-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36920-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="36920-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="36920-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36920-120">Request headers</span></span>
|<span data-ttu-id="36920-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36920-121">Header</span></span>|<span data-ttu-id="36920-122">値</span><span class="sxs-lookup"><span data-stu-id="36920-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36920-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36920-123">Authorization</span></span>|<span data-ttu-id="36920-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="36920-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36920-125">Accept</span><span class="sxs-lookup"><span data-stu-id="36920-125">Accept</span></span>|<span data-ttu-id="36920-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36920-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36920-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="36920-127">Request body</span></span>
<span data-ttu-id="36920-128">要求の本文に windowsPhoneEASEmailProfileConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="36920-128">In the request body, supply a JSON representation for the windowsPhoneEASEmailProfileConfiguration object.</span></span>

<span data-ttu-id="36920-129">次の表は、windowsPhoneEASEmailProfileConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="36920-129">The following table shows the properties that are required when you create the windowsPhoneEASEmailProfileConfiguration.</span></span>

|<span data-ttu-id="36920-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36920-130">Property</span></span>|<span data-ttu-id="36920-131">種類</span><span class="sxs-lookup"><span data-stu-id="36920-131">Type</span></span>|<span data-ttu-id="36920-132">説明</span><span class="sxs-lookup"><span data-stu-id="36920-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36920-133">ID</span><span class="sxs-lookup"><span data-stu-id="36920-133">id</span></span>|<span data-ttu-id="36920-134">String</span><span class="sxs-lookup"><span data-stu-id="36920-134">String</span></span>|<span data-ttu-id="36920-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="36920-135">Key of the entity.</span></span> <span data-ttu-id="36920-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36920-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36920-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="36920-137">lastModifiedDateTime</span></span>|<span data-ttu-id="36920-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36920-138">DateTimeOffset</span></span>|<span data-ttu-id="36920-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="36920-139">DateTime the object was last modified.</span></span> <span data-ttu-id="36920-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36920-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36920-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="36920-141">roleScopeTagIds</span></span>|<span data-ttu-id="36920-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="36920-142">String collection</span></span>|<span data-ttu-id="36920-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="36920-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="36920-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36920-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36920-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="36920-145">supportsScopeTags</span></span>|<span data-ttu-id="36920-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="36920-146">Boolean</span></span>|<span data-ttu-id="36920-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="36920-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="36920-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="36920-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="36920-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="36920-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="36920-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="36920-150">This property is read-only.</span></span> <span data-ttu-id="36920-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36920-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36920-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36920-152">createdDateTime</span></span>|<span data-ttu-id="36920-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36920-153">DateTimeOffset</span></span>|<span data-ttu-id="36920-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="36920-154">DateTime the object was created.</span></span> <span data-ttu-id="36920-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36920-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36920-156">説明</span><span class="sxs-lookup"><span data-stu-id="36920-156">description</span></span>|<span data-ttu-id="36920-157">String</span><span class="sxs-lookup"><span data-stu-id="36920-157">String</span></span>|<span data-ttu-id="36920-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="36920-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="36920-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36920-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36920-160">displayName</span><span class="sxs-lookup"><span data-stu-id="36920-160">displayName</span></span>|<span data-ttu-id="36920-161">String</span><span class="sxs-lookup"><span data-stu-id="36920-161">String</span></span>|<span data-ttu-id="36920-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="36920-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="36920-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36920-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36920-164">version</span><span class="sxs-lookup"><span data-stu-id="36920-164">version</span></span>|<span data-ttu-id="36920-165">Int32</span><span class="sxs-lookup"><span data-stu-id="36920-165">Int32</span></span>|<span data-ttu-id="36920-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="36920-166">Version of the device configuration.</span></span> <span data-ttu-id="36920-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="36920-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36920-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="36920-168">usernameSource</span></span>|[<span data-ttu-id="36920-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="36920-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="36920-170">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー名の属性です。</span><span class="sxs-lookup"><span data-stu-id="36920-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="36920-171">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="36920-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="36920-172">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="36920-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="36920-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="36920-173">usernameAADSource</span></span>|[<span data-ttu-id="36920-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="36920-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="36920-175">AAD フィールドには、電子メール プロファイルのユーザー名を取得するために使用するの名前です。</span><span class="sxs-lookup"><span data-stu-id="36920-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="36920-176">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="36920-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="36920-177">可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。</span><span class="sxs-lookup"><span data-stu-id="36920-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="36920-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="36920-178">userDomainNameSource</span></span>|[<span data-ttu-id="36920-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="36920-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="36920-180">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー ドメイン名属性です。</span><span class="sxs-lookup"><span data-stu-id="36920-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="36920-181">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="36920-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="36920-182">使用可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="36920-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="36920-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="36920-183">customDomainName</span></span>|<span data-ttu-id="36920-184">String</span><span class="sxs-lookup"><span data-stu-id="36920-184">String</span></span>|<span data-ttu-id="36920-185">カスタム ドメイン名の値は、デバイスにインストールする前に、電子メール プロファイルを生成する際に使用します。</span><span class="sxs-lookup"><span data-stu-id="36920-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="36920-186">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="36920-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="36920-187">accountName</span><span class="sxs-lookup"><span data-stu-id="36920-187">accountName</span></span>|<span data-ttu-id="36920-188">String</span><span class="sxs-lookup"><span data-stu-id="36920-188">String</span></span>|<span data-ttu-id="36920-189">アカウントの名前です。</span><span class="sxs-lookup"><span data-stu-id="36920-189">Account name.</span></span>|
|<span data-ttu-id="36920-190">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="36920-190">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="36920-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="36920-191">Boolean</span></span>|<span data-ttu-id="36920-192">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="36920-192">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="36920-193">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="36920-193">This property is read-only.</span></span>|
|<span data-ttu-id="36920-194">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="36920-194">syncCalendar</span></span>|<span data-ttu-id="36920-195">ブール型</span><span class="sxs-lookup"><span data-stu-id="36920-195">Boolean</span></span>|<span data-ttu-id="36920-196">予定表を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="36920-196">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="36920-197">syncContacts</span><span class="sxs-lookup"><span data-stu-id="36920-197">syncContacts</span></span>|<span data-ttu-id="36920-198">ブール型</span><span class="sxs-lookup"><span data-stu-id="36920-198">Boolean</span></span>|<span data-ttu-id="36920-199">連絡先を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="36920-199">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="36920-200">syncTasks</span><span class="sxs-lookup"><span data-stu-id="36920-200">syncTasks</span></span>|<span data-ttu-id="36920-201">ブール型</span><span class="sxs-lookup"><span data-stu-id="36920-201">Boolean</span></span>|<span data-ttu-id="36920-202">タスクを同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="36920-202">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="36920-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="36920-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="36920-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="36920-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="36920-205">同期するメールの期間です。使用可能な値: `userDefined`、 `oneDay`、 `threeDays`、 `oneWeek`、 `twoWeeks`、 `oneMonth`、 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="36920-205">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="36920-206">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="36920-206">emailAddressSource</span></span>|[<span data-ttu-id="36920-207">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="36920-207">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="36920-208">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたメール属性です。</span><span class="sxs-lookup"><span data-stu-id="36920-208">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="36920-209">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="36920-209">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="36920-210">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="36920-210">emailSyncSchedule</span></span>|[<span data-ttu-id="36920-211">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="36920-211">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="36920-212">電子メールの同期のスケジュールです。</span><span class="sxs-lookup"><span data-stu-id="36920-212">Email sync schedule.</span></span> <span data-ttu-id="36920-213">可能な値は、`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage` です。</span><span class="sxs-lookup"><span data-stu-id="36920-213">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="36920-214">hostName</span><span class="sxs-lookup"><span data-stu-id="36920-214">hostName</span></span>|<span data-ttu-id="36920-215">String</span><span class="sxs-lookup"><span data-stu-id="36920-215">String</span></span>|<span data-ttu-id="36920-216">場所 (URL) の交換、ネイティブのメール アプリケーションに接続します。</span><span class="sxs-lookup"><span data-stu-id="36920-216">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="36920-217">requireSsl</span><span class="sxs-lookup"><span data-stu-id="36920-217">requireSsl</span></span>|<span data-ttu-id="36920-218">ブール型</span><span class="sxs-lookup"><span data-stu-id="36920-218">Boolean</span></span>|<span data-ttu-id="36920-219">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="36920-219">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="36920-220">応答</span><span class="sxs-lookup"><span data-stu-id="36920-220">Response</span></span>
<span data-ttu-id="36920-221">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="36920-221">If successful, this method returns a `201 Created` response code and a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36920-222">例</span><span class="sxs-lookup"><span data-stu-id="36920-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="36920-223">要求</span><span class="sxs-lookup"><span data-stu-id="36920-223">Request</span></span>
<span data-ttu-id="36920-224">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="36920-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 858

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
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
  "applyOnlyToWindowsPhone81": true,
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSsl": true
}
```

### <a name="response"></a><span data-ttu-id="36920-225">応答</span><span class="sxs-lookup"><span data-stu-id="36920-225">Response</span></span>
<span data-ttu-id="36920-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="36920-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 966

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
  "id": "554f402a-402a-554f-2a40-4f552a404f55",
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
  "applyOnlyToWindowsPhone81": true,
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSsl": true
}
```





