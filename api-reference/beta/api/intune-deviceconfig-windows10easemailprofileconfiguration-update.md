---
title: Windows10EasEmailProfileConfiguration を更新します。
description: Windows10EasEmailProfileConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 2a548a528542ab82c05bab177dda19c39cd0681b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360313"
---
# <a name="update-windows10easemailprofileconfiguration"></a><span data-ttu-id="06fb6-103">Windows10EasEmailProfileConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="06fb6-103">Update windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="06fb6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="06fb6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06fb6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06fb6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06fb6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="06fb6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06fb6-107">[Windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="06fb6-107">Update the properties of a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06fb6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="06fb6-108">Prerequisites</span></span>
<span data-ttu-id="06fb6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06fb6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06fb6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="06fb6-111">Permission type</span></span>|<span data-ttu-id="06fb6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="06fb6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06fb6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="06fb6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06fb6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06fb6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06fb6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="06fb6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06fb6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06fb6-116">Not supported.</span></span>|
|<span data-ttu-id="06fb6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="06fb6-117">Application</span></span>|<span data-ttu-id="06fb6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06fb6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06fb6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="06fb6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="06fb6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="06fb6-120">Request headers</span></span>
|<span data-ttu-id="06fb6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="06fb6-121">Header</span></span>|<span data-ttu-id="06fb6-122">値</span><span class="sxs-lookup"><span data-stu-id="06fb6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06fb6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="06fb6-123">Authorization</span></span>|<span data-ttu-id="06fb6-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="06fb6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06fb6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="06fb6-125">Accept</span></span>|<span data-ttu-id="06fb6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06fb6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06fb6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="06fb6-127">Request body</span></span>
<span data-ttu-id="06fb6-128">要求の本文に[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="06fb6-128">In the request body, supply a JSON representation for the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="06fb6-129">[Windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="06fb6-129">The following table shows the properties that are required when you create the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="06fb6-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06fb6-130">Property</span></span>|<span data-ttu-id="06fb6-131">種類</span><span class="sxs-lookup"><span data-stu-id="06fb6-131">Type</span></span>|<span data-ttu-id="06fb6-132">説明</span><span class="sxs-lookup"><span data-stu-id="06fb6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06fb6-133">ID</span><span class="sxs-lookup"><span data-stu-id="06fb6-133">id</span></span>|<span data-ttu-id="06fb6-134">String</span><span class="sxs-lookup"><span data-stu-id="06fb6-134">String</span></span>|<span data-ttu-id="06fb6-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="06fb6-135">Key of the entity.</span></span> <span data-ttu-id="06fb6-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="06fb6-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06fb6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06fb6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="06fb6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06fb6-138">DateTimeOffset</span></span>|<span data-ttu-id="06fb6-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="06fb6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="06fb6-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="06fb6-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06fb6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="06fb6-141">roleScopeTagIds</span></span>|<span data-ttu-id="06fb6-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="06fb6-142">String collection</span></span>|<span data-ttu-id="06fb6-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="06fb6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="06fb6-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="06fb6-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06fb6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="06fb6-145">supportsScopeTags</span></span>|<span data-ttu-id="06fb6-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="06fb6-146">Boolean</span></span>|<span data-ttu-id="06fb6-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="06fb6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="06fb6-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="06fb6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="06fb6-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="06fb6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="06fb6-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="06fb6-150">This property is read-only.</span></span> <span data-ttu-id="06fb6-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="06fb6-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06fb6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06fb6-152">createdDateTime</span></span>|<span data-ttu-id="06fb6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06fb6-153">DateTimeOffset</span></span>|<span data-ttu-id="06fb6-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="06fb6-154">DateTime the object was created.</span></span> <span data-ttu-id="06fb6-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="06fb6-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06fb6-156">説明</span><span class="sxs-lookup"><span data-stu-id="06fb6-156">description</span></span>|<span data-ttu-id="06fb6-157">String</span><span class="sxs-lookup"><span data-stu-id="06fb6-157">String</span></span>|<span data-ttu-id="06fb6-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="06fb6-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="06fb6-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="06fb6-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06fb6-160">displayName</span><span class="sxs-lookup"><span data-stu-id="06fb6-160">displayName</span></span>|<span data-ttu-id="06fb6-161">String</span><span class="sxs-lookup"><span data-stu-id="06fb6-161">String</span></span>|<span data-ttu-id="06fb6-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="06fb6-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="06fb6-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="06fb6-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06fb6-164">version</span><span class="sxs-lookup"><span data-stu-id="06fb6-164">version</span></span>|<span data-ttu-id="06fb6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="06fb6-165">Int32</span></span>|<span data-ttu-id="06fb6-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="06fb6-166">Version of the device configuration.</span></span> <span data-ttu-id="06fb6-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="06fb6-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06fb6-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="06fb6-168">usernameSource</span></span>|[<span data-ttu-id="06fb6-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="06fb6-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="06fb6-170">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー名の属性です。</span><span class="sxs-lookup"><span data-stu-id="06fb6-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="06fb6-171">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="06fb6-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="06fb6-172">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="06fb6-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="06fb6-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="06fb6-173">usernameAADSource</span></span>|[<span data-ttu-id="06fb6-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="06fb6-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="06fb6-175">AAD フィールドには、電子メール プロファイルのユーザー名を取得するために使用するの名前です。</span><span class="sxs-lookup"><span data-stu-id="06fb6-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="06fb6-176">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="06fb6-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="06fb6-177">可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。</span><span class="sxs-lookup"><span data-stu-id="06fb6-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="06fb6-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="06fb6-178">userDomainNameSource</span></span>|[<span data-ttu-id="06fb6-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="06fb6-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="06fb6-180">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー ドメイン名属性です。</span><span class="sxs-lookup"><span data-stu-id="06fb6-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="06fb6-181">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="06fb6-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="06fb6-182">使用可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="06fb6-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="06fb6-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="06fb6-183">customDomainName</span></span>|<span data-ttu-id="06fb6-184">String</span><span class="sxs-lookup"><span data-stu-id="06fb6-184">String</span></span>|<span data-ttu-id="06fb6-185">カスタム ドメイン名の値は、デバイスにインストールする前に、電子メール プロファイルを生成する際に使用します。</span><span class="sxs-lookup"><span data-stu-id="06fb6-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="06fb6-186">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="06fb6-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="06fb6-187">accountName</span><span class="sxs-lookup"><span data-stu-id="06fb6-187">accountName</span></span>|<span data-ttu-id="06fb6-188">String</span><span class="sxs-lookup"><span data-stu-id="06fb6-188">String</span></span>|<span data-ttu-id="06fb6-189">アカウントの名前です。</span><span class="sxs-lookup"><span data-stu-id="06fb6-189">Account name.</span></span>|
|<span data-ttu-id="06fb6-190">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="06fb6-190">syncCalendar</span></span>|<span data-ttu-id="06fb6-191">ブール型</span><span class="sxs-lookup"><span data-stu-id="06fb6-191">Boolean</span></span>|<span data-ttu-id="06fb6-192">予定表を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="06fb6-192">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="06fb6-193">syncContacts</span><span class="sxs-lookup"><span data-stu-id="06fb6-193">syncContacts</span></span>|<span data-ttu-id="06fb6-194">ブール型</span><span class="sxs-lookup"><span data-stu-id="06fb6-194">Boolean</span></span>|<span data-ttu-id="06fb6-195">連絡先を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="06fb6-195">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="06fb6-196">syncTasks</span><span class="sxs-lookup"><span data-stu-id="06fb6-196">syncTasks</span></span>|<span data-ttu-id="06fb6-197">ブール型</span><span class="sxs-lookup"><span data-stu-id="06fb6-197">Boolean</span></span>|<span data-ttu-id="06fb6-198">タスクを同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="06fb6-198">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="06fb6-199">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="06fb6-199">durationOfEmailToSync</span></span>|[<span data-ttu-id="06fb6-200">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="06fb6-200">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="06fb6-201">同期するメールの期間です。使用可能な値: `userDefined`、 `oneDay`、 `threeDays`、 `oneWeek`、 `twoWeeks`、 `oneMonth`、 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="06fb6-201">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="06fb6-202">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="06fb6-202">emailAddressSource</span></span>|[<span data-ttu-id="06fb6-203">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="06fb6-203">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="06fb6-204">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたメール属性です。</span><span class="sxs-lookup"><span data-stu-id="06fb6-204">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="06fb6-205">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="06fb6-205">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="06fb6-206">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="06fb6-206">emailSyncSchedule</span></span>|[<span data-ttu-id="06fb6-207">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="06fb6-207">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="06fb6-208">電子メールの同期のスケジュールです。</span><span class="sxs-lookup"><span data-stu-id="06fb6-208">Email sync schedule.</span></span> <span data-ttu-id="06fb6-209">可能な値は、`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage` です。</span><span class="sxs-lookup"><span data-stu-id="06fb6-209">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="06fb6-210">hostName</span><span class="sxs-lookup"><span data-stu-id="06fb6-210">hostName</span></span>|<span data-ttu-id="06fb6-211">String</span><span class="sxs-lookup"><span data-stu-id="06fb6-211">String</span></span>|<span data-ttu-id="06fb6-212">場所 (URL) の交換、ネイティブのメール アプリケーションに接続します。</span><span class="sxs-lookup"><span data-stu-id="06fb6-212">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="06fb6-213">requireSsl</span><span class="sxs-lookup"><span data-stu-id="06fb6-213">requireSsl</span></span>|<span data-ttu-id="06fb6-214">ブール型</span><span class="sxs-lookup"><span data-stu-id="06fb6-214">Boolean</span></span>|<span data-ttu-id="06fb6-215">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="06fb6-215">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="06fb6-216">応答</span><span class="sxs-lookup"><span data-stu-id="06fb6-216">Response</span></span>
<span data-ttu-id="06fb6-217">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="06fb6-217">If successful, this method returns a `200 OK` response code and an updated [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06fb6-218">例</span><span class="sxs-lookup"><span data-stu-id="06fb6-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="06fb6-219">要求</span><span class="sxs-lookup"><span data-stu-id="06fb6-219">Request</span></span>
<span data-ttu-id="06fb6-220">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="06fb6-220">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 741

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

### <a name="response"></a><span data-ttu-id="06fb6-221">応答</span><span class="sxs-lookup"><span data-stu-id="06fb6-221">Response</span></span>
<span data-ttu-id="06fb6-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="06fb6-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 925

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
  "id": "9dc6f073-f073-9dc6-73f0-c69d73f0c69d",
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




