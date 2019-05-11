---
title: Windows10EasEmailProfileConfiguration の更新
description: Windows10EasEmailProfileConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b576569b8efc836884b920eaff01e7db0b89ee5
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33921836"
---
# <a name="update-windows10easemailprofileconfiguration"></a><span data-ttu-id="e7382-103">Windows10EasEmailProfileConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="e7382-103">Update windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="e7382-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7382-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7382-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e7382-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7382-106">[Windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e7382-106">Update the properties of a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7382-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e7382-107">Prerequisites</span></span>
<span data-ttu-id="e7382-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7382-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7382-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7382-110">Permission type</span></span>|<span data-ttu-id="e7382-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7382-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7382-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e7382-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7382-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7382-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7382-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7382-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7382-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7382-115">Not supported.</span></span>|
|<span data-ttu-id="e7382-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7382-116">Application</span></span>|<span data-ttu-id="e7382-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7382-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7382-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7382-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e7382-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7382-119">Request headers</span></span>
|<span data-ttu-id="e7382-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7382-120">Header</span></span>|<span data-ttu-id="e7382-121">値</span><span class="sxs-lookup"><span data-stu-id="e7382-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7382-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7382-122">Authorization</span></span>|<span data-ttu-id="e7382-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e7382-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7382-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e7382-124">Accept</span></span>|<span data-ttu-id="e7382-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7382-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7382-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e7382-126">Request body</span></span>
<span data-ttu-id="e7382-127">要求本文で、 [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7382-127">In the request body, supply a JSON representation for the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="e7382-128">次の表に、 [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e7382-128">The following table shows the properties that are required when you create the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="e7382-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7382-129">Property</span></span>|<span data-ttu-id="e7382-130">型</span><span class="sxs-lookup"><span data-stu-id="e7382-130">Type</span></span>|<span data-ttu-id="e7382-131">説明</span><span class="sxs-lookup"><span data-stu-id="e7382-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7382-132">id</span><span class="sxs-lookup"><span data-stu-id="e7382-132">id</span></span>|<span data-ttu-id="e7382-133">文字列</span><span class="sxs-lookup"><span data-stu-id="e7382-133">String</span></span>|<span data-ttu-id="e7382-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e7382-134">Key of the entity.</span></span> <span data-ttu-id="e7382-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7382-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7382-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7382-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e7382-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7382-137">DateTimeOffset</span></span>|<span data-ttu-id="e7382-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="e7382-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e7382-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7382-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7382-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e7382-140">roleScopeTagIds</span></span>|<span data-ttu-id="e7382-141">String collection</span><span class="sxs-lookup"><span data-stu-id="e7382-141">String collection</span></span>|<span data-ttu-id="e7382-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="e7382-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e7382-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7382-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7382-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e7382-144">supportsScopeTags</span></span>|<span data-ttu-id="e7382-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7382-145">Boolean</span></span>|<span data-ttu-id="e7382-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e7382-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e7382-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="e7382-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e7382-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="e7382-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e7382-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="e7382-149">This property is read-only.</span></span> <span data-ttu-id="e7382-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7382-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7382-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7382-151">createdDateTime</span></span>|<span data-ttu-id="e7382-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7382-152">DateTimeOffset</span></span>|<span data-ttu-id="e7382-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e7382-153">DateTime the object was created.</span></span> <span data-ttu-id="e7382-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7382-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7382-155">description</span><span class="sxs-lookup"><span data-stu-id="e7382-155">description</span></span>|<span data-ttu-id="e7382-156">String</span><span class="sxs-lookup"><span data-stu-id="e7382-156">String</span></span>|<span data-ttu-id="e7382-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="e7382-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e7382-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7382-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7382-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e7382-159">displayName</span></span>|<span data-ttu-id="e7382-160">String</span><span class="sxs-lookup"><span data-stu-id="e7382-160">String</span></span>|<span data-ttu-id="e7382-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="e7382-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e7382-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7382-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7382-163">version</span><span class="sxs-lookup"><span data-stu-id="e7382-163">version</span></span>|<span data-ttu-id="e7382-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e7382-164">Int32</span></span>|<span data-ttu-id="e7382-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e7382-165">Version of the device configuration.</span></span> <span data-ttu-id="e7382-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7382-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7382-167">usernameSource</span><span class="sxs-lookup"><span data-stu-id="e7382-167">usernameSource</span></span>|[<span data-ttu-id="e7382-168">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="e7382-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="e7382-169">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="e7382-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="e7382-170">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e7382-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="e7382-171">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="e7382-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="e7382-172">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="e7382-172">usernameAADSource</span></span>|[<span data-ttu-id="e7382-173">usernameSource</span><span class="sxs-lookup"><span data-stu-id="e7382-173">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="e7382-174">メールプロファイルのユーザー名を取得するために使用される AAD フィールドの名前。</span><span class="sxs-lookup"><span data-stu-id="e7382-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="e7382-175">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e7382-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="e7382-176">可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。</span><span class="sxs-lookup"><span data-stu-id="e7382-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="e7382-177">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="e7382-177">userDomainNameSource</span></span>|[<span data-ttu-id="e7382-178">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="e7382-178">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="e7382-179">UserDomainname 属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="e7382-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="e7382-180">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e7382-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="e7382-181">可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="e7382-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="e7382-182">customDomainName</span><span class="sxs-lookup"><span data-stu-id="e7382-182">customDomainName</span></span>|<span data-ttu-id="e7382-183">String</span><span class="sxs-lookup"><span data-stu-id="e7382-183">String</span></span>|<span data-ttu-id="e7382-184">デバイスにインストールする前に電子メールプロファイルを生成するときに使用するカスタムドメイン名の値。</span><span class="sxs-lookup"><span data-stu-id="e7382-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="e7382-185">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e7382-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="e7382-186">accountName</span><span class="sxs-lookup"><span data-stu-id="e7382-186">accountName</span></span>|<span data-ttu-id="e7382-187">String</span><span class="sxs-lookup"><span data-stu-id="e7382-187">String</span></span>|<span data-ttu-id="e7382-188">アカウント名。</span><span class="sxs-lookup"><span data-stu-id="e7382-188">Account name.</span></span>|
|<span data-ttu-id="e7382-189">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="e7382-189">syncCalendar</span></span>|<span data-ttu-id="e7382-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7382-190">Boolean</span></span>|<span data-ttu-id="e7382-191">予定表を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e7382-191">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="e7382-192">syncContacts</span><span class="sxs-lookup"><span data-stu-id="e7382-192">syncContacts</span></span>|<span data-ttu-id="e7382-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7382-193">Boolean</span></span>|<span data-ttu-id="e7382-194">連絡先を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e7382-194">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="e7382-195">syncTasks</span><span class="sxs-lookup"><span data-stu-id="e7382-195">syncTasks</span></span>|<span data-ttu-id="e7382-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7382-196">Boolean</span></span>|<span data-ttu-id="e7382-197">タスクを同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e7382-197">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="e7382-198">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="e7382-198">durationOfEmailToSync</span></span>|[<span data-ttu-id="e7382-199">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="e7382-199">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="e7382-200">同期する電子メールの期間。可能な値は`userDefined`、 `oneDay`、 `threeDays` `oneWeek` `twoWeeks` `oneMonth`、、、、 `unlimited`、です。</span><span class="sxs-lookup"><span data-stu-id="e7382-200">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="e7382-201">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="e7382-201">emailAddressSource</span></span>|[<span data-ttu-id="e7382-202">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="e7382-202">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="e7382-203">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="e7382-203">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="e7382-204">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="e7382-204">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="e7382-205">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="e7382-205">emailSyncSchedule</span></span>|[<span data-ttu-id="e7382-206">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="e7382-206">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="e7382-207">電子メール同期スケジュール。</span><span class="sxs-lookup"><span data-stu-id="e7382-207">Email sync schedule.</span></span> <span data-ttu-id="e7382-208">可能な値は、`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage` です。</span><span class="sxs-lookup"><span data-stu-id="e7382-208">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="e7382-209">hostName</span><span class="sxs-lookup"><span data-stu-id="e7382-209">hostName</span></span>|<span data-ttu-id="e7382-210">String</span><span class="sxs-lookup"><span data-stu-id="e7382-210">String</span></span>|<span data-ttu-id="e7382-211">ネイティブメールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="e7382-211">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="e7382-212">requireSsl</span><span class="sxs-lookup"><span data-stu-id="e7382-212">requireSsl</span></span>|<span data-ttu-id="e7382-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7382-213">Boolean</span></span>|<span data-ttu-id="e7382-214">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e7382-214">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="e7382-215">応答</span><span class="sxs-lookup"><span data-stu-id="e7382-215">Response</span></span>
<span data-ttu-id="e7382-216">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e7382-216">If successful, this method returns a `200 OK` response code and an updated [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7382-217">例</span><span class="sxs-lookup"><span data-stu-id="e7382-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7382-218">要求</span><span class="sxs-lookup"><span data-stu-id="e7382-218">Request</span></span>
<span data-ttu-id="e7382-219">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e7382-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 753

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
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

### <a name="response"></a><span data-ttu-id="e7382-220">応答</span><span class="sxs-lookup"><span data-stu-id="e7382-220">Response</span></span>
<span data-ttu-id="e7382-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e7382-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




