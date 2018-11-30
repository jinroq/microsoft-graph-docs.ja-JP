---
title: AndroidForWorkGmailEasConfiguration を更新します。
description: AndroidForWorkGmailEasConfiguration オブジェクトのプロパティを更新します。
ms.openlocfilehash: 2652a5a40bb82f411d4fd0b5169e17a5eaf3863d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071468"
---
# <a name="update-androidforworkgmaileasconfiguration"></a><span data-ttu-id="4f364-103">AndroidForWorkGmailEasConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="4f364-103">Update androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="4f364-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4f364-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f364-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f364-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4f364-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4f364-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f364-107">[AndroidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4f364-107">Update the properties of a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4f364-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4f364-108">Prerequisites</span></span>
<span data-ttu-id="4f364-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f364-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f364-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4f364-111">Permission type</span></span>|<span data-ttu-id="4f364-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4f364-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f364-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4f364-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f364-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f364-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f364-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4f364-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f364-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f364-116">Not supported.</span></span>|
|<span data-ttu-id="4f364-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4f364-117">Application</span></span>|<span data-ttu-id="4f364-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f364-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f364-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4f364-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4f364-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4f364-120">Request headers</span></span>
|<span data-ttu-id="4f364-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4f364-121">Header</span></span>|<span data-ttu-id="4f364-122">値</span><span class="sxs-lookup"><span data-stu-id="4f364-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f364-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f364-123">Authorization</span></span>|<span data-ttu-id="4f364-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4f364-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f364-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4f364-125">Accept</span></span>|<span data-ttu-id="4f364-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f364-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f364-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4f364-127">Request body</span></span>
<span data-ttu-id="4f364-128">要求の本文に[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="4f364-128">In the request body, supply a JSON representation for the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="4f364-129">[AndroidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="4f364-129">The following table shows the properties that are required when you create the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md).</span></span>

|<span data-ttu-id="4f364-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f364-130">Property</span></span>|<span data-ttu-id="4f364-131">型</span><span class="sxs-lookup"><span data-stu-id="4f364-131">Type</span></span>|<span data-ttu-id="4f364-132">説明</span><span class="sxs-lookup"><span data-stu-id="4f364-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f364-133">id</span><span class="sxs-lookup"><span data-stu-id="4f364-133">id</span></span>|<span data-ttu-id="4f364-134">String</span><span class="sxs-lookup"><span data-stu-id="4f364-134">String</span></span>|<span data-ttu-id="4f364-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4f364-135">Key of the entity.</span></span> <span data-ttu-id="4f364-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4f364-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f364-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f364-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4f364-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f364-138">DateTimeOffset</span></span>|<span data-ttu-id="4f364-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4f364-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4f364-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4f364-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f364-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4f364-141">roleScopeTagIds</span></span>|<span data-ttu-id="4f364-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4f364-142">String collection</span></span>|<span data-ttu-id="4f364-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="4f364-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4f364-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4f364-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f364-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4f364-145">supportsScopeTags</span></span>|<span data-ttu-id="4f364-146">ブール値</span><span class="sxs-lookup"><span data-stu-id="4f364-146">Boolean</span></span>|<span data-ttu-id="4f364-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4f364-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4f364-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="4f364-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4f364-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="4f364-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4f364-150">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="4f364-150">This property is read-only.</span></span> <span data-ttu-id="4f364-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4f364-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f364-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f364-152">createdDateTime</span></span>|<span data-ttu-id="4f364-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f364-153">DateTimeOffset</span></span>|<span data-ttu-id="4f364-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4f364-154">DateTime the object was created.</span></span> <span data-ttu-id="4f364-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4f364-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f364-156">説明</span><span class="sxs-lookup"><span data-stu-id="4f364-156">description</span></span>|<span data-ttu-id="4f364-157">String</span><span class="sxs-lookup"><span data-stu-id="4f364-157">String</span></span>|<span data-ttu-id="4f364-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="4f364-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4f364-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4f364-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f364-160">displayName</span><span class="sxs-lookup"><span data-stu-id="4f364-160">displayName</span></span>|<span data-ttu-id="4f364-161">String</span><span class="sxs-lookup"><span data-stu-id="4f364-161">String</span></span>|<span data-ttu-id="4f364-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="4f364-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4f364-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4f364-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f364-164">version</span><span class="sxs-lookup"><span data-stu-id="4f364-164">version</span></span>|<span data-ttu-id="4f364-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4f364-165">Int32</span></span>|<span data-ttu-id="4f364-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="4f364-166">Version of the device configuration.</span></span> <span data-ttu-id="4f364-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4f364-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f364-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4f364-168">authenticationMethod</span></span>|[<span data-ttu-id="4f364-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4f364-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="4f364-170">Exchange ActiveSync の認証方法です。</span><span class="sxs-lookup"><span data-stu-id="4f364-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="4f364-171">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4f364-171">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="4f364-172">使用可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="4f364-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="4f364-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="4f364-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="4f364-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="4f364-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="4f364-175">電子メールの時間の期間に同期する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4f364-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="4f364-176">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4f364-176">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="4f364-177">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="4f364-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="4f364-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="4f364-178">emailAddressSource</span></span>|[<span data-ttu-id="4f364-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="4f364-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="4f364-180">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたメール属性です。</span><span class="sxs-lookup"><span data-stu-id="4f364-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4f364-181">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4f364-181">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="4f364-182">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="4f364-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="4f364-183">hostName</span><span class="sxs-lookup"><span data-stu-id="4f364-183">hostName</span></span>|<span data-ttu-id="4f364-184">String</span><span class="sxs-lookup"><span data-stu-id="4f364-184">String</span></span>|<span data-ttu-id="4f364-185">Exchange の場所 (URL)、メール ・ アプリケーションに接続します。</span><span class="sxs-lookup"><span data-stu-id="4f364-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="4f364-186">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="4f364-186">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="4f364-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="4f364-187">requireSsl</span></span>|<span data-ttu-id="4f364-188">ブール値</span><span class="sxs-lookup"><span data-stu-id="4f364-188">Boolean</span></span>|<span data-ttu-id="4f364-189">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4f364-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="4f364-190">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="4f364-190">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="4f364-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="4f364-191">usernameSource</span></span>|[<span data-ttu-id="4f364-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="4f364-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="4f364-193">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー名の属性です。</span><span class="sxs-lookup"><span data-stu-id="4f364-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4f364-194">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4f364-194">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="4f364-195">可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="4f364-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="4f364-196">応答</span><span class="sxs-lookup"><span data-stu-id="4f364-196">Response</span></span>
<span data-ttu-id="4f364-197">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4f364-197">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f364-198">例</span><span class="sxs-lookup"><span data-stu-id="4f364-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="4f364-199">要求</span><span class="sxs-lookup"><span data-stu-id="4f364-199">Request</span></span>
<span data-ttu-id="4f364-200">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4f364-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4f364-201">応答</span><span class="sxs-lookup"><span data-stu-id="4f364-201">Response</span></span>
<span data-ttu-id="4f364-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4f364-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





