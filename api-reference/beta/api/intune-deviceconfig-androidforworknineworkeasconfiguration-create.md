---
title: AndroidForWorkNineWorkEasConfiguration を作成します。
description: 新しい androidForWorkNineWorkEasConfiguration オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: f30d9edc6b86de56b5ab283ac9301fbb199ba454
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310970"
---
# <a name="create-androidforworknineworkeasconfiguration"></a><span data-ttu-id="c2491-103">AndroidForWorkNineWorkEasConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="c2491-103">Create androidForWorkNineWorkEasConfiguration</span></span>

> <span data-ttu-id="c2491-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c2491-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2491-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2491-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2491-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c2491-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2491-107">新しい[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c2491-107">Create a new [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c2491-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c2491-108">Prerequisites</span></span>
<span data-ttu-id="c2491-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2491-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2491-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c2491-111">Permission type</span></span>|<span data-ttu-id="c2491-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c2491-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2491-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c2491-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2491-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2491-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c2491-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c2491-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2491-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2491-116">Not supported.</span></span>|
|<span data-ttu-id="c2491-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c2491-117">Application</span></span>|<span data-ttu-id="c2491-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2491-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2491-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c2491-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c2491-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2491-120">Request headers</span></span>
|<span data-ttu-id="c2491-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2491-121">Header</span></span>|<span data-ttu-id="c2491-122">値</span><span class="sxs-lookup"><span data-stu-id="c2491-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2491-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2491-123">Authorization</span></span>|<span data-ttu-id="c2491-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c2491-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2491-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c2491-125">Accept</span></span>|<span data-ttu-id="c2491-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2491-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2491-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c2491-127">Request body</span></span>
<span data-ttu-id="c2491-128">要求の本文に androidForWorkNineWorkEasConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="c2491-128">In the request body, supply a JSON representation for the androidForWorkNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="c2491-129">次の表は、androidForWorkNineWorkEasConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c2491-129">The following table shows the properties that are required when you create the androidForWorkNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="c2491-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c2491-130">Property</span></span>|<span data-ttu-id="c2491-131">種類</span><span class="sxs-lookup"><span data-stu-id="c2491-131">Type</span></span>|<span data-ttu-id="c2491-132">説明</span><span class="sxs-lookup"><span data-stu-id="c2491-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2491-133">ID</span><span class="sxs-lookup"><span data-stu-id="c2491-133">id</span></span>|<span data-ttu-id="c2491-134">String</span><span class="sxs-lookup"><span data-stu-id="c2491-134">String</span></span>|<span data-ttu-id="c2491-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c2491-135">Key of the entity.</span></span> <span data-ttu-id="c2491-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c2491-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2491-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2491-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c2491-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2491-138">DateTimeOffset</span></span>|<span data-ttu-id="c2491-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c2491-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c2491-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c2491-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2491-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c2491-141">roleScopeTagIds</span></span>|<span data-ttu-id="c2491-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c2491-142">String collection</span></span>|<span data-ttu-id="c2491-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="c2491-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c2491-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c2491-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2491-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c2491-145">supportsScopeTags</span></span>|<span data-ttu-id="c2491-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="c2491-146">Boolean</span></span>|<span data-ttu-id="c2491-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c2491-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c2491-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="c2491-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c2491-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="c2491-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c2491-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="c2491-150">This property is read-only.</span></span> <span data-ttu-id="c2491-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c2491-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2491-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c2491-152">createdDateTime</span></span>|<span data-ttu-id="c2491-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2491-153">DateTimeOffset</span></span>|<span data-ttu-id="c2491-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c2491-154">DateTime the object was created.</span></span> <span data-ttu-id="c2491-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c2491-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2491-156">説明</span><span class="sxs-lookup"><span data-stu-id="c2491-156">description</span></span>|<span data-ttu-id="c2491-157">String</span><span class="sxs-lookup"><span data-stu-id="c2491-157">String</span></span>|<span data-ttu-id="c2491-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="c2491-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c2491-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c2491-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2491-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c2491-160">displayName</span></span>|<span data-ttu-id="c2491-161">String</span><span class="sxs-lookup"><span data-stu-id="c2491-161">String</span></span>|<span data-ttu-id="c2491-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="c2491-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c2491-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c2491-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2491-164">version</span><span class="sxs-lookup"><span data-stu-id="c2491-164">version</span></span>|<span data-ttu-id="c2491-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c2491-165">Int32</span></span>|<span data-ttu-id="c2491-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="c2491-166">Version of the device configuration.</span></span> <span data-ttu-id="c2491-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c2491-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2491-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c2491-168">authenticationMethod</span></span>|[<span data-ttu-id="c2491-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c2491-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="c2491-170">Exchange ActiveSync の認証方法です。</span><span class="sxs-lookup"><span data-stu-id="c2491-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="c2491-171">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="c2491-171">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="c2491-172">使用可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="c2491-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="c2491-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="c2491-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="c2491-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="c2491-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="c2491-175">電子メールの時間の期間に同期する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c2491-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="c2491-176">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="c2491-176">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="c2491-177">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="c2491-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="c2491-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="c2491-178">emailAddressSource</span></span>|[<span data-ttu-id="c2491-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="c2491-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="c2491-180">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたメール属性です。</span><span class="sxs-lookup"><span data-stu-id="c2491-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c2491-181">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="c2491-181">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="c2491-182">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="c2491-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="c2491-183">hostName</span><span class="sxs-lookup"><span data-stu-id="c2491-183">hostName</span></span>|<span data-ttu-id="c2491-184">String</span><span class="sxs-lookup"><span data-stu-id="c2491-184">String</span></span>|<span data-ttu-id="c2491-185">Exchange の場所 (URL)、メール ・ アプリケーションに接続します。</span><span class="sxs-lookup"><span data-stu-id="c2491-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="c2491-186">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="c2491-186">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="c2491-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="c2491-187">requireSsl</span></span>|<span data-ttu-id="c2491-188">ブール型</span><span class="sxs-lookup"><span data-stu-id="c2491-188">Boolean</span></span>|<span data-ttu-id="c2491-189">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c2491-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="c2491-190">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="c2491-190">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="c2491-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="c2491-191">usernameSource</span></span>|[<span data-ttu-id="c2491-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="c2491-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="c2491-193">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー名の属性です。</span><span class="sxs-lookup"><span data-stu-id="c2491-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c2491-194">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="c2491-194">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="c2491-195">可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="c2491-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="c2491-196">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="c2491-196">syncCalendar</span></span>|<span data-ttu-id="c2491-197">ブール型</span><span class="sxs-lookup"><span data-stu-id="c2491-197">Boolean</span></span>|<span data-ttu-id="c2491-198">カレンダーの同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="c2491-198">Toggles syncing the calendar.</span></span> <span data-ttu-id="c2491-199">場合は、デバイス上の予定表を false に設定がオフになっているとなります。</span><span class="sxs-lookup"><span data-stu-id="c2491-199">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="c2491-200">syncContacts</span><span class="sxs-lookup"><span data-stu-id="c2491-200">syncContacts</span></span>|<span data-ttu-id="c2491-201">ブール型</span><span class="sxs-lookup"><span data-stu-id="c2491-201">Boolean</span></span>|<span data-ttu-id="c2491-202">連絡先の同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="c2491-202">Toggles syncing contacts.</span></span> <span data-ttu-id="c2491-203">場合は取引先担当者の場合は false に設定は、デバイスの電源が切れます。</span><span class="sxs-lookup"><span data-stu-id="c2491-203">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="c2491-204">syncTasks</span><span class="sxs-lookup"><span data-stu-id="c2491-204">syncTasks</span></span>|<span data-ttu-id="c2491-205">ブール型</span><span class="sxs-lookup"><span data-stu-id="c2491-205">Boolean</span></span>|<span data-ttu-id="c2491-206">タスクの同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="c2491-206">Toggles syncing tasks.</span></span> <span data-ttu-id="c2491-207">場合はタスクの場合は false に設定は、デバイスの電源が切れます。</span><span class="sxs-lookup"><span data-stu-id="c2491-207">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="c2491-208">応答</span><span class="sxs-lookup"><span data-stu-id="c2491-208">Response</span></span>
<span data-ttu-id="c2491-209">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c2491-209">If successful, this method returns a `201 Created` response code and a [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2491-210">例</span><span class="sxs-lookup"><span data-stu-id="c2491-210">Example</span></span>
### <a name="request"></a><span data-ttu-id="c2491-211">要求</span><span class="sxs-lookup"><span data-stu-id="c2491-211">Request</span></span>
<span data-ttu-id="c2491-212">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c2491-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 630

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
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
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```

### <a name="response"></a><span data-ttu-id="c2491-213">応答</span><span class="sxs-lookup"><span data-stu-id="c2491-213">Response</span></span>
<span data-ttu-id="c2491-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c2491-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




