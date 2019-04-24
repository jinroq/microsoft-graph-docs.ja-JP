---
title: androidforwork gmaileasconfiguration の作成
description: 新しい androidforwork gmaileasconfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 10a53f08d3f0af5bb54d84655e6d735d3d2cd5d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32479002"
---
# <a name="create-androidforworkgmaileasconfiguration"></a><span data-ttu-id="c9ea1-103">androidforwork gmaileasconfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="c9ea1-103">Create androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="c9ea1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9ea1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9ea1-106">新しい[androidforwork gmaileasconfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-106">Create a new [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9ea1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c9ea1-107">Prerequisites</span></span>
<span data-ttu-id="c9ea1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9ea1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c9ea1-110">Permission type</span></span>|<span data-ttu-id="c9ea1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c9ea1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9ea1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c9ea1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c9ea1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9ea1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9ea1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c9ea1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9ea1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-115">Not supported.</span></span>|
|<span data-ttu-id="c9ea1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c9ea1-116">Application</span></span>|<span data-ttu-id="c9ea1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9ea1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c9ea1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c9ea1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9ea1-119">Request headers</span></span>
|<span data-ttu-id="c9ea1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9ea1-120">Header</span></span>|<span data-ttu-id="c9ea1-121">値</span><span class="sxs-lookup"><span data-stu-id="c9ea1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9ea1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9ea1-122">Authorization</span></span>|<span data-ttu-id="c9ea1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9ea1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c9ea1-124">Accept</span></span>|<span data-ttu-id="c9ea1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c9ea1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9ea1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c9ea1-126">Request body</span></span>
<span data-ttu-id="c9ea1-127">要求本文で、androidforwork gmaileasconfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-127">In the request body, supply a JSON representation for the androidForWorkGmailEasConfiguration object.</span></span>

<span data-ttu-id="c9ea1-128">次の表に、androidforwork gmaileasconfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-128">The following table shows the properties that are required when you create the androidForWorkGmailEasConfiguration.</span></span>

|<span data-ttu-id="c9ea1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9ea1-129">Property</span></span>|<span data-ttu-id="c9ea1-130">型</span><span class="sxs-lookup"><span data-stu-id="c9ea1-130">Type</span></span>|<span data-ttu-id="c9ea1-131">説明</span><span class="sxs-lookup"><span data-stu-id="c9ea1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9ea1-132">id</span><span class="sxs-lookup"><span data-stu-id="c9ea1-132">id</span></span>|<span data-ttu-id="c9ea1-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c9ea1-133">String</span></span>|<span data-ttu-id="c9ea1-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-134">Key of the entity.</span></span> <span data-ttu-id="c9ea1-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c9ea1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9ea1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9ea1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c9ea1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9ea1-137">DateTimeOffset</span></span>|<span data-ttu-id="c9ea1-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c9ea1-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c9ea1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9ea1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c9ea1-140">roleScopeTagIds</span></span>|<span data-ttu-id="c9ea1-141">String collection</span><span class="sxs-lookup"><span data-stu-id="c9ea1-141">String collection</span></span>|<span data-ttu-id="c9ea1-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c9ea1-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c9ea1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9ea1-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c9ea1-144">supportsScopeTags</span></span>|<span data-ttu-id="c9ea1-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9ea1-145">Boolean</span></span>|<span data-ttu-id="c9ea1-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c9ea1-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c9ea1-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c9ea1-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-149">This property is read-only.</span></span> <span data-ttu-id="c9ea1-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c9ea1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9ea1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9ea1-151">createdDateTime</span></span>|<span data-ttu-id="c9ea1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9ea1-152">DateTimeOffset</span></span>|<span data-ttu-id="c9ea1-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-153">DateTime the object was created.</span></span> <span data-ttu-id="c9ea1-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c9ea1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9ea1-155">説明</span><span class="sxs-lookup"><span data-stu-id="c9ea1-155">description</span></span>|<span data-ttu-id="c9ea1-156">String</span><span class="sxs-lookup"><span data-stu-id="c9ea1-156">String</span></span>|<span data-ttu-id="c9ea1-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c9ea1-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c9ea1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9ea1-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c9ea1-159">displayName</span></span>|<span data-ttu-id="c9ea1-160">String</span><span class="sxs-lookup"><span data-stu-id="c9ea1-160">String</span></span>|<span data-ttu-id="c9ea1-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c9ea1-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c9ea1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9ea1-163">version</span><span class="sxs-lookup"><span data-stu-id="c9ea1-163">version</span></span>|<span data-ttu-id="c9ea1-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c9ea1-164">Int32</span></span>|<span data-ttu-id="c9ea1-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-165">Version of the device configuration.</span></span> <span data-ttu-id="c9ea1-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c9ea1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9ea1-167">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c9ea1-167">authenticationMethod</span></span>|[<span data-ttu-id="c9ea1-168">easauthenticationmethod</span><span class="sxs-lookup"><span data-stu-id="c9ea1-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="c9ea1-169">Exchange ActiveSync の認証方法。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="c9ea1-170">[androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-170">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="c9ea1-171">可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-171">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="c9ea1-172">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="c9ea1-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="c9ea1-173">emailsyncduration</span><span class="sxs-lookup"><span data-stu-id="c9ea1-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="c9ea1-174">電子メールを同期する時間の長さ。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="c9ea1-175">[androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-175">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="c9ea1-176">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="c9ea1-177">emailaddresssource</span><span class="sxs-lookup"><span data-stu-id="c9ea1-177">emailAddressSource</span></span>|[<span data-ttu-id="c9ea1-178">useremailsource</span><span class="sxs-lookup"><span data-stu-id="c9ea1-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="c9ea1-179">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c9ea1-180">[androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-180">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="c9ea1-181">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="c9ea1-182">hostName</span><span class="sxs-lookup"><span data-stu-id="c9ea1-182">hostName</span></span>|<span data-ttu-id="c9ea1-183">String</span><span class="sxs-lookup"><span data-stu-id="c9ea1-183">String</span></span>|<span data-ttu-id="c9ea1-184">メールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="c9ea1-185">[androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="c9ea1-185">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="c9ea1-186">requireSsl</span><span class="sxs-lookup"><span data-stu-id="c9ea1-186">requireSsl</span></span>|<span data-ttu-id="c9ea1-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9ea1-187">Boolean</span></span>|<span data-ttu-id="c9ea1-188">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="c9ea1-189">[androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="c9ea1-189">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="c9ea1-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="c9ea1-190">usernameSource</span></span>|[<span data-ttu-id="c9ea1-191">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="c9ea1-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="c9ea1-192">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c9ea1-193">[androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-193">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="c9ea1-194">可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="c9ea1-195">応答</span><span class="sxs-lookup"><span data-stu-id="c9ea1-195">Response</span></span>
<span data-ttu-id="c9ea1-196">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidforwork gmaileasconfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-196">If successful, this method returns a `201 Created` response code and a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9ea1-197">例</span><span class="sxs-lookup"><span data-stu-id="c9ea1-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9ea1-198">要求</span><span class="sxs-lookup"><span data-stu-id="c9ea1-198">Request</span></span>
<span data-ttu-id="c9ea1-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 491

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="c9ea1-200">応答</span><span class="sxs-lookup"><span data-stu-id="c9ea1-200">Response</span></span>
<span data-ttu-id="c9ea1-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c9ea1-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 663

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
  "id": "2bafc891-c891-2baf-91c8-af2b91c8af2b",
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





