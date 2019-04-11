---
title: windowsphoneeasemailprofileconfiguration の更新
description: windowsphoneeasemailprofileconfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b29dc72efd5cbea575cf874f18d95a7252efb02
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792826"
---
# <a name="update-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="9f48c-103">windowsphoneeasemailprofileconfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="9f48c-103">Update windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="9f48c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f48c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f48c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9f48c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f48c-106">[windowsphoneeasemailprofileconfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9f48c-106">Update the properties of a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f48c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9f48c-107">Prerequisites</span></span>
<span data-ttu-id="9f48c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f48c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f48c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9f48c-110">Permission type</span></span>|<span data-ttu-id="9f48c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9f48c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f48c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9f48c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f48c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f48c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f48c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9f48c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f48c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f48c-115">Not supported.</span></span>|
|<span data-ttu-id="9f48c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9f48c-116">Application</span></span>|<span data-ttu-id="9f48c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f48c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f48c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9f48c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9f48c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9f48c-119">Request headers</span></span>
|<span data-ttu-id="9f48c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9f48c-120">Header</span></span>|<span data-ttu-id="9f48c-121">値</span><span class="sxs-lookup"><span data-stu-id="9f48c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f48c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f48c-122">Authorization</span></span>|<span data-ttu-id="9f48c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9f48c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f48c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9f48c-124">Accept</span></span>|<span data-ttu-id="9f48c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f48c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f48c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9f48c-126">Request body</span></span>
<span data-ttu-id="9f48c-127">要求本文で、 [windowsphoneeasemailprofileconfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9f48c-127">In the request body, supply a JSON representation for the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="9f48c-128">次の表に、 [windowsphoneeasemailprofileconfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9f48c-128">The following table shows the properties that are required when you create the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="9f48c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f48c-129">Property</span></span>|<span data-ttu-id="9f48c-130">型</span><span class="sxs-lookup"><span data-stu-id="9f48c-130">Type</span></span>|<span data-ttu-id="9f48c-131">説明</span><span class="sxs-lookup"><span data-stu-id="9f48c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f48c-132">id</span><span class="sxs-lookup"><span data-stu-id="9f48c-132">id</span></span>|<span data-ttu-id="9f48c-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9f48c-133">String</span></span>|<span data-ttu-id="9f48c-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9f48c-134">Key of the entity.</span></span> <span data-ttu-id="9f48c-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f48c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f48c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f48c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9f48c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f48c-137">DateTimeOffset</span></span>|<span data-ttu-id="9f48c-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="9f48c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9f48c-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f48c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f48c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9f48c-140">roleScopeTagIds</span></span>|<span data-ttu-id="9f48c-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9f48c-141">String collection</span></span>|<span data-ttu-id="9f48c-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="9f48c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9f48c-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f48c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f48c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9f48c-144">supportsScopeTags</span></span>|<span data-ttu-id="9f48c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f48c-145">Boolean</span></span>|<span data-ttu-id="9f48c-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9f48c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9f48c-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="9f48c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9f48c-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="9f48c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9f48c-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="9f48c-149">This property is read-only.</span></span> <span data-ttu-id="9f48c-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f48c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f48c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f48c-151">createdDateTime</span></span>|<span data-ttu-id="9f48c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f48c-152">DateTimeOffset</span></span>|<span data-ttu-id="9f48c-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9f48c-153">DateTime the object was created.</span></span> <span data-ttu-id="9f48c-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f48c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f48c-155">説明</span><span class="sxs-lookup"><span data-stu-id="9f48c-155">description</span></span>|<span data-ttu-id="9f48c-156">String</span><span class="sxs-lookup"><span data-stu-id="9f48c-156">String</span></span>|<span data-ttu-id="9f48c-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="9f48c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9f48c-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f48c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f48c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9f48c-159">displayName</span></span>|<span data-ttu-id="9f48c-160">String</span><span class="sxs-lookup"><span data-stu-id="9f48c-160">String</span></span>|<span data-ttu-id="9f48c-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="9f48c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9f48c-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f48c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f48c-163">version</span><span class="sxs-lookup"><span data-stu-id="9f48c-163">version</span></span>|<span data-ttu-id="9f48c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9f48c-164">Int32</span></span>|<span data-ttu-id="9f48c-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9f48c-165">Version of the device configuration.</span></span> <span data-ttu-id="9f48c-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f48c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f48c-167">usernameSource</span><span class="sxs-lookup"><span data-stu-id="9f48c-167">usernameSource</span></span>|[<span data-ttu-id="9f48c-168">useremailsource</span><span class="sxs-lookup"><span data-stu-id="9f48c-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="9f48c-169">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="9f48c-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9f48c-170">[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="9f48c-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="9f48c-171">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="9f48c-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="9f48c-172">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="9f48c-172">usernameAADSource</span></span>|[<span data-ttu-id="9f48c-173">usernameSource</span><span class="sxs-lookup"><span data-stu-id="9f48c-173">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="9f48c-174">メールプロファイルのユーザー名を取得するために使用される AAD フィールドの名前。</span><span class="sxs-lookup"><span data-stu-id="9f48c-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="9f48c-175">[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="9f48c-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="9f48c-176">使用可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。</span><span class="sxs-lookup"><span data-stu-id="9f48c-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="9f48c-177">userdomainnamesource</span><span class="sxs-lookup"><span data-stu-id="9f48c-177">userDomainNameSource</span></span>|[<span data-ttu-id="9f48c-178">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="9f48c-178">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="9f48c-179">userdomainname 属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="9f48c-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9f48c-180">[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="9f48c-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="9f48c-181">可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="9f48c-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="9f48c-182">customdomainname</span><span class="sxs-lookup"><span data-stu-id="9f48c-182">customDomainName</span></span>|<span data-ttu-id="9f48c-183">文字列</span><span class="sxs-lookup"><span data-stu-id="9f48c-183">String</span></span>|<span data-ttu-id="9f48c-184">デバイスにインストールする前に電子メールプロファイルを生成するときに使用するカスタムドメイン名の値。</span><span class="sxs-lookup"><span data-stu-id="9f48c-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="9f48c-185">[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="9f48c-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="9f48c-186">アカウント</span><span class="sxs-lookup"><span data-stu-id="9f48c-186">accountName</span></span>|<span data-ttu-id="9f48c-187">文字列</span><span class="sxs-lookup"><span data-stu-id="9f48c-187">String</span></span>|<span data-ttu-id="9f48c-188">アカウント名。</span><span class="sxs-lookup"><span data-stu-id="9f48c-188">Account name.</span></span>|
|<span data-ttu-id="9f48c-189">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="9f48c-189">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="9f48c-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f48c-190">Boolean</span></span>|<span data-ttu-id="9f48c-191">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="9f48c-191">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="9f48c-192">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9f48c-192">This property is read-only.</span></span>|
|<span data-ttu-id="9f48c-193">synccalendar</span><span class="sxs-lookup"><span data-stu-id="9f48c-193">syncCalendar</span></span>|<span data-ttu-id="9f48c-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f48c-194">Boolean</span></span>|<span data-ttu-id="9f48c-195">予定表を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9f48c-195">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="9f48c-196">synccontacts</span><span class="sxs-lookup"><span data-stu-id="9f48c-196">syncContacts</span></span>|<span data-ttu-id="9f48c-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f48c-197">Boolean</span></span>|<span data-ttu-id="9f48c-198">連絡先を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9f48c-198">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="9f48c-199">synctasks</span><span class="sxs-lookup"><span data-stu-id="9f48c-199">syncTasks</span></span>|<span data-ttu-id="9f48c-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f48c-200">Boolean</span></span>|<span data-ttu-id="9f48c-201">タスクを同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9f48c-201">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="9f48c-202">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="9f48c-202">durationOfEmailToSync</span></span>|[<span data-ttu-id="9f48c-203">emailsyncduration</span><span class="sxs-lookup"><span data-stu-id="9f48c-203">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="9f48c-204">同期する電子メールの期間。可能な値は`userDefined`、 `oneDay`、 `threeDays` `oneWeek` `twoWeeks` `oneMonth`、、、、 `unlimited`、です。</span><span class="sxs-lookup"><span data-stu-id="9f48c-204">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="9f48c-205">emailaddresssource</span><span class="sxs-lookup"><span data-stu-id="9f48c-205">emailAddressSource</span></span>|[<span data-ttu-id="9f48c-206">useremailsource</span><span class="sxs-lookup"><span data-stu-id="9f48c-206">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="9f48c-207">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="9f48c-207">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9f48c-208">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="9f48c-208">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="9f48c-209">emailsyncschedule</span><span class="sxs-lookup"><span data-stu-id="9f48c-209">emailSyncSchedule</span></span>|[<span data-ttu-id="9f48c-210">emailsyncschedule</span><span class="sxs-lookup"><span data-stu-id="9f48c-210">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="9f48c-211">電子メール同期スケジュール。</span><span class="sxs-lookup"><span data-stu-id="9f48c-211">Email sync schedule.</span></span> <span data-ttu-id="9f48c-212">可能な値は、`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage` です。</span><span class="sxs-lookup"><span data-stu-id="9f48c-212">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="9f48c-213">hostName</span><span class="sxs-lookup"><span data-stu-id="9f48c-213">hostName</span></span>|<span data-ttu-id="9f48c-214">String</span><span class="sxs-lookup"><span data-stu-id="9f48c-214">String</span></span>|<span data-ttu-id="9f48c-215">ネイティブメールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="9f48c-215">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="9f48c-216">requireSsl</span><span class="sxs-lookup"><span data-stu-id="9f48c-216">requireSsl</span></span>|<span data-ttu-id="9f48c-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f48c-217">Boolean</span></span>|<span data-ttu-id="9f48c-218">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9f48c-218">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="9f48c-219">応答</span><span class="sxs-lookup"><span data-stu-id="9f48c-219">Response</span></span>
<span data-ttu-id="9f48c-220">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsphoneeasemailprofileconfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9f48c-220">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f48c-221">例</span><span class="sxs-lookup"><span data-stu-id="9f48c-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f48c-222">要求</span><span class="sxs-lookup"><span data-stu-id="9f48c-222">Request</span></span>
<span data-ttu-id="9f48c-223">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9f48c-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="9f48c-224">応答</span><span class="sxs-lookup"><span data-stu-id="9f48c-224">Response</span></span>
<span data-ttu-id="9f48c-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9f48c-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





