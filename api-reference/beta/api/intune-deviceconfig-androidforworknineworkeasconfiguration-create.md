---
title: AndroidForWorkNineWorkEasConfiguration を作成します。
description: 新しい androidForWorkNineWorkEasConfiguration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 612e1732db0c1c7b9da83d4e1a0f96f0ed72666a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394475"
---
# <a name="create-androidforworknineworkeasconfiguration"></a><span data-ttu-id="1a164-103">AndroidForWorkNineWorkEasConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="1a164-103">Create androidForWorkNineWorkEasConfiguration</span></span>

> <span data-ttu-id="1a164-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1a164-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1a164-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a164-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a164-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1a164-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a164-107">新しい[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1a164-107">Create a new [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a164-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1a164-108">Prerequisites</span></span>
<span data-ttu-id="1a164-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a164-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1a164-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a164-111">Permission type</span></span>|<span data-ttu-id="1a164-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a164-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a164-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a164-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a164-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a164-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1a164-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a164-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a164-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a164-116">Not supported.</span></span>|
|<span data-ttu-id="1a164-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a164-117">Application</span></span>|<span data-ttu-id="1a164-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a164-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a164-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a164-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1a164-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a164-120">Request headers</span></span>
|<span data-ttu-id="1a164-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a164-121">Header</span></span>|<span data-ttu-id="1a164-122">値</span><span class="sxs-lookup"><span data-stu-id="1a164-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a164-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a164-123">Authorization</span></span>|<span data-ttu-id="1a164-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1a164-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a164-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1a164-125">Accept</span></span>|<span data-ttu-id="1a164-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a164-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a164-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a164-127">Request body</span></span>
<span data-ttu-id="1a164-128">要求の本文に androidForWorkNineWorkEasConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="1a164-128">In the request body, supply a JSON representation for the androidForWorkNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="1a164-129">次の表は、androidForWorkNineWorkEasConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1a164-129">The following table shows the properties that are required when you create the androidForWorkNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="1a164-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a164-130">Property</span></span>|<span data-ttu-id="1a164-131">型</span><span class="sxs-lookup"><span data-stu-id="1a164-131">Type</span></span>|<span data-ttu-id="1a164-132">説明</span><span class="sxs-lookup"><span data-stu-id="1a164-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a164-133">id</span><span class="sxs-lookup"><span data-stu-id="1a164-133">id</span></span>|<span data-ttu-id="1a164-134">String</span><span class="sxs-lookup"><span data-stu-id="1a164-134">String</span></span>|<span data-ttu-id="1a164-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1a164-135">Key of the entity.</span></span> <span data-ttu-id="1a164-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a164-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a164-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a164-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1a164-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a164-138">DateTimeOffset</span></span>|<span data-ttu-id="1a164-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1a164-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1a164-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a164-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a164-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1a164-141">roleScopeTagIds</span></span>|<span data-ttu-id="1a164-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1a164-142">String collection</span></span>|<span data-ttu-id="1a164-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="1a164-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1a164-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a164-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a164-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1a164-145">supportsScopeTags</span></span>|<span data-ttu-id="1a164-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a164-146">Boolean</span></span>|<span data-ttu-id="1a164-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1a164-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1a164-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="1a164-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1a164-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="1a164-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1a164-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="1a164-150">This property is read-only.</span></span> <span data-ttu-id="1a164-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a164-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a164-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a164-152">createdDateTime</span></span>|<span data-ttu-id="1a164-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a164-153">DateTimeOffset</span></span>|<span data-ttu-id="1a164-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1a164-154">DateTime the object was created.</span></span> <span data-ttu-id="1a164-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a164-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a164-156">説明</span><span class="sxs-lookup"><span data-stu-id="1a164-156">description</span></span>|<span data-ttu-id="1a164-157">String</span><span class="sxs-lookup"><span data-stu-id="1a164-157">String</span></span>|<span data-ttu-id="1a164-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="1a164-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1a164-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a164-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a164-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1a164-160">displayName</span></span>|<span data-ttu-id="1a164-161">String</span><span class="sxs-lookup"><span data-stu-id="1a164-161">String</span></span>|<span data-ttu-id="1a164-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="1a164-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1a164-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a164-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a164-164">version</span><span class="sxs-lookup"><span data-stu-id="1a164-164">version</span></span>|<span data-ttu-id="1a164-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1a164-165">Int32</span></span>|<span data-ttu-id="1a164-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1a164-166">Version of the device configuration.</span></span> <span data-ttu-id="1a164-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a164-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a164-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1a164-168">authenticationMethod</span></span>|[<span data-ttu-id="1a164-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1a164-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="1a164-170">Exchange ActiveSync の認証方法です。</span><span class="sxs-lookup"><span data-stu-id="1a164-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="1a164-171">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1a164-171">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="1a164-172">使用可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="1a164-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="1a164-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="1a164-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="1a164-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="1a164-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="1a164-175">電子メールの時間の期間に同期する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1a164-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="1a164-176">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1a164-176">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="1a164-177">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="1a164-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="1a164-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="1a164-178">emailAddressSource</span></span>|[<span data-ttu-id="1a164-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="1a164-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="1a164-180">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたメール属性です。</span><span class="sxs-lookup"><span data-stu-id="1a164-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="1a164-181">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1a164-181">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="1a164-182">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="1a164-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="1a164-183">hostName</span><span class="sxs-lookup"><span data-stu-id="1a164-183">hostName</span></span>|<span data-ttu-id="1a164-184">String</span><span class="sxs-lookup"><span data-stu-id="1a164-184">String</span></span>|<span data-ttu-id="1a164-185">Exchange の場所 (URL)、メール ・ アプリケーションに接続します。</span><span class="sxs-lookup"><span data-stu-id="1a164-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="1a164-186">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="1a164-186">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="1a164-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="1a164-187">requireSsl</span></span>|<span data-ttu-id="1a164-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a164-188">Boolean</span></span>|<span data-ttu-id="1a164-189">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1a164-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="1a164-190">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="1a164-190">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="1a164-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="1a164-191">usernameSource</span></span>|[<span data-ttu-id="1a164-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="1a164-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="1a164-193">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー名の属性です。</span><span class="sxs-lookup"><span data-stu-id="1a164-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="1a164-194">[AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1a164-194">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="1a164-195">可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="1a164-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="1a164-196">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="1a164-196">syncCalendar</span></span>|<span data-ttu-id="1a164-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a164-197">Boolean</span></span>|<span data-ttu-id="1a164-198">カレンダーの同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="1a164-198">Toggles syncing the calendar.</span></span> <span data-ttu-id="1a164-199">場合は、デバイス上の予定表を false に設定がオフになっているとなります。</span><span class="sxs-lookup"><span data-stu-id="1a164-199">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="1a164-200">syncContacts</span><span class="sxs-lookup"><span data-stu-id="1a164-200">syncContacts</span></span>|<span data-ttu-id="1a164-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a164-201">Boolean</span></span>|<span data-ttu-id="1a164-202">連絡先の同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="1a164-202">Toggles syncing contacts.</span></span> <span data-ttu-id="1a164-203">場合は取引先担当者の場合は false に設定は、デバイスの電源が切れます。</span><span class="sxs-lookup"><span data-stu-id="1a164-203">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="1a164-204">syncTasks</span><span class="sxs-lookup"><span data-stu-id="1a164-204">syncTasks</span></span>|<span data-ttu-id="1a164-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a164-205">Boolean</span></span>|<span data-ttu-id="1a164-206">タスクの同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="1a164-206">Toggles syncing tasks.</span></span> <span data-ttu-id="1a164-207">場合はタスクの場合は false に設定は、デバイスの電源が切れます。</span><span class="sxs-lookup"><span data-stu-id="1a164-207">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="1a164-208">応答</span><span class="sxs-lookup"><span data-stu-id="1a164-208">Response</span></span>
<span data-ttu-id="1a164-209">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1a164-209">If successful, this method returns a `201 Created` response code and a [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a164-210">例</span><span class="sxs-lookup"><span data-stu-id="1a164-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a164-211">要求</span><span class="sxs-lookup"><span data-stu-id="1a164-211">Request</span></span>
<span data-ttu-id="1a164-212">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1a164-212">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1a164-213">応答</span><span class="sxs-lookup"><span data-stu-id="1a164-213">Response</span></span>
<span data-ttu-id="1a164-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1a164-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




