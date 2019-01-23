---
title: AndroidWorkProfileNineWorkEasConfiguration を作成します。
description: 新しい androidWorkProfileNineWorkEasConfiguration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6370675d0e14d35ea3a762ae0c3e99ccd9945fb0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425387"
---
# <a name="create-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="37338-103">AndroidWorkProfileNineWorkEasConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="37338-103">Create androidWorkProfileNineWorkEasConfiguration</span></span>

> <span data-ttu-id="37338-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="37338-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="37338-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37338-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37338-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="37338-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37338-107">新しい[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="37338-107">Create a new [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37338-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="37338-108">Prerequisites</span></span>
<span data-ttu-id="37338-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="37338-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="37338-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="37338-111">Permission type</span></span>|<span data-ttu-id="37338-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="37338-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37338-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="37338-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37338-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37338-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37338-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="37338-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37338-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37338-116">Not supported.</span></span>|
|<span data-ttu-id="37338-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="37338-117">Application</span></span>|<span data-ttu-id="37338-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37338-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37338-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="37338-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="37338-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37338-120">Request headers</span></span>
|<span data-ttu-id="37338-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37338-121">Header</span></span>|<span data-ttu-id="37338-122">値</span><span class="sxs-lookup"><span data-stu-id="37338-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37338-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="37338-123">Authorization</span></span>|<span data-ttu-id="37338-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="37338-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37338-125">Accept</span><span class="sxs-lookup"><span data-stu-id="37338-125">Accept</span></span>|<span data-ttu-id="37338-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37338-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37338-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="37338-127">Request body</span></span>
<span data-ttu-id="37338-128">要求の本文に androidWorkProfileNineWorkEasConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="37338-128">In the request body, supply a JSON representation for the androidWorkProfileNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="37338-129">次の表は、androidWorkProfileNineWorkEasConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="37338-129">The following table shows the properties that are required when you create the androidWorkProfileNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="37338-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37338-130">Property</span></span>|<span data-ttu-id="37338-131">型</span><span class="sxs-lookup"><span data-stu-id="37338-131">Type</span></span>|<span data-ttu-id="37338-132">説明</span><span class="sxs-lookup"><span data-stu-id="37338-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37338-133">id</span><span class="sxs-lookup"><span data-stu-id="37338-133">id</span></span>|<span data-ttu-id="37338-134">String</span><span class="sxs-lookup"><span data-stu-id="37338-134">String</span></span>|<span data-ttu-id="37338-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="37338-135">Key of the entity.</span></span> <span data-ttu-id="37338-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="37338-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37338-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37338-137">lastModifiedDateTime</span></span>|<span data-ttu-id="37338-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37338-138">DateTimeOffset</span></span>|<span data-ttu-id="37338-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="37338-139">DateTime the object was last modified.</span></span> <span data-ttu-id="37338-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="37338-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37338-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="37338-141">roleScopeTagIds</span></span>|<span data-ttu-id="37338-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="37338-142">String collection</span></span>|<span data-ttu-id="37338-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="37338-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="37338-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="37338-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37338-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="37338-145">supportsScopeTags</span></span>|<span data-ttu-id="37338-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="37338-146">Boolean</span></span>|<span data-ttu-id="37338-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="37338-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="37338-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="37338-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="37338-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="37338-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="37338-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="37338-150">This property is read-only.</span></span> <span data-ttu-id="37338-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="37338-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37338-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37338-152">createdDateTime</span></span>|<span data-ttu-id="37338-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37338-153">DateTimeOffset</span></span>|<span data-ttu-id="37338-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="37338-154">DateTime the object was created.</span></span> <span data-ttu-id="37338-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="37338-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37338-156">説明</span><span class="sxs-lookup"><span data-stu-id="37338-156">description</span></span>|<span data-ttu-id="37338-157">String</span><span class="sxs-lookup"><span data-stu-id="37338-157">String</span></span>|<span data-ttu-id="37338-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="37338-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="37338-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="37338-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37338-160">displayName</span><span class="sxs-lookup"><span data-stu-id="37338-160">displayName</span></span>|<span data-ttu-id="37338-161">String</span><span class="sxs-lookup"><span data-stu-id="37338-161">String</span></span>|<span data-ttu-id="37338-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="37338-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="37338-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="37338-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37338-164">version</span><span class="sxs-lookup"><span data-stu-id="37338-164">version</span></span>|<span data-ttu-id="37338-165">Int32</span><span class="sxs-lookup"><span data-stu-id="37338-165">Int32</span></span>|<span data-ttu-id="37338-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="37338-166">Version of the device configuration.</span></span> <span data-ttu-id="37338-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="37338-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37338-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="37338-168">authenticationMethod</span></span>|[<span data-ttu-id="37338-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="37338-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="37338-170">Exchange ActiveSync の認証方法です。</span><span class="sxs-lookup"><span data-stu-id="37338-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="37338-171">[AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="37338-171">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="37338-172">使用可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="37338-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="37338-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="37338-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="37338-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="37338-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="37338-175">電子メールの時間の期間に同期する必要があります。</span><span class="sxs-lookup"><span data-stu-id="37338-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="37338-176">[AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="37338-176">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="37338-177">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="37338-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="37338-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="37338-178">emailAddressSource</span></span>|[<span data-ttu-id="37338-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="37338-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="37338-180">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたメール属性です。</span><span class="sxs-lookup"><span data-stu-id="37338-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="37338-181">[AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="37338-181">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="37338-182">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="37338-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="37338-183">hostName</span><span class="sxs-lookup"><span data-stu-id="37338-183">hostName</span></span>|<span data-ttu-id="37338-184">String</span><span class="sxs-lookup"><span data-stu-id="37338-184">String</span></span>|<span data-ttu-id="37338-185">Exchange の場所 (URL)、メール ・ アプリケーションに接続します。</span><span class="sxs-lookup"><span data-stu-id="37338-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="37338-186">[AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="37338-186">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="37338-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="37338-187">requireSsl</span></span>|<span data-ttu-id="37338-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="37338-188">Boolean</span></span>|<span data-ttu-id="37338-189">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="37338-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="37338-190">[AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="37338-190">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="37338-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="37338-191">usernameSource</span></span>|[<span data-ttu-id="37338-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="37338-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="37338-193">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー名の属性です。</span><span class="sxs-lookup"><span data-stu-id="37338-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="37338-194">[AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="37338-194">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="37338-195">可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="37338-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="37338-196">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="37338-196">syncCalendar</span></span>|<span data-ttu-id="37338-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="37338-197">Boolean</span></span>|<span data-ttu-id="37338-198">カレンダーの同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="37338-198">Toggles syncing the calendar.</span></span> <span data-ttu-id="37338-199">場合は、デバイス上の予定表を false に設定がオフになっているとなります。</span><span class="sxs-lookup"><span data-stu-id="37338-199">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="37338-200">syncContacts</span><span class="sxs-lookup"><span data-stu-id="37338-200">syncContacts</span></span>|<span data-ttu-id="37338-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="37338-201">Boolean</span></span>|<span data-ttu-id="37338-202">連絡先の同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="37338-202">Toggles syncing contacts.</span></span> <span data-ttu-id="37338-203">場合は取引先担当者の場合は false に設定は、デバイスの電源が切れます。</span><span class="sxs-lookup"><span data-stu-id="37338-203">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="37338-204">syncTasks</span><span class="sxs-lookup"><span data-stu-id="37338-204">syncTasks</span></span>|<span data-ttu-id="37338-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="37338-205">Boolean</span></span>|<span data-ttu-id="37338-206">タスクの同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="37338-206">Toggles syncing tasks.</span></span> <span data-ttu-id="37338-207">場合はタスクの場合は false に設定は、デバイスの電源が切れます。</span><span class="sxs-lookup"><span data-stu-id="37338-207">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="37338-208">応答</span><span class="sxs-lookup"><span data-stu-id="37338-208">Response</span></span>
<span data-ttu-id="37338-209">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="37338-209">If successful, this method returns a `201 Created` response code and a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37338-210">例</span><span class="sxs-lookup"><span data-stu-id="37338-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="37338-211">要求</span><span class="sxs-lookup"><span data-stu-id="37338-211">Request</span></span>
<span data-ttu-id="37338-212">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="37338-212">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="37338-213">応答</span><span class="sxs-lookup"><span data-stu-id="37338-213">Response</span></span>
<span data-ttu-id="37338-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="37338-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




