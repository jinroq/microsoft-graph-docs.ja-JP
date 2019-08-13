---
title: AndroidForWorkNineWorkEasConfiguration の更新
description: AndroidForWorkNineWorkEasConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b10ef76ca530afef886c5a65d1fe7aa8e387aa06
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36312027"
---
# <a name="update-androidforworknineworkeasconfiguration"></a><span data-ttu-id="57951-103">AndroidForWorkNineWorkEasConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="57951-103">Update androidForWorkNineWorkEasConfiguration</span></span>

> <span data-ttu-id="57951-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57951-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57951-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="57951-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57951-106">[AndroidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="57951-106">Update the properties of a [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57951-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="57951-107">Prerequisites</span></span>
<span data-ttu-id="57951-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="57951-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57951-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="57951-110">Permission type</span></span>|<span data-ttu-id="57951-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="57951-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57951-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="57951-112">Delegated (work or school account)</span></span>|<span data-ttu-id="57951-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57951-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="57951-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="57951-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57951-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57951-115">Not supported.</span></span>|
|<span data-ttu-id="57951-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="57951-116">Application</span></span>|<span data-ttu-id="57951-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57951-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57951-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="57951-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="57951-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="57951-119">Request headers</span></span>
|<span data-ttu-id="57951-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="57951-120">Header</span></span>|<span data-ttu-id="57951-121">値</span><span class="sxs-lookup"><span data-stu-id="57951-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57951-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="57951-122">Authorization</span></span>|<span data-ttu-id="57951-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="57951-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57951-124">承諾</span><span class="sxs-lookup"><span data-stu-id="57951-124">Accept</span></span>|<span data-ttu-id="57951-125">application/json</span><span class="sxs-lookup"><span data-stu-id="57951-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57951-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="57951-126">Request body</span></span>
<span data-ttu-id="57951-127">要求本文で、 [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="57951-127">In the request body, supply a JSON representation for the [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

<span data-ttu-id="57951-128">次の表に、 [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="57951-128">The following table shows the properties that are required when you create the [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md).</span></span>

|<span data-ttu-id="57951-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57951-129">Property</span></span>|<span data-ttu-id="57951-130">型</span><span class="sxs-lookup"><span data-stu-id="57951-130">Type</span></span>|<span data-ttu-id="57951-131">説明</span><span class="sxs-lookup"><span data-stu-id="57951-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57951-132">id</span><span class="sxs-lookup"><span data-stu-id="57951-132">id</span></span>|<span data-ttu-id="57951-133">文字列</span><span class="sxs-lookup"><span data-stu-id="57951-133">String</span></span>|<span data-ttu-id="57951-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="57951-134">Key of the entity.</span></span> <span data-ttu-id="57951-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57951-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57951-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="57951-136">lastModifiedDateTime</span></span>|<span data-ttu-id="57951-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57951-137">DateTimeOffset</span></span>|<span data-ttu-id="57951-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="57951-138">DateTime the object was last modified.</span></span> <span data-ttu-id="57951-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57951-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57951-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="57951-140">roleScopeTagIds</span></span>|<span data-ttu-id="57951-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="57951-141">String collection</span></span>|<span data-ttu-id="57951-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="57951-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="57951-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57951-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57951-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="57951-144">supportsScopeTags</span></span>|<span data-ttu-id="57951-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="57951-145">Boolean</span></span>|<span data-ttu-id="57951-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="57951-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="57951-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="57951-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="57951-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="57951-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="57951-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="57951-149">This property is read-only.</span></span> <span data-ttu-id="57951-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57951-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57951-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="57951-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="57951-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="57951-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="57951-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="57951-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="57951-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57951-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57951-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="57951-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="57951-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="57951-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="57951-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="57951-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="57951-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57951-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57951-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="57951-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="57951-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="57951-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="57951-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="57951-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="57951-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57951-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57951-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="57951-163">createdDateTime</span></span>|<span data-ttu-id="57951-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57951-164">DateTimeOffset</span></span>|<span data-ttu-id="57951-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="57951-165">DateTime the object was created.</span></span> <span data-ttu-id="57951-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57951-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57951-167">description</span><span class="sxs-lookup"><span data-stu-id="57951-167">description</span></span>|<span data-ttu-id="57951-168">String</span><span class="sxs-lookup"><span data-stu-id="57951-168">String</span></span>|<span data-ttu-id="57951-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="57951-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="57951-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57951-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57951-171">displayName</span><span class="sxs-lookup"><span data-stu-id="57951-171">displayName</span></span>|<span data-ttu-id="57951-172">String</span><span class="sxs-lookup"><span data-stu-id="57951-172">String</span></span>|<span data-ttu-id="57951-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="57951-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="57951-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57951-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57951-175">version</span><span class="sxs-lookup"><span data-stu-id="57951-175">version</span></span>|<span data-ttu-id="57951-176">Int32</span><span class="sxs-lookup"><span data-stu-id="57951-176">Int32</span></span>|<span data-ttu-id="57951-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="57951-177">Version of the device configuration.</span></span> <span data-ttu-id="57951-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57951-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57951-179">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="57951-179">authenticationMethod</span></span>|[<span data-ttu-id="57951-180">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="57951-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="57951-181">Exchange ActiveSync の認証方法。</span><span class="sxs-lookup"><span data-stu-id="57951-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="57951-182">[Androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="57951-182">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="57951-183">可能な値は、`usernameAndPassword`、`certificate`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="57951-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="57951-184">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="57951-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="57951-185">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="57951-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="57951-186">電子メールを同期する時間の長さ。</span><span class="sxs-lookup"><span data-stu-id="57951-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="57951-187">[Androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="57951-187">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="57951-188">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="57951-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="57951-189">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="57951-189">emailAddressSource</span></span>|[<span data-ttu-id="57951-190">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="57951-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="57951-191">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="57951-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="57951-192">[Androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="57951-192">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="57951-193">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="57951-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="57951-194">hostName</span><span class="sxs-lookup"><span data-stu-id="57951-194">hostName</span></span>|<span data-ttu-id="57951-195">String</span><span class="sxs-lookup"><span data-stu-id="57951-195">String</span></span>|<span data-ttu-id="57951-196">メールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="57951-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="57951-197">[Androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="57951-197">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="57951-198">requireSsl</span><span class="sxs-lookup"><span data-stu-id="57951-198">requireSsl</span></span>|<span data-ttu-id="57951-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="57951-199">Boolean</span></span>|<span data-ttu-id="57951-200">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="57951-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="57951-201">[Androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="57951-201">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="57951-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="57951-202">usernameSource</span></span>|[<span data-ttu-id="57951-203">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="57951-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="57951-204">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="57951-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="57951-205">[Androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="57951-205">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="57951-206">使用可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="57951-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="57951-207">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="57951-207">syncCalendar</span></span>|<span data-ttu-id="57951-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="57951-208">Boolean</span></span>|<span data-ttu-id="57951-209">予定表の同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="57951-209">Toggles syncing the calendar.</span></span> <span data-ttu-id="57951-210">False に設定すると、予定表はデバイスで無効になります。</span><span class="sxs-lookup"><span data-stu-id="57951-210">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="57951-211">syncContacts</span><span class="sxs-lookup"><span data-stu-id="57951-211">syncContacts</span></span>|<span data-ttu-id="57951-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="57951-212">Boolean</span></span>|<span data-ttu-id="57951-213">連絡先の同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="57951-213">Toggles syncing contacts.</span></span> <span data-ttu-id="57951-214">False に設定すると、デバイスで [連絡先] がオフになります。</span><span class="sxs-lookup"><span data-stu-id="57951-214">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="57951-215">syncTasks</span><span class="sxs-lookup"><span data-stu-id="57951-215">syncTasks</span></span>|<span data-ttu-id="57951-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="57951-216">Boolean</span></span>|<span data-ttu-id="57951-217">タスクの同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="57951-217">Toggles syncing tasks.</span></span> <span data-ttu-id="57951-218">False タスクに設定した場合は、デバイスで無効になります。</span><span class="sxs-lookup"><span data-stu-id="57951-218">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="57951-219">応答</span><span class="sxs-lookup"><span data-stu-id="57951-219">Response</span></span>
<span data-ttu-id="57951-220">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="57951-220">If successful, this method returns a `200 OK` response code and an updated [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57951-221">例</span><span class="sxs-lookup"><span data-stu-id="57951-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="57951-222">要求</span><span class="sxs-lookup"><span data-stu-id="57951-222">Request</span></span>
<span data-ttu-id="57951-223">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="57951-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1339

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```

### <a name="response"></a><span data-ttu-id="57951-224">応答</span><span class="sxs-lookup"><span data-stu-id="57951-224">Response</span></span>
<span data-ttu-id="57951-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="57951-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1511

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
  "id": "f8ef19e0-19e0-f8ef-e019-eff8e019eff8",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```






