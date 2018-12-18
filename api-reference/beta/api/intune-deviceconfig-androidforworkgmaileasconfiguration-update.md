---
title: AndroidForWorkGmailEasConfiguration を更新します。
description: AndroidForWorkGmailEasConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 9da99cb4ecb0d466a8367e2d7b5ad3902956e1c7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317795"
---
# <a name="update-androidforworkgmaileasconfiguration"></a><span data-ttu-id="fb306-103">AndroidForWorkGmailEasConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="fb306-103">Update androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="fb306-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fb306-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb306-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb306-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb306-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fb306-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb306-107">[AndroidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fb306-107">Update the properties of a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb306-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="fb306-108">Prerequisites</span></span>
<span data-ttu-id="fb306-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fb306-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb306-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fb306-111">Permission type</span></span>|<span data-ttu-id="fb306-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fb306-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb306-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fb306-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb306-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb306-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fb306-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fb306-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb306-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb306-116">Not supported.</span></span>|
|<span data-ttu-id="fb306-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fb306-117">Application</span></span>|<span data-ttu-id="fb306-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb306-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb306-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fb306-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fb306-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb306-120">Request headers</span></span>
|<span data-ttu-id="fb306-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb306-121">Header</span></span>|<span data-ttu-id="fb306-122">値</span><span class="sxs-lookup"><span data-stu-id="fb306-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb306-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb306-123">Authorization</span></span>|<span data-ttu-id="fb306-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fb306-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb306-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb306-125">Accept</span></span>|<span data-ttu-id="fb306-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb306-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb306-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fb306-127">Request body</span></span>
<span data-ttu-id="fb306-128">要求の本文に[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="fb306-128">In the request body, supply a JSON representation for the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="fb306-129">[AndroidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="fb306-129">The following table shows the properties that are required when you create the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md).</span></span>

|<span data-ttu-id="fb306-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb306-130">Property</span></span>|<span data-ttu-id="fb306-131">種類</span><span class="sxs-lookup"><span data-stu-id="fb306-131">Type</span></span>|<span data-ttu-id="fb306-132">説明</span><span class="sxs-lookup"><span data-stu-id="fb306-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb306-133">ID</span><span class="sxs-lookup"><span data-stu-id="fb306-133">id</span></span>|<span data-ttu-id="fb306-134">String</span><span class="sxs-lookup"><span data-stu-id="fb306-134">String</span></span>|<span data-ttu-id="fb306-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fb306-135">Key of the entity.</span></span> <span data-ttu-id="fb306-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fb306-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb306-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb306-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fb306-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb306-138">DateTimeOffset</span></span>|<span data-ttu-id="fb306-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="fb306-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fb306-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fb306-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb306-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fb306-141">roleScopeTagIds</span></span>|<span data-ttu-id="fb306-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fb306-142">String collection</span></span>|<span data-ttu-id="fb306-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="fb306-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fb306-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fb306-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb306-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fb306-145">supportsScopeTags</span></span>|<span data-ttu-id="fb306-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="fb306-146">Boolean</span></span>|<span data-ttu-id="fb306-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fb306-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fb306-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="fb306-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fb306-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="fb306-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fb306-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="fb306-150">This property is read-only.</span></span> <span data-ttu-id="fb306-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fb306-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb306-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb306-152">createdDateTime</span></span>|<span data-ttu-id="fb306-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb306-153">DateTimeOffset</span></span>|<span data-ttu-id="fb306-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="fb306-154">DateTime the object was created.</span></span> <span data-ttu-id="fb306-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fb306-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb306-156">説明</span><span class="sxs-lookup"><span data-stu-id="fb306-156">description</span></span>|<span data-ttu-id="fb306-157">String</span><span class="sxs-lookup"><span data-stu-id="fb306-157">String</span></span>|<span data-ttu-id="fb306-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="fb306-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fb306-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fb306-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb306-160">displayName</span><span class="sxs-lookup"><span data-stu-id="fb306-160">displayName</span></span>|<span data-ttu-id="fb306-161">String</span><span class="sxs-lookup"><span data-stu-id="fb306-161">String</span></span>|<span data-ttu-id="fb306-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="fb306-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fb306-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fb306-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb306-164">version</span><span class="sxs-lookup"><span data-stu-id="fb306-164">version</span></span>|<span data-ttu-id="fb306-165">Int32</span><span class="sxs-lookup"><span data-stu-id="fb306-165">Int32</span></span>|<span data-ttu-id="fb306-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="fb306-166">Version of the device configuration.</span></span> <span data-ttu-id="fb306-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fb306-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb306-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fb306-168">authenticationMethod</span></span>|[<span data-ttu-id="fb306-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fb306-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="fb306-170">Exchange ActiveSync の認証方法です。</span><span class="sxs-lookup"><span data-stu-id="fb306-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="fb306-171">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="fb306-171">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="fb306-172">使用可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="fb306-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="fb306-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="fb306-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="fb306-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="fb306-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="fb306-175">電子メールの時間の期間に同期する必要があります。</span><span class="sxs-lookup"><span data-stu-id="fb306-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="fb306-176">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="fb306-176">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="fb306-177">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="fb306-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="fb306-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="fb306-178">emailAddressSource</span></span>|[<span data-ttu-id="fb306-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="fb306-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="fb306-180">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたメール属性です。</span><span class="sxs-lookup"><span data-stu-id="fb306-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="fb306-181">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="fb306-181">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="fb306-182">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="fb306-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="fb306-183">hostName</span><span class="sxs-lookup"><span data-stu-id="fb306-183">hostName</span></span>|<span data-ttu-id="fb306-184">String</span><span class="sxs-lookup"><span data-stu-id="fb306-184">String</span></span>|<span data-ttu-id="fb306-185">Exchange の場所 (URL)、メール ・ アプリケーションに接続します。</span><span class="sxs-lookup"><span data-stu-id="fb306-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="fb306-186">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="fb306-186">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="fb306-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="fb306-187">requireSsl</span></span>|<span data-ttu-id="fb306-188">ブール型</span><span class="sxs-lookup"><span data-stu-id="fb306-188">Boolean</span></span>|<span data-ttu-id="fb306-189">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fb306-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="fb306-190">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="fb306-190">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="fb306-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="fb306-191">usernameSource</span></span>|[<span data-ttu-id="fb306-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="fb306-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="fb306-193">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー名の属性です。</span><span class="sxs-lookup"><span data-stu-id="fb306-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="fb306-194">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="fb306-194">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="fb306-195">可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="fb306-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="fb306-196">応答</span><span class="sxs-lookup"><span data-stu-id="fb306-196">Response</span></span>
<span data-ttu-id="fb306-197">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="fb306-197">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb306-198">例</span><span class="sxs-lookup"><span data-stu-id="fb306-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb306-199">要求</span><span class="sxs-lookup"><span data-stu-id="fb306-199">Request</span></span>
<span data-ttu-id="fb306-200">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fb306-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 481

{
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

### <a name="response"></a><span data-ttu-id="fb306-201">応答</span><span class="sxs-lookup"><span data-stu-id="fb306-201">Response</span></span>
<span data-ttu-id="fb306-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fb306-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





