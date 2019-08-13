---
title: Androidwork Profileninework Keasconfiguration の作成
description: 新しい Androidwork Profileninework Keasconfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ba5b9d47ea07c818b2fe1de74c318ce6bc17fae
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36340734"
---
# <a name="create-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="7e9b8-103">Androidwork Profileninework Keasconfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="7e9b8-103">Create androidWorkProfileNineWorkEasConfiguration</span></span>

> <span data-ttu-id="7e9b8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e9b8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e9b8-106">新しい[Androidwork Profileninework Keasconfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-106">Create a new [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e9b8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7e9b8-107">Prerequisites</span></span>
<span data-ttu-id="7e9b8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e9b8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7e9b8-110">Permission type</span></span>|<span data-ttu-id="7e9b8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7e9b8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e9b8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7e9b8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7e9b8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e9b8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7e9b8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7e9b8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e9b8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-115">Not supported.</span></span>|
|<span data-ttu-id="7e9b8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7e9b8-116">Application</span></span>|<span data-ttu-id="7e9b8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e9b8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e9b8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7e9b8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7e9b8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e9b8-119">Request headers</span></span>
|<span data-ttu-id="7e9b8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e9b8-120">Header</span></span>|<span data-ttu-id="7e9b8-121">値</span><span class="sxs-lookup"><span data-stu-id="7e9b8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e9b8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e9b8-122">Authorization</span></span>|<span data-ttu-id="7e9b8-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e9b8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7e9b8-124">Accept</span></span>|<span data-ttu-id="7e9b8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7e9b8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e9b8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7e9b8-126">Request body</span></span>
<span data-ttu-id="7e9b8-127">要求本文で、Androidwork Profileninework Keasconfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-127">In the request body, supply a JSON representation for the androidWorkProfileNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="7e9b8-128">次の表に、Androidwork Profileninework Keasconfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-128">The following table shows the properties that are required when you create the androidWorkProfileNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="7e9b8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e9b8-129">Property</span></span>|<span data-ttu-id="7e9b8-130">型</span><span class="sxs-lookup"><span data-stu-id="7e9b8-130">Type</span></span>|<span data-ttu-id="7e9b8-131">説明</span><span class="sxs-lookup"><span data-stu-id="7e9b8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e9b8-132">id</span><span class="sxs-lookup"><span data-stu-id="7e9b8-132">id</span></span>|<span data-ttu-id="7e9b8-133">文字列</span><span class="sxs-lookup"><span data-stu-id="7e9b8-133">String</span></span>|<span data-ttu-id="7e9b8-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-134">Key of the entity.</span></span> <span data-ttu-id="7e9b8-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e9b8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9b8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e9b8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7e9b8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e9b8-137">DateTimeOffset</span></span>|<span data-ttu-id="7e9b8-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7e9b8-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e9b8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9b8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7e9b8-140">roleScopeTagIds</span></span>|<span data-ttu-id="7e9b8-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="7e9b8-141">String collection</span></span>|<span data-ttu-id="7e9b8-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7e9b8-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e9b8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9b8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7e9b8-144">supportsScopeTags</span></span>|<span data-ttu-id="7e9b8-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e9b8-145">Boolean</span></span>|<span data-ttu-id="7e9b8-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7e9b8-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7e9b8-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7e9b8-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-149">This property is read-only.</span></span> <span data-ttu-id="7e9b8-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e9b8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9b8-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7e9b8-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7e9b8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7e9b8-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7e9b8-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7e9b8-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e9b8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9b8-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7e9b8-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7e9b8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7e9b8-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7e9b8-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7e9b8-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e9b8-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9b8-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="7e9b8-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7e9b8-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="7e9b8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7e9b8-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7e9b8-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e9b8-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9b8-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e9b8-163">createdDateTime</span></span>|<span data-ttu-id="7e9b8-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e9b8-164">DateTimeOffset</span></span>|<span data-ttu-id="7e9b8-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-165">DateTime the object was created.</span></span> <span data-ttu-id="7e9b8-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e9b8-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9b8-167">description</span><span class="sxs-lookup"><span data-stu-id="7e9b8-167">description</span></span>|<span data-ttu-id="7e9b8-168">String</span><span class="sxs-lookup"><span data-stu-id="7e9b8-168">String</span></span>|<span data-ttu-id="7e9b8-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7e9b8-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e9b8-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9b8-171">displayName</span><span class="sxs-lookup"><span data-stu-id="7e9b8-171">displayName</span></span>|<span data-ttu-id="7e9b8-172">String</span><span class="sxs-lookup"><span data-stu-id="7e9b8-172">String</span></span>|<span data-ttu-id="7e9b8-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7e9b8-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e9b8-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9b8-175">version</span><span class="sxs-lookup"><span data-stu-id="7e9b8-175">version</span></span>|<span data-ttu-id="7e9b8-176">Int32</span><span class="sxs-lookup"><span data-stu-id="7e9b8-176">Int32</span></span>|<span data-ttu-id="7e9b8-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-177">Version of the device configuration.</span></span> <span data-ttu-id="7e9b8-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e9b8-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e9b8-179">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7e9b8-179">authenticationMethod</span></span>|[<span data-ttu-id="7e9b8-180">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7e9b8-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="7e9b8-181">Exchange ActiveSync の認証方法。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="7e9b8-182">[Androidwork Profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-182">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="7e9b8-183">可能な値は、`usernameAndPassword`、`certificate`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="7e9b8-184">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="7e9b8-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="7e9b8-185">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="7e9b8-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="7e9b8-186">電子メールを同期する時間の長さ。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="7e9b8-187">[Androidwork Profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-187">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="7e9b8-188">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="7e9b8-189">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="7e9b8-189">emailAddressSource</span></span>|[<span data-ttu-id="7e9b8-190">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="7e9b8-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="7e9b8-191">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7e9b8-192">[Androidwork Profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-192">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="7e9b8-193">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7e9b8-194">hostName</span><span class="sxs-lookup"><span data-stu-id="7e9b8-194">hostName</span></span>|<span data-ttu-id="7e9b8-195">String</span><span class="sxs-lookup"><span data-stu-id="7e9b8-195">String</span></span>|<span data-ttu-id="7e9b8-196">メールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="7e9b8-197">[Androidwork Profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="7e9b8-197">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="7e9b8-198">requireSsl</span><span class="sxs-lookup"><span data-stu-id="7e9b8-198">requireSsl</span></span>|<span data-ttu-id="7e9b8-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e9b8-199">Boolean</span></span>|<span data-ttu-id="7e9b8-200">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="7e9b8-201">[Androidwork Profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="7e9b8-201">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="7e9b8-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="7e9b8-202">usernameSource</span></span>|[<span data-ttu-id="7e9b8-203">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="7e9b8-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="7e9b8-204">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7e9b8-205">[Androidwork Profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-205">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="7e9b8-206">使用可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7e9b8-207">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="7e9b8-207">syncCalendar</span></span>|<span data-ttu-id="7e9b8-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e9b8-208">Boolean</span></span>|<span data-ttu-id="7e9b8-209">予定表の同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-209">Toggles syncing the calendar.</span></span> <span data-ttu-id="7e9b8-210">False に設定すると、予定表はデバイスで無効になります。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-210">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="7e9b8-211">syncContacts</span><span class="sxs-lookup"><span data-stu-id="7e9b8-211">syncContacts</span></span>|<span data-ttu-id="7e9b8-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e9b8-212">Boolean</span></span>|<span data-ttu-id="7e9b8-213">連絡先の同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-213">Toggles syncing contacts.</span></span> <span data-ttu-id="7e9b8-214">False に設定すると、デバイスで [連絡先] がオフになります。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-214">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="7e9b8-215">syncTasks</span><span class="sxs-lookup"><span data-stu-id="7e9b8-215">syncTasks</span></span>|<span data-ttu-id="7e9b8-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e9b8-216">Boolean</span></span>|<span data-ttu-id="7e9b8-217">タスクの同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-217">Toggles syncing tasks.</span></span> <span data-ttu-id="7e9b8-218">False タスクに設定した場合は、デバイスで無効になります。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-218">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="7e9b8-219">応答</span><span class="sxs-lookup"><span data-stu-id="7e9b8-219">Response</span></span>
<span data-ttu-id="7e9b8-220">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Androidwork Profileninework keasconfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-220">If successful, this method returns a `201 Created` response code and a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e9b8-221">例</span><span class="sxs-lookup"><span data-stu-id="7e9b8-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e9b8-222">要求</span><span class="sxs-lookup"><span data-stu-id="7e9b8-222">Request</span></span>
<span data-ttu-id="7e9b8-223">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1343

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="7e9b8-224">応答</span><span class="sxs-lookup"><span data-stu-id="7e9b8-224">Response</span></span>
<span data-ttu-id="7e9b8-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7e9b8-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1515

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
  "id": "3d9e3a30-3a30-3d9e-303a-9e3d303a9e3d",
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






