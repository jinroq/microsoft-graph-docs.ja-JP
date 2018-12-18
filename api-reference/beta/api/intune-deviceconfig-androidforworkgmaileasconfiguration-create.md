---
title: AndroidForWorkGmailEasConfiguration を作成します。
description: 新しい androidForWorkGmailEasConfiguration オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 7da73972b4738c23f9f5cff5c7d80ea29d7561d3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355532"
---
# <a name="create-androidforworkgmaileasconfiguration"></a><span data-ttu-id="87e52-103">AndroidForWorkGmailEasConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="87e52-103">Create androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="87e52-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="87e52-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87e52-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87e52-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87e52-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="87e52-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87e52-107">新しい[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="87e52-107">Create a new [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87e52-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="87e52-108">Prerequisites</span></span>
<span data-ttu-id="87e52-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87e52-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87e52-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="87e52-111">Permission type</span></span>|<span data-ttu-id="87e52-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="87e52-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87e52-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="87e52-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87e52-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87e52-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="87e52-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="87e52-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87e52-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87e52-116">Not supported.</span></span>|
|<span data-ttu-id="87e52-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="87e52-117">Application</span></span>|<span data-ttu-id="87e52-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87e52-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87e52-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="87e52-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="87e52-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87e52-120">Request headers</span></span>
|<span data-ttu-id="87e52-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87e52-121">Header</span></span>|<span data-ttu-id="87e52-122">値</span><span class="sxs-lookup"><span data-stu-id="87e52-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87e52-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="87e52-123">Authorization</span></span>|<span data-ttu-id="87e52-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="87e52-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87e52-125">Accept</span><span class="sxs-lookup"><span data-stu-id="87e52-125">Accept</span></span>|<span data-ttu-id="87e52-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87e52-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87e52-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="87e52-127">Request body</span></span>
<span data-ttu-id="87e52-128">要求の本文に androidForWorkGmailEasConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="87e52-128">In the request body, supply a JSON representation for the androidForWorkGmailEasConfiguration object.</span></span>

<span data-ttu-id="87e52-129">次の表は、androidForWorkGmailEasConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="87e52-129">The following table shows the properties that are required when you create the androidForWorkGmailEasConfiguration.</span></span>

