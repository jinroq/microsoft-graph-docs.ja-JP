---
title: AndroidWorkProfileNineWorkEasConfiguration を作成します。
description: 新しい androidWorkProfileNineWorkEasConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a399aa12dcd5304e667d955a6a3208fd0b68484b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929691"
---
# <a name="create-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="7351f-103">AndroidWorkProfileNineWorkEasConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="7351f-103">Create androidWorkProfileNineWorkEasConfiguration</span></span>

> <span data-ttu-id="7351f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7351f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7351f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7351f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7351f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7351f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7351f-107">新しい[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7351f-107">Create a new [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7351f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7351f-108">Prerequisites</span></span>
<span data-ttu-id="7351f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7351f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7351f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7351f-111">Permission type</span></span>|<span data-ttu-id="7351f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7351f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7351f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7351f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7351f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7351f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7351f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7351f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7351f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7351f-116">Not supported.</span></span>|
|<span data-ttu-id="7351f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7351f-117">Application</span></span>|<span data-ttu-id="7351f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7351f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7351f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7351f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7351f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7351f-120">Request headers</span></span>
|<span data-ttu-id="7351f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7351f-121">Header</span></span>|<span data-ttu-id="7351f-122">値</span><span class="sxs-lookup"><span data-stu-id="7351f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7351f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7351f-123">Authorization</span></span>|<span data-ttu-id="7351f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7351f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7351f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7351f-125">Accept</span></span>|<span data-ttu-id="7351f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7351f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7351f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7351f-127">Request body</span></span>
<span data-ttu-id="7351f-128">要求の本文に androidWorkProfileNineWorkEasConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="7351f-128">In the request body, supply a JSON representation for the androidWorkProfileNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="7351f-129">次の表は、androidWorkProfileNineWorkEasConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7351f-129">The following table shows the properties that are required when you create the androidWorkProfileNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="7351f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7351f-130">Property</span></span>|<span data-ttu-id="7351f-131">型</span><span class="sxs-lookup"><span data-stu-id="7351f-131">Type</span></span>|<span data-ttu-id="7351f-132">説明</span><span class="sxs-lookup"><span data-stu-id="7351f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7351f-133">ID</span><span class="sxs-lookup"><span data-stu-id="7351f-133">id</span></span>|<span data-ttu-id="7351f-134">String</span><span class="sxs-lookup"><span data-stu-id="7351f-134">String</span></span>|<span data-ttu-id="7351f-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7351f-135">Key of the entity.</span></span> <span data-ttu-id="7351f-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7351f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7351f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7351f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7351f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7351f-138">DateTimeOffset</span></span>|<span data-ttu-id="7351f-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7351f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7351f-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7351f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7351f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7351f-141">roleScopeTagIds</span></span>|<span data-ttu-id="7351f-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7351f-142">String collection</span></span>|<span data-ttu-id="7351f-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="7351f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7351f-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7351f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7351f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7351f-145">supportsScopeTags</span></span>|<span data-ttu-id="7351f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="7351f-146">Boolean</span></span>|<span data-ttu-id="7351f-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7351f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7351f-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="7351f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7351f-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="7351f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7351f-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="7351f-150">This property is read-only.</span></span> <span data-ttu-id="7351f-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7351f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7351f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7351f-152">createdDateTime</span></span>|<span data-ttu-id="7351f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7351f-153">DateTimeOffset</span></span>|<span data-ttu-id="7351f-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7351f-154">DateTime the object was created.</span></span> <span data-ttu-id="7351f-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7351f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7351f-156">説明</span><span class="sxs-lookup"><span data-stu-id="7351f-156">description</span></span>|<span data-ttu-id="7351f-157">String</span><span class="sxs-lookup"><span data-stu-id="7351f-157">String</span></span>|<span data-ttu-id="7351f-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="7351f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7351f-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7351f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7351f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="7351f-160">displayName</span></span>|<span data-ttu-id="7351f-161">String</span><span class="sxs-lookup"><span data-stu-id="7351f-161">String</span></span>|<span data-ttu-id="7351f-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="7351f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7351f-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7351f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7351f-164">version</span><span class="sxs-lookup"><span data-stu-id="7351f-164">version</span></span>|<span data-ttu-id="7351f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7351f-165">Int32</span></span>|<span data-ttu-id="7351f-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7351f-166">Version of the device configuration.</span></span> <span data-ttu-id="7351f-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7351f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7351f-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7351f-168">authenticationMethod</span></span>|[<span data-ttu-id="7351f-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7351f-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="7351f-170">Exchange ActiveSync の認証方法です。</span><span class="sxs-lookup"><span data-stu-id="7351f-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="7351f-171">[AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="7351f-171">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="7351f-172">使用可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="7351f-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="7351f-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="7351f-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="7351f-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="7351f-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="7351f-175">電子メールの時間の期間に同期する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7351f-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="7351f-176">[AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="7351f-176">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="7351f-177">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="7351f-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="7351f-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="7351f-178">emailAddressSource</span></span>|[<span data-ttu-id="7351f-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="7351f-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="7351f-180">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたメール属性です。</span><span class="sxs-lookup"><span data-stu-id="7351f-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7351f-181">[AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="7351f-181">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="7351f-182">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="7351f-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7351f-183">hostName</span><span class="sxs-lookup"><span data-stu-id="7351f-183">hostName</span></span>|<span data-ttu-id="7351f-184">String</span><span class="sxs-lookup"><span data-stu-id="7351f-184">String</span></span>|<span data-ttu-id="7351f-185">Exchange の場所 (URL)、メール ・ アプリケーションに接続します。</span><span class="sxs-lookup"><span data-stu-id="7351f-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="7351f-186">[AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="7351f-186">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="7351f-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="7351f-187">requireSsl</span></span>|<span data-ttu-id="7351f-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="7351f-188">Boolean</span></span>|<span data-ttu-id="7351f-189">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7351f-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="7351f-190">[AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="7351f-190">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="7351f-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="7351f-191">usernameSource</span></span>|[<span data-ttu-id="7351f-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="7351f-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="7351f-193">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー名の属性です。</span><span class="sxs-lookup"><span data-stu-id="7351f-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7351f-194">[AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="7351f-194">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="7351f-195">可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="7351f-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7351f-196">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="7351f-196">syncCalendar</span></span>|<span data-ttu-id="7351f-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="7351f-197">Boolean</span></span>|<span data-ttu-id="7351f-198">カレンダーの同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="7351f-198">Toggles syncing the calendar.</span></span> <span data-ttu-id="7351f-199">場合は、デバイス上の予定表を false に設定がオフになっているとなります。</span><span class="sxs-lookup"><span data-stu-id="7351f-199">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="7351f-200">syncContacts</span><span class="sxs-lookup"><span data-stu-id="7351f-200">syncContacts</span></span>|<span data-ttu-id="7351f-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="7351f-201">Boolean</span></span>|<span data-ttu-id="7351f-202">連絡先の同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="7351f-202">Toggles syncing contacts.</span></span> <span data-ttu-id="7351f-203">場合は取引先担当者の場合は false に設定は、デバイスの電源が切れます。</span><span class="sxs-lookup"><span data-stu-id="7351f-203">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="7351f-204">syncTasks</span><span class="sxs-lookup"><span data-stu-id="7351f-204">syncTasks</span></span>|<span data-ttu-id="7351f-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="7351f-205">Boolean</span></span>|<span data-ttu-id="7351f-206">タスクの同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="7351f-206">Toggles syncing tasks.</span></span> <span data-ttu-id="7351f-207">場合はタスクの場合は false に設定は、デバイスの電源が切れます。</span><span class="sxs-lookup"><span data-stu-id="7351f-207">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="7351f-208">応答</span><span class="sxs-lookup"><span data-stu-id="7351f-208">Response</span></span>
<span data-ttu-id="7351f-209">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7351f-209">If successful, this method returns a `201 Created` response code and a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7351f-210">例</span><span class="sxs-lookup"><span data-stu-id="7351f-210">Example</span></span>
### <a name="request"></a><span data-ttu-id="7351f-211">要求</span><span class="sxs-lookup"><span data-stu-id="7351f-211">Request</span></span>
<span data-ttu-id="7351f-212">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7351f-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 634

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="7351f-213">応答</span><span class="sxs-lookup"><span data-stu-id="7351f-213">Response</span></span>
<span data-ttu-id="7351f-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7351f-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





