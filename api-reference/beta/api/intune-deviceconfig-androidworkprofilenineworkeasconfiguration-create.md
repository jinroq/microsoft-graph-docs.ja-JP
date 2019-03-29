---
title: androidwork profileninework keasconfiguration の作成
description: 新しい androidwork profileninework keasconfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 555ddaa8819dd52cc1caba3e8b98f1981e055f11
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969387"
---
# <a name="create-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="b275b-103">androidwork profileninework keasconfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="b275b-103">Create androidWorkProfileNineWorkEasConfiguration</span></span>

> <span data-ttu-id="b275b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b275b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b275b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b275b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b275b-106">新しい[androidwork profileninework keasconfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b275b-106">Create a new [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b275b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b275b-107">Prerequisites</span></span>
<span data-ttu-id="b275b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b275b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b275b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b275b-110">Permission type</span></span>|<span data-ttu-id="b275b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b275b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b275b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b275b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b275b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b275b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b275b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b275b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b275b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b275b-115">Not supported.</span></span>|
|<span data-ttu-id="b275b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b275b-116">Application</span></span>|<span data-ttu-id="b275b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b275b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b275b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b275b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b275b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b275b-119">Request headers</span></span>
|<span data-ttu-id="b275b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b275b-120">Header</span></span>|<span data-ttu-id="b275b-121">値</span><span class="sxs-lookup"><span data-stu-id="b275b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b275b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b275b-122">Authorization</span></span>|<span data-ttu-id="b275b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b275b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b275b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b275b-124">Accept</span></span>|<span data-ttu-id="b275b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b275b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b275b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b275b-126">Request body</span></span>
<span data-ttu-id="b275b-127">要求本文で、androidwork profileninework keasconfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b275b-127">In the request body, supply a JSON representation for the androidWorkProfileNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="b275b-128">次の表に、androidwork profileninework keasconfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b275b-128">The following table shows the properties that are required when you create the androidWorkProfileNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="b275b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b275b-129">Property</span></span>|<span data-ttu-id="b275b-130">型</span><span class="sxs-lookup"><span data-stu-id="b275b-130">Type</span></span>|<span data-ttu-id="b275b-131">説明</span><span class="sxs-lookup"><span data-stu-id="b275b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b275b-132">id</span><span class="sxs-lookup"><span data-stu-id="b275b-132">id</span></span>|<span data-ttu-id="b275b-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b275b-133">String</span></span>|<span data-ttu-id="b275b-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b275b-134">Key of the entity.</span></span> <span data-ttu-id="b275b-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b275b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b275b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b275b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b275b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b275b-137">DateTimeOffset</span></span>|<span data-ttu-id="b275b-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="b275b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b275b-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b275b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b275b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b275b-140">roleScopeTagIds</span></span>|<span data-ttu-id="b275b-141">String collection</span><span class="sxs-lookup"><span data-stu-id="b275b-141">String collection</span></span>|<span data-ttu-id="b275b-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="b275b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b275b-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b275b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b275b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b275b-144">supportsScopeTags</span></span>|<span data-ttu-id="b275b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b275b-145">Boolean</span></span>|<span data-ttu-id="b275b-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b275b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b275b-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="b275b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b275b-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="b275b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b275b-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="b275b-149">This property is read-only.</span></span> <span data-ttu-id="b275b-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b275b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b275b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b275b-151">createdDateTime</span></span>|<span data-ttu-id="b275b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b275b-152">DateTimeOffset</span></span>|<span data-ttu-id="b275b-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b275b-153">DateTime the object was created.</span></span> <span data-ttu-id="b275b-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b275b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b275b-155">description</span><span class="sxs-lookup"><span data-stu-id="b275b-155">description</span></span>|<span data-ttu-id="b275b-156">String</span><span class="sxs-lookup"><span data-stu-id="b275b-156">String</span></span>|<span data-ttu-id="b275b-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="b275b-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b275b-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b275b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b275b-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b275b-159">displayName</span></span>|<span data-ttu-id="b275b-160">String</span><span class="sxs-lookup"><span data-stu-id="b275b-160">String</span></span>|<span data-ttu-id="b275b-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="b275b-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b275b-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b275b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b275b-163">version</span><span class="sxs-lookup"><span data-stu-id="b275b-163">version</span></span>|<span data-ttu-id="b275b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b275b-164">Int32</span></span>|<span data-ttu-id="b275b-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="b275b-165">Version of the device configuration.</span></span> <span data-ttu-id="b275b-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b275b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b275b-167">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b275b-167">authenticationMethod</span></span>|[<span data-ttu-id="b275b-168">easauthenticationmethod</span><span class="sxs-lookup"><span data-stu-id="b275b-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="b275b-169">Exchange ActiveSync の認証方法。</span><span class="sxs-lookup"><span data-stu-id="b275b-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="b275b-170">[androidwork profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="b275b-170">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="b275b-171">可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="b275b-171">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="b275b-172">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="b275b-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="b275b-173">emailsyncduration</span><span class="sxs-lookup"><span data-stu-id="b275b-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="b275b-174">電子メールを同期する時間の長さ。</span><span class="sxs-lookup"><span data-stu-id="b275b-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="b275b-175">[androidwork profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="b275b-175">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="b275b-176">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="b275b-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="b275b-177">emailaddresssource</span><span class="sxs-lookup"><span data-stu-id="b275b-177">emailAddressSource</span></span>|[<span data-ttu-id="b275b-178">useremailsource</span><span class="sxs-lookup"><span data-stu-id="b275b-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="b275b-179">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="b275b-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b275b-180">[androidwork profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="b275b-180">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="b275b-181">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="b275b-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="b275b-182">hostName</span><span class="sxs-lookup"><span data-stu-id="b275b-182">hostName</span></span>|<span data-ttu-id="b275b-183">String</span><span class="sxs-lookup"><span data-stu-id="b275b-183">String</span></span>|<span data-ttu-id="b275b-184">メールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="b275b-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="b275b-185">[androidwork profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="b275b-185">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="b275b-186">requireSsl</span><span class="sxs-lookup"><span data-stu-id="b275b-186">requireSsl</span></span>|<span data-ttu-id="b275b-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="b275b-187">Boolean</span></span>|<span data-ttu-id="b275b-188">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b275b-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="b275b-189">[androidwork profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="b275b-189">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="b275b-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="b275b-190">usernameSource</span></span>|[<span data-ttu-id="b275b-191">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="b275b-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="b275b-192">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="b275b-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b275b-193">[androidwork profileeasemailprofilebase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="b275b-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="b275b-194">可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="b275b-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="b275b-195">synccalendar</span><span class="sxs-lookup"><span data-stu-id="b275b-195">syncCalendar</span></span>|<span data-ttu-id="b275b-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="b275b-196">Boolean</span></span>|<span data-ttu-id="b275b-197">予定表の同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="b275b-197">Toggles syncing the calendar.</span></span> <span data-ttu-id="b275b-198">false に設定すると、予定表はデバイスで無効になります。</span><span class="sxs-lookup"><span data-stu-id="b275b-198">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="b275b-199">synccontacts</span><span class="sxs-lookup"><span data-stu-id="b275b-199">syncContacts</span></span>|<span data-ttu-id="b275b-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="b275b-200">Boolean</span></span>|<span data-ttu-id="b275b-201">連絡先の同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="b275b-201">Toggles syncing contacts.</span></span> <span data-ttu-id="b275b-202">false に設定すると、デバイスで [連絡先] がオフになります。</span><span class="sxs-lookup"><span data-stu-id="b275b-202">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="b275b-203">synctasks</span><span class="sxs-lookup"><span data-stu-id="b275b-203">syncTasks</span></span>|<span data-ttu-id="b275b-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="b275b-204">Boolean</span></span>|<span data-ttu-id="b275b-205">タスクの同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="b275b-205">Toggles syncing tasks.</span></span> <span data-ttu-id="b275b-206">false タスクに設定した場合は、デバイスで無効になります。</span><span class="sxs-lookup"><span data-stu-id="b275b-206">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="b275b-207">応答</span><span class="sxs-lookup"><span data-stu-id="b275b-207">Response</span></span>
<span data-ttu-id="b275b-208">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidwork profileninework keasconfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b275b-208">If successful, this method returns a `201 Created` response code and a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b275b-209">例</span><span class="sxs-lookup"><span data-stu-id="b275b-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="b275b-210">要求</span><span class="sxs-lookup"><span data-stu-id="b275b-210">Request</span></span>
<span data-ttu-id="b275b-211">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b275b-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 570

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="b275b-212">応答</span><span class="sxs-lookup"><span data-stu-id="b275b-212">Response</span></span>
<span data-ttu-id="b275b-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b275b-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 742

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
  "id": "3d9e3a30-3a30-3d9e-303a-9e3d303a9e3d",
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




