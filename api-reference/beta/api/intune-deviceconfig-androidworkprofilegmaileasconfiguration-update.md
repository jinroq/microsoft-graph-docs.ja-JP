---
title: AndroidWorkProfileGmailEasConfiguration を更新します。
description: AndroidWorkProfileGmailEasConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: a3de985759cb4f9630593e5d86082421a5f3b937
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324186"
---
# <a name="update-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="92511-103">AndroidWorkProfileGmailEasConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="92511-103">Update androidWorkProfileGmailEasConfiguration</span></span>

> <span data-ttu-id="92511-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="92511-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92511-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92511-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="92511-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="92511-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92511-107">[AndroidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="92511-107">Update the properties of a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="92511-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="92511-108">Prerequisites</span></span>
<span data-ttu-id="92511-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92511-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92511-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="92511-111">Permission type</span></span>|<span data-ttu-id="92511-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="92511-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92511-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="92511-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92511-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92511-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92511-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="92511-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92511-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92511-116">Not supported.</span></span>|
|<span data-ttu-id="92511-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="92511-117">Application</span></span>|<span data-ttu-id="92511-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92511-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92511-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="92511-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="92511-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92511-120">Request headers</span></span>
|<span data-ttu-id="92511-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92511-121">Header</span></span>|<span data-ttu-id="92511-122">値</span><span class="sxs-lookup"><span data-stu-id="92511-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92511-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="92511-123">Authorization</span></span>|<span data-ttu-id="92511-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="92511-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92511-125">Accept</span><span class="sxs-lookup"><span data-stu-id="92511-125">Accept</span></span>|<span data-ttu-id="92511-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92511-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92511-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="92511-127">Request body</span></span>
<span data-ttu-id="92511-128">要求の本文に[androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="92511-128">In the request body, supply a JSON representation for the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="92511-129">[AndroidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="92511-129">The following table shows the properties that are required when you create the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md).</span></span>

|<span data-ttu-id="92511-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92511-130">Property</span></span>|<span data-ttu-id="92511-131">種類</span><span class="sxs-lookup"><span data-stu-id="92511-131">Type</span></span>|<span data-ttu-id="92511-132">説明</span><span class="sxs-lookup"><span data-stu-id="92511-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92511-133">ID</span><span class="sxs-lookup"><span data-stu-id="92511-133">id</span></span>|<span data-ttu-id="92511-134">String</span><span class="sxs-lookup"><span data-stu-id="92511-134">String</span></span>|<span data-ttu-id="92511-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="92511-135">Key of the entity.</span></span> <span data-ttu-id="92511-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92511-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92511-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92511-137">lastModifiedDateTime</span></span>|<span data-ttu-id="92511-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92511-138">DateTimeOffset</span></span>|<span data-ttu-id="92511-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="92511-139">DateTime the object was last modified.</span></span> <span data-ttu-id="92511-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92511-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92511-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="92511-141">roleScopeTagIds</span></span>|<span data-ttu-id="92511-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="92511-142">String collection</span></span>|<span data-ttu-id="92511-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="92511-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="92511-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92511-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92511-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="92511-145">supportsScopeTags</span></span>|<span data-ttu-id="92511-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="92511-146">Boolean</span></span>|<span data-ttu-id="92511-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="92511-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="92511-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="92511-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="92511-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="92511-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="92511-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="92511-150">This property is read-only.</span></span> <span data-ttu-id="92511-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92511-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92511-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92511-152">createdDateTime</span></span>|<span data-ttu-id="92511-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92511-153">DateTimeOffset</span></span>|<span data-ttu-id="92511-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="92511-154">DateTime the object was created.</span></span> <span data-ttu-id="92511-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92511-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92511-156">説明</span><span class="sxs-lookup"><span data-stu-id="92511-156">description</span></span>|<span data-ttu-id="92511-157">String</span><span class="sxs-lookup"><span data-stu-id="92511-157">String</span></span>|<span data-ttu-id="92511-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="92511-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="92511-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92511-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92511-160">displayName</span><span class="sxs-lookup"><span data-stu-id="92511-160">displayName</span></span>|<span data-ttu-id="92511-161">String</span><span class="sxs-lookup"><span data-stu-id="92511-161">String</span></span>|<span data-ttu-id="92511-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="92511-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="92511-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92511-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92511-164">version</span><span class="sxs-lookup"><span data-stu-id="92511-164">version</span></span>|<span data-ttu-id="92511-165">Int32</span><span class="sxs-lookup"><span data-stu-id="92511-165">Int32</span></span>|<span data-ttu-id="92511-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="92511-166">Version of the device configuration.</span></span> <span data-ttu-id="92511-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92511-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92511-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="92511-168">authenticationMethod</span></span>|[<span data-ttu-id="92511-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="92511-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="92511-170">Exchange ActiveSync の認証方法です。</span><span class="sxs-lookup"><span data-stu-id="92511-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="92511-171">[AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="92511-171">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="92511-172">使用可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="92511-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="92511-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="92511-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="92511-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="92511-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="92511-175">電子メールの時間の期間に同期する必要があります。</span><span class="sxs-lookup"><span data-stu-id="92511-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="92511-176">[AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="92511-176">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="92511-177">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="92511-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="92511-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="92511-178">emailAddressSource</span></span>|[<span data-ttu-id="92511-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="92511-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="92511-180">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたメール属性です。</span><span class="sxs-lookup"><span data-stu-id="92511-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="92511-181">[AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="92511-181">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="92511-182">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="92511-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="92511-183">hostName</span><span class="sxs-lookup"><span data-stu-id="92511-183">hostName</span></span>|<span data-ttu-id="92511-184">String</span><span class="sxs-lookup"><span data-stu-id="92511-184">String</span></span>|<span data-ttu-id="92511-185">Exchange の場所 (URL)、メール ・ アプリケーションに接続します。</span><span class="sxs-lookup"><span data-stu-id="92511-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="92511-186">[AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="92511-186">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="92511-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="92511-187">requireSsl</span></span>|<span data-ttu-id="92511-188">ブール型</span><span class="sxs-lookup"><span data-stu-id="92511-188">Boolean</span></span>|<span data-ttu-id="92511-189">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="92511-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="92511-190">[AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="92511-190">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="92511-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="92511-191">usernameSource</span></span>|[<span data-ttu-id="92511-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="92511-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="92511-193">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー名の属性です。</span><span class="sxs-lookup"><span data-stu-id="92511-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="92511-194">[AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="92511-194">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="92511-195">可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="92511-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="92511-196">応答</span><span class="sxs-lookup"><span data-stu-id="92511-196">Response</span></span>
<span data-ttu-id="92511-197">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="92511-197">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92511-198">例</span><span class="sxs-lookup"><span data-stu-id="92511-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="92511-199">要求</span><span class="sxs-lookup"><span data-stu-id="92511-199">Request</span></span>
<span data-ttu-id="92511-200">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="92511-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="92511-201">応答</span><span class="sxs-lookup"><span data-stu-id="92511-201">Response</span></span>
<span data-ttu-id="92511-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="92511-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




