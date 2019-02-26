---
title: androidforwork gmaileasconfiguration の更新
description: androidforwork gmaileasconfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0282a819f6c5e4883c36433e8066159e1be70364
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142722"
---
# <a name="update-androidforworkgmaileasconfiguration"></a><span data-ttu-id="bb6a8-103">androidforwork gmaileasconfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="bb6a8-103">Update androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="bb6a8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb6a8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb6a8-106">[androidforwork gmaileasconfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-106">Update the properties of a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb6a8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="bb6a8-107">Prerequisites</span></span>
<span data-ttu-id="bb6a8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bb6a8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bb6a8-110">Permission type</span></span>|<span data-ttu-id="bb6a8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bb6a8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb6a8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bb6a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb6a8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb6a8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb6a8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bb6a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb6a8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-115">Not supported.</span></span>|
|<span data-ttu-id="bb6a8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bb6a8-116">Application</span></span>|<span data-ttu-id="bb6a8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb6a8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bb6a8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bb6a8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb6a8-119">Request headers</span></span>
|<span data-ttu-id="bb6a8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb6a8-120">Header</span></span>|<span data-ttu-id="bb6a8-121">値</span><span class="sxs-lookup"><span data-stu-id="bb6a8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb6a8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb6a8-122">Authorization</span></span>|<span data-ttu-id="bb6a8-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb6a8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="bb6a8-124">Accept</span></span>|<span data-ttu-id="bb6a8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bb6a8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb6a8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bb6a8-126">Request body</span></span>
<span data-ttu-id="bb6a8-127">要求本文で、 [androidforwork gmaileasconfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-127">In the request body, supply a JSON representation for the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="bb6a8-128">次の表に、 [androidforwork gmaileasconfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-128">The following table shows the properties that are required when you create the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md).</span></span>

|<span data-ttu-id="bb6a8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb6a8-129">Property</span></span>|<span data-ttu-id="bb6a8-130">型</span><span class="sxs-lookup"><span data-stu-id="bb6a8-130">Type</span></span>|<span data-ttu-id="bb6a8-131">説明</span><span class="sxs-lookup"><span data-stu-id="bb6a8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb6a8-132">id</span><span class="sxs-lookup"><span data-stu-id="bb6a8-132">id</span></span>|<span data-ttu-id="bb6a8-133">文字列</span><span class="sxs-lookup"><span data-stu-id="bb6a8-133">String</span></span>|<span data-ttu-id="bb6a8-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-134">Key of the entity.</span></span> <span data-ttu-id="bb6a8-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bb6a8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb6a8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb6a8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bb6a8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb6a8-137">DateTimeOffset</span></span>|<span data-ttu-id="bb6a8-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="bb6a8-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bb6a8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb6a8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bb6a8-140">roleScopeTagIds</span></span>|<span data-ttu-id="bb6a8-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="bb6a8-141">String collection</span></span>|<span data-ttu-id="bb6a8-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bb6a8-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bb6a8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb6a8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bb6a8-144">supportsScopeTags</span></span>|<span data-ttu-id="bb6a8-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb6a8-145">Boolean</span></span>|<span data-ttu-id="bb6a8-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bb6a8-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bb6a8-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bb6a8-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-149">This property is read-only.</span></span> <span data-ttu-id="bb6a8-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bb6a8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb6a8-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb6a8-151">createdDateTime</span></span>|<span data-ttu-id="bb6a8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb6a8-152">DateTimeOffset</span></span>|<span data-ttu-id="bb6a8-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-153">DateTime the object was created.</span></span> <span data-ttu-id="bb6a8-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bb6a8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb6a8-155">説明</span><span class="sxs-lookup"><span data-stu-id="bb6a8-155">description</span></span>|<span data-ttu-id="bb6a8-156">文字列</span><span class="sxs-lookup"><span data-stu-id="bb6a8-156">String</span></span>|<span data-ttu-id="bb6a8-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bb6a8-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bb6a8-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb6a8-159">displayName</span><span class="sxs-lookup"><span data-stu-id="bb6a8-159">displayName</span></span>|<span data-ttu-id="bb6a8-160">String</span><span class="sxs-lookup"><span data-stu-id="bb6a8-160">String</span></span>|<span data-ttu-id="bb6a8-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bb6a8-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bb6a8-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb6a8-163">version</span><span class="sxs-lookup"><span data-stu-id="bb6a8-163">version</span></span>|<span data-ttu-id="bb6a8-164">Int32</span><span class="sxs-lookup"><span data-stu-id="bb6a8-164">Int32</span></span>|<span data-ttu-id="bb6a8-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-165">Version of the device configuration.</span></span> <span data-ttu-id="bb6a8-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bb6a8-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb6a8-167">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="bb6a8-167">authenticationMethod</span></span>|[<span data-ttu-id="bb6a8-168">easauthenticationmethod</span><span class="sxs-lookup"><span data-stu-id="bb6a8-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="bb6a8-169">Exchange ActiveSync の認証方法。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="bb6a8-170">[androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-170">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="bb6a8-171">使用可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-171">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="bb6a8-172">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="bb6a8-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="bb6a8-173">emailsyncduration</span><span class="sxs-lookup"><span data-stu-id="bb6a8-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="bb6a8-174">電子メールを同期する時間の長さ。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="bb6a8-175">[androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-175">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="bb6a8-176">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="bb6a8-177">emailaddresssource</span><span class="sxs-lookup"><span data-stu-id="bb6a8-177">emailAddressSource</span></span>|[<span data-ttu-id="bb6a8-178">useremailsource</span><span class="sxs-lookup"><span data-stu-id="bb6a8-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="bb6a8-179">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="bb6a8-180">[androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-180">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="bb6a8-181">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="bb6a8-182">hostName</span><span class="sxs-lookup"><span data-stu-id="bb6a8-182">hostName</span></span>|<span data-ttu-id="bb6a8-183">String</span><span class="sxs-lookup"><span data-stu-id="bb6a8-183">String</span></span>|<span data-ttu-id="bb6a8-184">メールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="bb6a8-185">[androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="bb6a8-185">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="bb6a8-186">requireSsl</span><span class="sxs-lookup"><span data-stu-id="bb6a8-186">requireSsl</span></span>|<span data-ttu-id="bb6a8-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb6a8-187">Boolean</span></span>|<span data-ttu-id="bb6a8-188">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="bb6a8-189">[androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="bb6a8-189">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="bb6a8-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="bb6a8-190">usernameSource</span></span>|[<span data-ttu-id="bb6a8-191">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="bb6a8-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="bb6a8-192">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="bb6a8-193">[androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-193">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="bb6a8-194">可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="bb6a8-195">応答</span><span class="sxs-lookup"><span data-stu-id="bb6a8-195">Response</span></span>
<span data-ttu-id="bb6a8-196">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidforwork gmaileasconfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-196">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb6a8-197">例</span><span class="sxs-lookup"><span data-stu-id="bb6a8-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb6a8-198">要求</span><span class="sxs-lookup"><span data-stu-id="bb6a8-198">Request</span></span>
<span data-ttu-id="bb6a8-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="bb6a8-200">応答</span><span class="sxs-lookup"><span data-stu-id="bb6a8-200">Response</span></span>
<span data-ttu-id="bb6a8-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bb6a8-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




