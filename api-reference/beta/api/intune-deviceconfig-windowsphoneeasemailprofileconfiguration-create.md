---
title: windowsphoneeasemailprofileconfiguration の作成
description: 新しい windowsphoneeasemailprofileconfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5cb552095848bb768159160487f178681511187d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32512531"
---
# <a name="create-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="95fd2-103">windowsphoneeasemailprofileconfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="95fd2-103">Create windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="95fd2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95fd2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95fd2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="95fd2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95fd2-106">新しい[windowsphoneeasemailprofileconfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="95fd2-106">Create a new [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95fd2-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="95fd2-107">Prerequisites</span></span>
<span data-ttu-id="95fd2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95fd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95fd2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95fd2-110">Permission type</span></span>|<span data-ttu-id="95fd2-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="95fd2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95fd2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95fd2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95fd2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95fd2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95fd2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95fd2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95fd2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95fd2-115">Not supported.</span></span>|
|<span data-ttu-id="95fd2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95fd2-116">Application</span></span>|<span data-ttu-id="95fd2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95fd2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95fd2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95fd2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="95fd2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95fd2-119">Request headers</span></span>
|<span data-ttu-id="95fd2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95fd2-120">Header</span></span>|<span data-ttu-id="95fd2-121">値</span><span class="sxs-lookup"><span data-stu-id="95fd2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95fd2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="95fd2-122">Authorization</span></span>|<span data-ttu-id="95fd2-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="95fd2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95fd2-124">承諾</span><span class="sxs-lookup"><span data-stu-id="95fd2-124">Accept</span></span>|<span data-ttu-id="95fd2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95fd2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95fd2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="95fd2-126">Request body</span></span>
<span data-ttu-id="95fd2-127">要求本文で、windowsphoneeasemailprofileconfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="95fd2-127">In the request body, supply a JSON representation for the windowsPhoneEASEmailProfileConfiguration object.</span></span>

<span data-ttu-id="95fd2-128">次の表に、windowsphoneeasemailprofileconfiguration 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="95fd2-128">The following table shows the properties that are required when you create the windowsPhoneEASEmailProfileConfiguration.</span></span>

