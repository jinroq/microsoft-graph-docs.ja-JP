---
title: androidwork profilの maileasconfiguration の作成
description: 新しい androidwork profilな maileasconfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3cf1fd8b16b635c9137944f1d0446cd64a97758d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141959"
---
# <a name="create-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="c1306-103">androidwork profilの maileasconfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="c1306-103">Create androidWorkProfileGmailEasConfiguration</span></span>

> <span data-ttu-id="c1306-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1306-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1306-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c1306-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1306-106">新しい[androidwork profilな maileasconfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c1306-106">Create a new [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1306-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c1306-107">Prerequisites</span></span>
<span data-ttu-id="c1306-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c1306-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c1306-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c1306-110">Permission type</span></span>|<span data-ttu-id="c1306-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c1306-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1306-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c1306-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1306-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1306-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1306-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c1306-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1306-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1306-115">Not supported.</span></span>|
|<span data-ttu-id="c1306-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c1306-116">Application</span></span>|<span data-ttu-id="c1306-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1306-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1306-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c1306-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c1306-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c1306-119">Request headers</span></span>
|<span data-ttu-id="c1306-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c1306-120">Header</span></span>|<span data-ttu-id="c1306-121">値</span><span class="sxs-lookup"><span data-stu-id="c1306-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1306-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1306-122">Authorization</span></span>|<span data-ttu-id="c1306-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c1306-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1306-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c1306-124">Accept</span></span>|<span data-ttu-id="c1306-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1306-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1306-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c1306-126">Request body</span></span>
<span data-ttu-id="c1306-127">要求本文で、androidwork profilな maileasconfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c1306-127">In the request body, supply a JSON representation for the androidWorkProfileGmailEasConfiguration object.</span></span>

<span data-ttu-id="c1306-128">次の表に、androidwork profilare maileasconfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c1306-128">The following table shows the properties that are required when you create the androidWorkProfileGmailEasConfiguration.</span></span>

|<span data-ttu-id="c1306-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1306-129">Property</span></span>|<span data-ttu-id="c1306-130">型</span><span class="sxs-lookup"><span data-stu-id="c1306-130">Type</span></span>|<span data-ttu-id="c1306-131">説明</span><span class="sxs-lookup"><span data-stu-id="c1306-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1306-132">id</span><span class="sxs-lookup"><span data-stu-id="c1306-132">id</span></span>|<span data-ttu-id="c1306-133">文字列</span><span class="sxs-lookup"><span data-stu-id="c1306-133">String</span></span>|<span data-ttu-id="c1306-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c1306-134">Key of the entity.</span></span> <span data-ttu-id="c1306-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1306-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1306-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1306-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c1306-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1306-137">DateTimeOffset</span></span>|<span data-ttu-id="c1306-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c1306-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c1306-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1306-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1306-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c1306-140">roleScopeTagIds</span></span>|<span data-ttu-id="c1306-141">String collection</span><span class="sxs-lookup"><span data-stu-id="c1306-141">String collection</span></span>|<span data-ttu-id="c1306-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="c1306-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c1306-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1306-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1306-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c1306-144">supportsScopeTags</span></span>|<span data-ttu-id="c1306-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="c1306-145">Boolean</span></span>|<span data-ttu-id="c1306-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c1306-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c1306-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="c1306-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c1306-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="c1306-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c1306-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="c1306-149">This property is read-only.</span></span> <span data-ttu-id="c1306-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1306-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1306-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1306-151">createdDateTime</span></span>|<span data-ttu-id="c1306-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1306-152">DateTimeOffset</span></span>|<span data-ttu-id="c1306-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c1306-153">DateTime the object was created.</span></span> <span data-ttu-id="c1306-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1306-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1306-155">説明</span><span class="sxs-lookup"><span data-stu-id="c1306-155">description</span></span>|<span data-ttu-id="c1306-156">文字列</span><span class="sxs-lookup"><span data-stu-id="c1306-156">String</span></span>|<span data-ttu-id="c1306-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="c1306-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c1306-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1306-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1306-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c1306-159">displayName</span></span>|<span data-ttu-id="c1306-160">String</span><span class="sxs-lookup"><span data-stu-id="c1306-160">String</span></span>|<span data-ttu-id="c1306-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="c1306-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c1306-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1306-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1306-163">version</span><span class="sxs-lookup"><span data-stu-id="c1306-163">version</span></span>|<span data-ttu-id="c1306-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c1306-164">Int32</span></span>|<span data-ttu-id="c1306-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="c1306-165">Version of the device configuration.</span></span> <span data-ttu-id="c1306-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1306-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1306-167">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c1306-167">authenticationMethod</span></span>|[<span data-ttu-id="c1306-168">easauthenticationmethod</span><span class="sxs-lookup"><span data-stu-id="c1306-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="c1306-169">Exchange ActiveSync の認証方法。</span><span class="sxs-lookup"><span data-stu-id="c1306-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="c1306-170">[androidwork profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c1306-170">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="c1306-171">使用可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="c1306-171">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="c1306-172">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="c1306-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="c1306-173">emailsyncduration</span><span class="sxs-lookup"><span data-stu-id="c1306-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="c1306-174">電子メールを同期する時間の長さ。</span><span class="sxs-lookup"><span data-stu-id="c1306-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="c1306-175">[androidwork profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c1306-175">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="c1306-176">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="c1306-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="c1306-177">emailaddresssource</span><span class="sxs-lookup"><span data-stu-id="c1306-177">emailAddressSource</span></span>|[<span data-ttu-id="c1306-178">useremailsource</span><span class="sxs-lookup"><span data-stu-id="c1306-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="c1306-179">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="c1306-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c1306-180">[androidwork profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c1306-180">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="c1306-181">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="c1306-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="c1306-182">hostName</span><span class="sxs-lookup"><span data-stu-id="c1306-182">hostName</span></span>|<span data-ttu-id="c1306-183">String</span><span class="sxs-lookup"><span data-stu-id="c1306-183">String</span></span>|<span data-ttu-id="c1306-184">メールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="c1306-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="c1306-185">[androidwork profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="c1306-185">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="c1306-186">requireSsl</span><span class="sxs-lookup"><span data-stu-id="c1306-186">requireSsl</span></span>|<span data-ttu-id="c1306-187">ブール値</span><span class="sxs-lookup"><span data-stu-id="c1306-187">Boolean</span></span>|<span data-ttu-id="c1306-188">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c1306-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="c1306-189">[androidwork profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="c1306-189">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="c1306-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="c1306-190">usernameSource</span></span>|[<span data-ttu-id="c1306-191">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="c1306-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="c1306-192">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="c1306-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c1306-193">[androidwork profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c1306-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="c1306-194">可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="c1306-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="c1306-195">応答</span><span class="sxs-lookup"><span data-stu-id="c1306-195">Response</span></span>
<span data-ttu-id="c1306-196">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidwork profilな maileasconfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c1306-196">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1306-197">例</span><span class="sxs-lookup"><span data-stu-id="c1306-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1306-198">要求</span><span class="sxs-lookup"><span data-stu-id="c1306-198">Request</span></span>
<span data-ttu-id="c1306-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c1306-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 495

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName"
}
```

### <a name="response"></a><span data-ttu-id="c1306-200">応答</span><span class="sxs-lookup"><span data-stu-id="c1306-200">Response</span></span>
<span data-ttu-id="c1306-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c1306-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 667

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
  "id": "a4a44bb5-4bb5-a4a4-b54b-a4a4b54ba4a4",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName"
}
```




