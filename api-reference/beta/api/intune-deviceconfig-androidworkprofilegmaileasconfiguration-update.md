---
title: androidwork profilの maileasconfiguration の更新
description: androidwork profilな maileasconfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 40bfa97e8502b68f92c56c2ba31fcef0084caa1a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142036"
---
# <a name="update-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="f4a9e-103">androidwork profilの maileasconfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="f4a9e-103">Update androidWorkProfileGmailEasConfiguration</span></span>

> <span data-ttu-id="f4a9e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4a9e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4a9e-106">[androidwork profilな maileasconfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-106">Update the properties of a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4a9e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f4a9e-107">Prerequisites</span></span>
<span data-ttu-id="f4a9e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f4a9e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f4a9e-110">Permission type</span></span>|<span data-ttu-id="f4a9e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f4a9e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4a9e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f4a9e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4a9e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4a9e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4a9e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f4a9e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4a9e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-115">Not supported.</span></span>|
|<span data-ttu-id="f4a9e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f4a9e-116">Application</span></span>|<span data-ttu-id="f4a9e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4a9e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f4a9e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f4a9e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4a9e-119">Request headers</span></span>
|<span data-ttu-id="f4a9e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4a9e-120">Header</span></span>|<span data-ttu-id="f4a9e-121">値</span><span class="sxs-lookup"><span data-stu-id="f4a9e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4a9e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4a9e-122">Authorization</span></span>|<span data-ttu-id="f4a9e-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4a9e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f4a9e-124">Accept</span></span>|<span data-ttu-id="f4a9e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4a9e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4a9e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f4a9e-126">Request body</span></span>
<span data-ttu-id="f4a9e-127">要求本文で、 [androidwork profilな maileasconfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-127">In the request body, supply a JSON representation for the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="f4a9e-128">次の表に、 [androidwork profilare maileasconfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-128">The following table shows the properties that are required when you create the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md).</span></span>

|<span data-ttu-id="f4a9e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4a9e-129">Property</span></span>|<span data-ttu-id="f4a9e-130">型</span><span class="sxs-lookup"><span data-stu-id="f4a9e-130">Type</span></span>|<span data-ttu-id="f4a9e-131">説明</span><span class="sxs-lookup"><span data-stu-id="f4a9e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4a9e-132">id</span><span class="sxs-lookup"><span data-stu-id="f4a9e-132">id</span></span>|<span data-ttu-id="f4a9e-133">文字列</span><span class="sxs-lookup"><span data-stu-id="f4a9e-133">String</span></span>|<span data-ttu-id="f4a9e-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-134">Key of the entity.</span></span> <span data-ttu-id="f4a9e-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f4a9e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4a9e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4a9e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f4a9e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4a9e-137">DateTimeOffset</span></span>|<span data-ttu-id="f4a9e-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f4a9e-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f4a9e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4a9e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f4a9e-140">roleScopeTagIds</span></span>|<span data-ttu-id="f4a9e-141">String collection</span><span class="sxs-lookup"><span data-stu-id="f4a9e-141">String collection</span></span>|<span data-ttu-id="f4a9e-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f4a9e-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f4a9e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4a9e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f4a9e-144">supportsScopeTags</span></span>|<span data-ttu-id="f4a9e-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="f4a9e-145">Boolean</span></span>|<span data-ttu-id="f4a9e-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f4a9e-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f4a9e-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f4a9e-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-149">This property is read-only.</span></span> <span data-ttu-id="f4a9e-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f4a9e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4a9e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4a9e-151">createdDateTime</span></span>|<span data-ttu-id="f4a9e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4a9e-152">DateTimeOffset</span></span>|<span data-ttu-id="f4a9e-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-153">DateTime the object was created.</span></span> <span data-ttu-id="f4a9e-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f4a9e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4a9e-155">説明</span><span class="sxs-lookup"><span data-stu-id="f4a9e-155">description</span></span>|<span data-ttu-id="f4a9e-156">文字列</span><span class="sxs-lookup"><span data-stu-id="f4a9e-156">String</span></span>|<span data-ttu-id="f4a9e-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f4a9e-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f4a9e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4a9e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f4a9e-159">displayName</span></span>|<span data-ttu-id="f4a9e-160">String</span><span class="sxs-lookup"><span data-stu-id="f4a9e-160">String</span></span>|<span data-ttu-id="f4a9e-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f4a9e-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f4a9e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4a9e-163">version</span><span class="sxs-lookup"><span data-stu-id="f4a9e-163">version</span></span>|<span data-ttu-id="f4a9e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f4a9e-164">Int32</span></span>|<span data-ttu-id="f4a9e-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-165">Version of the device configuration.</span></span> <span data-ttu-id="f4a9e-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f4a9e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4a9e-167">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f4a9e-167">authenticationMethod</span></span>|[<span data-ttu-id="f4a9e-168">easauthenticationmethod</span><span class="sxs-lookup"><span data-stu-id="f4a9e-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="f4a9e-169">Exchange ActiveSync の認証方法。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="f4a9e-170">[androidwork profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-170">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="f4a9e-171">使用可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-171">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="f4a9e-172">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="f4a9e-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="f4a9e-173">emailsyncduration</span><span class="sxs-lookup"><span data-stu-id="f4a9e-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="f4a9e-174">電子メールを同期する時間の長さ。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="f4a9e-175">[androidwork profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-175">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="f4a9e-176">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="f4a9e-177">emailaddresssource</span><span class="sxs-lookup"><span data-stu-id="f4a9e-177">emailAddressSource</span></span>|[<span data-ttu-id="f4a9e-178">useremailsource</span><span class="sxs-lookup"><span data-stu-id="f4a9e-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="f4a9e-179">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="f4a9e-180">[androidwork profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-180">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="f4a9e-181">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="f4a9e-182">hostName</span><span class="sxs-lookup"><span data-stu-id="f4a9e-182">hostName</span></span>|<span data-ttu-id="f4a9e-183">String</span><span class="sxs-lookup"><span data-stu-id="f4a9e-183">String</span></span>|<span data-ttu-id="f4a9e-184">メールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="f4a9e-185">[androidwork profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f4a9e-185">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="f4a9e-186">requireSsl</span><span class="sxs-lookup"><span data-stu-id="f4a9e-186">requireSsl</span></span>|<span data-ttu-id="f4a9e-187">ブール値</span><span class="sxs-lookup"><span data-stu-id="f4a9e-187">Boolean</span></span>|<span data-ttu-id="f4a9e-188">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="f4a9e-189">[androidwork profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f4a9e-189">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="f4a9e-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="f4a9e-190">usernameSource</span></span>|[<span data-ttu-id="f4a9e-191">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="f4a9e-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="f4a9e-192">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="f4a9e-193">[androidwork profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="f4a9e-194">可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="f4a9e-195">応答</span><span class="sxs-lookup"><span data-stu-id="f4a9e-195">Response</span></span>
<span data-ttu-id="f4a9e-196">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidwork profilな maileasconfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-196">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4a9e-197">例</span><span class="sxs-lookup"><span data-stu-id="f4a9e-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4a9e-198">要求</span><span class="sxs-lookup"><span data-stu-id="f4a9e-198">Request</span></span>
<span data-ttu-id="f4a9e-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="f4a9e-200">応答</span><span class="sxs-lookup"><span data-stu-id="f4a9e-200">Response</span></span>
<span data-ttu-id="f4a9e-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f4a9e-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