|<span data-ttu-id="95fd2-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95fd2-129">Property</span></span>|<span data-ttu-id="95fd2-130">型</span><span class="sxs-lookup"><span data-stu-id="95fd2-130">Type</span></span>|<span data-ttu-id="95fd2-131">説明</span><span class="sxs-lookup"><span data-stu-id="95fd2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95fd2-132">id</span><span class="sxs-lookup"><span data-stu-id="95fd2-132">id</span></span>|<span data-ttu-id="95fd2-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="95fd2-133">String</span></span>|<span data-ttu-id="95fd2-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="95fd2-134">Key of the entity.</span></span> <span data-ttu-id="95fd2-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95fd2-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95fd2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95fd2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="95fd2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95fd2-137">DateTimeOffset</span></span>|<span data-ttu-id="95fd2-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="95fd2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="95fd2-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95fd2-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95fd2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95fd2-140">roleScopeTagIds</span></span>|<span data-ttu-id="95fd2-141">String collection</span><span class="sxs-lookup"><span data-stu-id="95fd2-141">String collection</span></span>|<span data-ttu-id="95fd2-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="95fd2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="95fd2-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95fd2-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95fd2-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="95fd2-144">supportsScopeTags</span></span>|<span data-ttu-id="95fd2-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="95fd2-145">Boolean</span></span>|<span data-ttu-id="95fd2-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="95fd2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="95fd2-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="95fd2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="95fd2-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="95fd2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="95fd2-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="95fd2-149">This property is read-only.</span></span> <span data-ttu-id="95fd2-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95fd2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95fd2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95fd2-151">createdDateTime</span></span>|<span data-ttu-id="95fd2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95fd2-152">DateTimeOffset</span></span>|<span data-ttu-id="95fd2-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="95fd2-153">DateTime the object was created.</span></span> <span data-ttu-id="95fd2-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95fd2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95fd2-155">説明</span><span class="sxs-lookup"><span data-stu-id="95fd2-155">description</span></span>|<span data-ttu-id="95fd2-156">String</span><span class="sxs-lookup"><span data-stu-id="95fd2-156">String</span></span>|<span data-ttu-id="95fd2-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="95fd2-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="95fd2-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95fd2-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95fd2-159">displayName</span><span class="sxs-lookup"><span data-stu-id="95fd2-159">displayName</span></span>|<span data-ttu-id="95fd2-160">String</span><span class="sxs-lookup"><span data-stu-id="95fd2-160">String</span></span>|<span data-ttu-id="95fd2-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="95fd2-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="95fd2-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95fd2-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95fd2-163">version</span><span class="sxs-lookup"><span data-stu-id="95fd2-163">version</span></span>|<span data-ttu-id="95fd2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="95fd2-164">Int32</span></span>|<span data-ttu-id="95fd2-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="95fd2-165">Version of the device configuration.</span></span> <span data-ttu-id="95fd2-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95fd2-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95fd2-167">usernameSource</span><span class="sxs-lookup"><span data-stu-id="95fd2-167">usernameSource</span></span>|[<span data-ttu-id="95fd2-168">useremailsource</span><span class="sxs-lookup"><span data-stu-id="95fd2-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="95fd2-169">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="95fd2-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="95fd2-170">[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="95fd2-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="95fd2-171">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="95fd2-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="95fd2-172">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="95fd2-172">usernameAADSource</span></span>|[<span data-ttu-id="95fd2-173">usernameSource</span><span class="sxs-lookup"><span data-stu-id="95fd2-173">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="95fd2-174">メールプロファイルのユーザー名を取得するために使用される AAD フィールドの名前。</span><span class="sxs-lookup"><span data-stu-id="95fd2-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="95fd2-175">[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="95fd2-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="95fd2-176">使用可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。</span><span class="sxs-lookup"><span data-stu-id="95fd2-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="95fd2-177">userdomainnamesource</span><span class="sxs-lookup"><span data-stu-id="95fd2-177">userDomainNameSource</span></span>|[<span data-ttu-id="95fd2-178">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="95fd2-178">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="95fd2-179">userdomainname 属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="95fd2-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="95fd2-180">[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="95fd2-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="95fd2-181">可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="95fd2-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="95fd2-182">customdomainname</span><span class="sxs-lookup"><span data-stu-id="95fd2-182">customDomainName</span></span>|<span data-ttu-id="95fd2-183">String</span><span class="sxs-lookup"><span data-stu-id="95fd2-183">String</span></span>|<span data-ttu-id="95fd2-184">デバイスにインストールする前に電子メールプロファイルを生成するときに使用するカスタムドメイン名の値。</span><span class="sxs-lookup"><span data-stu-id="95fd2-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="95fd2-185">[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="95fd2-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="95fd2-186">アカウント</span><span class="sxs-lookup"><span data-stu-id="95fd2-186">accountName</span></span>|<span data-ttu-id="95fd2-187">String</span><span class="sxs-lookup"><span data-stu-id="95fd2-187">String</span></span>|<span data-ttu-id="95fd2-188">アカウント名。</span><span class="sxs-lookup"><span data-stu-id="95fd2-188">Account name.</span></span>|
|<span data-ttu-id="95fd2-189">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="95fd2-189">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="95fd2-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="95fd2-190">Boolean</span></span>|<span data-ttu-id="95fd2-191">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="95fd2-191">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="95fd2-192">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="95fd2-192">This property is read-only.</span></span>|
|<span data-ttu-id="95fd2-193">synccalendar</span><span class="sxs-lookup"><span data-stu-id="95fd2-193">syncCalendar</span></span>|<span data-ttu-id="95fd2-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="95fd2-194">Boolean</span></span>|<span data-ttu-id="95fd2-195">予定表を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="95fd2-195">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="95fd2-196">synccontacts</span><span class="sxs-lookup"><span data-stu-id="95fd2-196">syncContacts</span></span>|<span data-ttu-id="95fd2-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="95fd2-197">Boolean</span></span>|<span data-ttu-id="95fd2-198">連絡先を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="95fd2-198">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="95fd2-199">synctasks</span><span class="sxs-lookup"><span data-stu-id="95fd2-199">syncTasks</span></span>|<span data-ttu-id="95fd2-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="95fd2-200">Boolean</span></span>|<span data-ttu-id="95fd2-201">タスクを同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="95fd2-201">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="95fd2-202">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="95fd2-202">durationOfEmailToSync</span></span>|[<span data-ttu-id="95fd2-203">emailsyncduration</span><span class="sxs-lookup"><span data-stu-id="95fd2-203">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="95fd2-204">同期する電子メールの期間。可能な値は`userDefined`、 `oneDay`、 `threeDays` `oneWeek` `twoWeeks` `oneMonth`、、、、 `unlimited`、です。</span><span class="sxs-lookup"><span data-stu-id="95fd2-204">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="95fd2-205">emailaddresssource</span><span class="sxs-lookup"><span data-stu-id="95fd2-205">emailAddressSource</span></span>|[<span data-ttu-id="95fd2-206">useremailsource</span><span class="sxs-lookup"><span data-stu-id="95fd2-206">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="95fd2-207">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="95fd2-207">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="95fd2-208">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="95fd2-208">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="95fd2-209">emailsyncschedule</span><span class="sxs-lookup"><span data-stu-id="95fd2-209">emailSyncSchedule</span></span>|[<span data-ttu-id="95fd2-210">emailsyncschedule</span><span class="sxs-lookup"><span data-stu-id="95fd2-210">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="95fd2-211">電子メール同期スケジュール。</span><span class="sxs-lookup"><span data-stu-id="95fd2-211">Email sync schedule.</span></span> <span data-ttu-id="95fd2-212">可能な値は、`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage` です。</span><span class="sxs-lookup"><span data-stu-id="95fd2-212">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="95fd2-213">hostName</span><span class="sxs-lookup"><span data-stu-id="95fd2-213">hostName</span></span>|<span data-ttu-id="95fd2-214">String</span><span class="sxs-lookup"><span data-stu-id="95fd2-214">String</span></span>|<span data-ttu-id="95fd2-215">ネイティブメールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="95fd2-215">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="95fd2-216">requireSsl</span><span class="sxs-lookup"><span data-stu-id="95fd2-216">requireSsl</span></span>|<span data-ttu-id="95fd2-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="95fd2-217">Boolean</span></span>|<span data-ttu-id="95fd2-218">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="95fd2-218">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="95fd2-219">応答</span><span class="sxs-lookup"><span data-stu-id="95fd2-219">Response</span></span>
<span data-ttu-id="95fd2-220">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsphoneeasemailprofileconfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="95fd2-220">If successful, this method returns a `201 Created` response code and a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95fd2-221">例</span><span class="sxs-lookup"><span data-stu-id="95fd2-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="95fd2-222">要求</span><span class="sxs-lookup"><span data-stu-id="95fd2-222">Request</span></span>
<span data-ttu-id="95fd2-223">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="95fd2-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 794

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
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

### <a name="response"></a><span data-ttu-id="95fd2-224">応答</span><span class="sxs-lookup"><span data-stu-id="95fd2-224">Response</span></span>
<span data-ttu-id="95fd2-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="95fd2-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





