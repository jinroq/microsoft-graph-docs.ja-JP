---
title: androidForWorkNineWorkEasConfiguration を作成する
description: 新しい androidForWorkNineWorkEasConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9352728e8bc2fdf8557d950582da0b0036abf028
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152753"
---
# <a name="create-androidforworknineworkeasconfiguration"></a><span data-ttu-id="0ade1-103">androidForWorkNineWorkEasConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="0ade1-103">Create androidForWorkNineWorkEasConfiguration</span></span>

> <span data-ttu-id="0ade1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ade1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ade1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ade1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ade1-106">新しい[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0ade1-106">Create a new [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ade1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0ade1-107">Prerequisites</span></span>
<span data-ttu-id="0ade1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0ade1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0ade1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0ade1-110">Permission type</span></span>|<span data-ttu-id="0ade1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0ade1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ade1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0ade1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ade1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ade1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ade1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0ade1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ade1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ade1-115">Not supported.</span></span>|
|<span data-ttu-id="0ade1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0ade1-116">Application</span></span>|<span data-ttu-id="0ade1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ade1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ade1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0ade1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0ade1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ade1-119">Request headers</span></span>
|<span data-ttu-id="0ade1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ade1-120">Header</span></span>|<span data-ttu-id="0ade1-121">値</span><span class="sxs-lookup"><span data-stu-id="0ade1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ade1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ade1-122">Authorization</span></span>|<span data-ttu-id="0ade1-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0ade1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ade1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0ade1-124">Accept</span></span>|<span data-ttu-id="0ade1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0ade1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ade1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0ade1-126">Request body</span></span>
<span data-ttu-id="0ade1-127">要求本文で、androidForWorkNineWorkEasConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0ade1-127">In the request body, supply a JSON representation for the androidForWorkNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="0ade1-128">次の表に、androidForWorkNineWorkEasConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0ade1-128">The following table shows the properties that are required when you create the androidForWorkNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="0ade1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ade1-129">Property</span></span>|<span data-ttu-id="0ade1-130">型</span><span class="sxs-lookup"><span data-stu-id="0ade1-130">Type</span></span>|<span data-ttu-id="0ade1-131">説明</span><span class="sxs-lookup"><span data-stu-id="0ade1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ade1-132">id</span><span class="sxs-lookup"><span data-stu-id="0ade1-132">id</span></span>|<span data-ttu-id="0ade1-133">文字列</span><span class="sxs-lookup"><span data-stu-id="0ade1-133">String</span></span>|<span data-ttu-id="0ade1-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0ade1-134">Key of the entity.</span></span> <span data-ttu-id="0ade1-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ade1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ade1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ade1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0ade1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ade1-137">DateTimeOffset</span></span>|<span data-ttu-id="0ade1-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0ade1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0ade1-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ade1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ade1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0ade1-140">roleScopeTagIds</span></span>|<span data-ttu-id="0ade1-141">String collection</span><span class="sxs-lookup"><span data-stu-id="0ade1-141">String collection</span></span>|<span data-ttu-id="0ade1-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="0ade1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0ade1-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ade1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ade1-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0ade1-144">supportsScopeTags</span></span>|<span data-ttu-id="0ade1-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ade1-145">Boolean</span></span>|<span data-ttu-id="0ade1-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0ade1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0ade1-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="0ade1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0ade1-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="0ade1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0ade1-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="0ade1-149">This property is read-only.</span></span> <span data-ttu-id="0ade1-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ade1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ade1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ade1-151">createdDateTime</span></span>|<span data-ttu-id="0ade1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ade1-152">DateTimeOffset</span></span>|<span data-ttu-id="0ade1-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0ade1-153">DateTime the object was created.</span></span> <span data-ttu-id="0ade1-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ade1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ade1-155">説明</span><span class="sxs-lookup"><span data-stu-id="0ade1-155">description</span></span>|<span data-ttu-id="0ade1-156">文字列</span><span class="sxs-lookup"><span data-stu-id="0ade1-156">String</span></span>|<span data-ttu-id="0ade1-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="0ade1-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0ade1-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ade1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ade1-159">displayName</span><span class="sxs-lookup"><span data-stu-id="0ade1-159">displayName</span></span>|<span data-ttu-id="0ade1-160">String</span><span class="sxs-lookup"><span data-stu-id="0ade1-160">String</span></span>|<span data-ttu-id="0ade1-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="0ade1-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0ade1-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ade1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ade1-163">version</span><span class="sxs-lookup"><span data-stu-id="0ade1-163">version</span></span>|<span data-ttu-id="0ade1-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0ade1-164">Int32</span></span>|<span data-ttu-id="0ade1-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="0ade1-165">Version of the device configuration.</span></span> <span data-ttu-id="0ade1-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0ade1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ade1-167">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0ade1-167">authenticationMethod</span></span>|[<span data-ttu-id="0ade1-168">easauthenticationmethod</span><span class="sxs-lookup"><span data-stu-id="0ade1-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="0ade1-169">Exchange ActiveSync の認証方法。</span><span class="sxs-lookup"><span data-stu-id="0ade1-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="0ade1-170">[androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0ade1-170">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="0ade1-171">使用可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="0ade1-171">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="0ade1-172">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="0ade1-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="0ade1-173">emailsyncduration</span><span class="sxs-lookup"><span data-stu-id="0ade1-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="0ade1-174">電子メールを同期する時間の長さ。</span><span class="sxs-lookup"><span data-stu-id="0ade1-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="0ade1-175">[androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0ade1-175">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="0ade1-176">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="0ade1-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="0ade1-177">emailaddresssource</span><span class="sxs-lookup"><span data-stu-id="0ade1-177">emailAddressSource</span></span>|[<span data-ttu-id="0ade1-178">useremailsource</span><span class="sxs-lookup"><span data-stu-id="0ade1-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="0ade1-179">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="0ade1-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0ade1-180">[androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0ade1-180">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="0ade1-181">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="0ade1-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="0ade1-182">hostName</span><span class="sxs-lookup"><span data-stu-id="0ade1-182">hostName</span></span>|<span data-ttu-id="0ade1-183">String</span><span class="sxs-lookup"><span data-stu-id="0ade1-183">String</span></span>|<span data-ttu-id="0ade1-184">メールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="0ade1-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="0ade1-185">[androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="0ade1-185">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="0ade1-186">requireSsl</span><span class="sxs-lookup"><span data-stu-id="0ade1-186">requireSsl</span></span>|<span data-ttu-id="0ade1-187">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ade1-187">Boolean</span></span>|<span data-ttu-id="0ade1-188">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0ade1-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="0ade1-189">[androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="0ade1-189">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="0ade1-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="0ade1-190">usernameSource</span></span>|[<span data-ttu-id="0ade1-191">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="0ade1-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="0ade1-192">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="0ade1-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0ade1-193">[androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0ade1-193">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="0ade1-194">使用可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="0ade1-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="0ade1-195">synccalendar</span><span class="sxs-lookup"><span data-stu-id="0ade1-195">syncCalendar</span></span>|<span data-ttu-id="0ade1-196">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ade1-196">Boolean</span></span>|<span data-ttu-id="0ade1-197">予定表の同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="0ade1-197">Toggles syncing the calendar.</span></span> <span data-ttu-id="0ade1-198">false に設定すると、予定表はデバイスで無効になります。</span><span class="sxs-lookup"><span data-stu-id="0ade1-198">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="0ade1-199">synccontacts</span><span class="sxs-lookup"><span data-stu-id="0ade1-199">syncContacts</span></span>|<span data-ttu-id="0ade1-200">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ade1-200">Boolean</span></span>|<span data-ttu-id="0ade1-201">連絡先の同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="0ade1-201">Toggles syncing contacts.</span></span> <span data-ttu-id="0ade1-202">false に設定すると、デバイスで [連絡先] がオフになります。</span><span class="sxs-lookup"><span data-stu-id="0ade1-202">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="0ade1-203">synctasks</span><span class="sxs-lookup"><span data-stu-id="0ade1-203">syncTasks</span></span>|<span data-ttu-id="0ade1-204">ブール値</span><span class="sxs-lookup"><span data-stu-id="0ade1-204">Boolean</span></span>|<span data-ttu-id="0ade1-205">タスクの同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="0ade1-205">Toggles syncing tasks.</span></span> <span data-ttu-id="0ade1-206">false タスクに設定した場合は、デバイスで無効になります。</span><span class="sxs-lookup"><span data-stu-id="0ade1-206">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="0ade1-207">応答</span><span class="sxs-lookup"><span data-stu-id="0ade1-207">Response</span></span>
<span data-ttu-id="0ade1-208">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0ade1-208">If successful, this method returns a `201 Created` response code and a [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ade1-209">例</span><span class="sxs-lookup"><span data-stu-id="0ade1-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ade1-210">要求</span><span class="sxs-lookup"><span data-stu-id="0ade1-210">Request</span></span>
<span data-ttu-id="0ade1-211">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0ade1-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 566

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
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
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```

### <a name="response"></a><span data-ttu-id="0ade1-212">応答</span><span class="sxs-lookup"><span data-stu-id="0ade1-212">Response</span></span>
<span data-ttu-id="0ade1-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0ade1-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 738

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
  "id": "f8ef19e0-19e0-f8ef-e019-eff8e019eff8",
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
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```