|<span data-ttu-id="87e52-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="87e52-130">Property</span></span>|<span data-ttu-id="87e52-131">種類</span><span class="sxs-lookup"><span data-stu-id="87e52-131">Type</span></span>|<span data-ttu-id="87e52-132">説明</span><span class="sxs-lookup"><span data-stu-id="87e52-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87e52-133">ID</span><span class="sxs-lookup"><span data-stu-id="87e52-133">id</span></span>|<span data-ttu-id="87e52-134">String</span><span class="sxs-lookup"><span data-stu-id="87e52-134">String</span></span>|<span data-ttu-id="87e52-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="87e52-135">Key of the entity.</span></span> <span data-ttu-id="87e52-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="87e52-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87e52-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87e52-137">lastModifiedDateTime</span></span>|<span data-ttu-id="87e52-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87e52-138">DateTimeOffset</span></span>|<span data-ttu-id="87e52-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="87e52-139">DateTime the object was last modified.</span></span> <span data-ttu-id="87e52-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="87e52-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87e52-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="87e52-141">roleScopeTagIds</span></span>|<span data-ttu-id="87e52-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="87e52-142">String collection</span></span>|<span data-ttu-id="87e52-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="87e52-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="87e52-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="87e52-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87e52-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="87e52-145">supportsScopeTags</span></span>|<span data-ttu-id="87e52-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="87e52-146">Boolean</span></span>|<span data-ttu-id="87e52-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="87e52-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="87e52-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="87e52-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="87e52-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="87e52-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="87e52-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="87e52-150">This property is read-only.</span></span> <span data-ttu-id="87e52-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="87e52-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87e52-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87e52-152">createdDateTime</span></span>|<span data-ttu-id="87e52-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87e52-153">DateTimeOffset</span></span>|<span data-ttu-id="87e52-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="87e52-154">DateTime the object was created.</span></span> <span data-ttu-id="87e52-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="87e52-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87e52-156">説明</span><span class="sxs-lookup"><span data-stu-id="87e52-156">description</span></span>|<span data-ttu-id="87e52-157">String</span><span class="sxs-lookup"><span data-stu-id="87e52-157">String</span></span>|<span data-ttu-id="87e52-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="87e52-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="87e52-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="87e52-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87e52-160">displayName</span><span class="sxs-lookup"><span data-stu-id="87e52-160">displayName</span></span>|<span data-ttu-id="87e52-161">String</span><span class="sxs-lookup"><span data-stu-id="87e52-161">String</span></span>|<span data-ttu-id="87e52-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="87e52-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="87e52-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="87e52-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87e52-164">version</span><span class="sxs-lookup"><span data-stu-id="87e52-164">version</span></span>|<span data-ttu-id="87e52-165">Int32</span><span class="sxs-lookup"><span data-stu-id="87e52-165">Int32</span></span>|<span data-ttu-id="87e52-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="87e52-166">Version of the device configuration.</span></span> <span data-ttu-id="87e52-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="87e52-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87e52-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="87e52-168">authenticationMethod</span></span>|[<span data-ttu-id="87e52-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="87e52-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="87e52-170">Exchange ActiveSync の認証方法です。</span><span class="sxs-lookup"><span data-stu-id="87e52-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="87e52-171">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="87e52-171">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="87e52-172">使用可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="87e52-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="87e52-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="87e52-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="87e52-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="87e52-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="87e52-175">電子メールの時間の期間に同期する必要があります。</span><span class="sxs-lookup"><span data-stu-id="87e52-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="87e52-176">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="87e52-176">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="87e52-177">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="87e52-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="87e52-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="87e52-178">emailAddressSource</span></span>|[<span data-ttu-id="87e52-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="87e52-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="87e52-180">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたメール属性です。</span><span class="sxs-lookup"><span data-stu-id="87e52-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="87e52-181">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="87e52-181">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="87e52-182">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="87e52-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="87e52-183">hostName</span><span class="sxs-lookup"><span data-stu-id="87e52-183">hostName</span></span>|<span data-ttu-id="87e52-184">String</span><span class="sxs-lookup"><span data-stu-id="87e52-184">String</span></span>|<span data-ttu-id="87e52-185">Exchange の場所 (URL)、メール ・ アプリケーションに接続します。</span><span class="sxs-lookup"><span data-stu-id="87e52-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="87e52-186">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="87e52-186">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="87e52-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="87e52-187">requireSsl</span></span>|<span data-ttu-id="87e52-188">ブール型</span><span class="sxs-lookup"><span data-stu-id="87e52-188">Boolean</span></span>|<span data-ttu-id="87e52-189">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="87e52-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="87e52-190">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="87e52-190">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="87e52-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="87e52-191">usernameSource</span></span>|[<span data-ttu-id="87e52-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="87e52-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="87e52-193">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー名の属性です。</span><span class="sxs-lookup"><span data-stu-id="87e52-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="87e52-194">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="87e52-194">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="87e52-195">可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="87e52-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="87e52-196">応答</span><span class="sxs-lookup"><span data-stu-id="87e52-196">Response</span></span>
<span data-ttu-id="87e52-197">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="87e52-197">If successful, this method returns a `201 Created` response code and a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87e52-198">例</span><span class="sxs-lookup"><span data-stu-id="87e52-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="87e52-199">要求</span><span class="sxs-lookup"><span data-stu-id="87e52-199">Request</span></span>
<span data-ttu-id="87e52-200">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="87e52-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 555

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="87e52-201">応答</span><span class="sxs-lookup"><span data-stu-id="87e52-201">Response</span></span>
<span data-ttu-id="87e52-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="87e52-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





