---
title: Windows10EasEmailProfileConfiguration を更新します。
description: Windows10EasEmailProfileConfiguration オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7cbb293477c2cdc3e1b022445daf381202f48d4c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398213"
---
# <a name="update-windows10easemailprofileconfiguration"></a><span data-ttu-id="9b09f-103">Windows10EasEmailProfileConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="9b09f-103">Update windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="9b09f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9b09f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9b09f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b09f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b09f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9b09f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b09f-107">[Windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9b09f-107">Update the properties of a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b09f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9b09f-108">Prerequisites</span></span>
<span data-ttu-id="9b09f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b09f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9b09f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9b09f-111">Permission type</span></span>|<span data-ttu-id="9b09f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9b09f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b09f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9b09f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b09f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b09f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b09f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9b09f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b09f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b09f-116">Not supported.</span></span>|
|<span data-ttu-id="9b09f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9b09f-117">Application</span></span>|<span data-ttu-id="9b09f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b09f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b09f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9b09f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9b09f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b09f-120">Request headers</span></span>
|<span data-ttu-id="9b09f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b09f-121">Header</span></span>|<span data-ttu-id="9b09f-122">値</span><span class="sxs-lookup"><span data-stu-id="9b09f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b09f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b09f-123">Authorization</span></span>|<span data-ttu-id="9b09f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9b09f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b09f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9b09f-125">Accept</span></span>|<span data-ttu-id="9b09f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b09f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b09f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9b09f-127">Request body</span></span>
<span data-ttu-id="9b09f-128">要求の本文に[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="9b09f-128">In the request body, supply a JSON representation for the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="9b09f-129">[Windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="9b09f-129">The following table shows the properties that are required when you create the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="9b09f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b09f-130">Property</span></span>|<span data-ttu-id="9b09f-131">型</span><span class="sxs-lookup"><span data-stu-id="9b09f-131">Type</span></span>|<span data-ttu-id="9b09f-132">説明</span><span class="sxs-lookup"><span data-stu-id="9b09f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b09f-133">id</span><span class="sxs-lookup"><span data-stu-id="9b09f-133">id</span></span>|<span data-ttu-id="9b09f-134">String</span><span class="sxs-lookup"><span data-stu-id="9b09f-134">String</span></span>|<span data-ttu-id="9b09f-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9b09f-135">Key of the entity.</span></span> <span data-ttu-id="9b09f-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b09f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b09f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b09f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9b09f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b09f-138">DateTimeOffset</span></span>|<span data-ttu-id="9b09f-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9b09f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9b09f-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b09f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b09f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9b09f-141">roleScopeTagIds</span></span>|<span data-ttu-id="9b09f-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9b09f-142">String collection</span></span>|<span data-ttu-id="9b09f-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="9b09f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9b09f-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b09f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b09f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9b09f-145">supportsScopeTags</span></span>|<span data-ttu-id="9b09f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b09f-146">Boolean</span></span>|<span data-ttu-id="9b09f-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9b09f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9b09f-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="9b09f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9b09f-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="9b09f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9b09f-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="9b09f-150">This property is read-only.</span></span> <span data-ttu-id="9b09f-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b09f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b09f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b09f-152">createdDateTime</span></span>|<span data-ttu-id="9b09f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b09f-153">DateTimeOffset</span></span>|<span data-ttu-id="9b09f-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9b09f-154">DateTime the object was created.</span></span> <span data-ttu-id="9b09f-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b09f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b09f-156">説明</span><span class="sxs-lookup"><span data-stu-id="9b09f-156">description</span></span>|<span data-ttu-id="9b09f-157">String</span><span class="sxs-lookup"><span data-stu-id="9b09f-157">String</span></span>|<span data-ttu-id="9b09f-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="9b09f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9b09f-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b09f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b09f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="9b09f-160">displayName</span></span>|<span data-ttu-id="9b09f-161">String</span><span class="sxs-lookup"><span data-stu-id="9b09f-161">String</span></span>|<span data-ttu-id="9b09f-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="9b09f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9b09f-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b09f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b09f-164">version</span><span class="sxs-lookup"><span data-stu-id="9b09f-164">version</span></span>|<span data-ttu-id="9b09f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9b09f-165">Int32</span></span>|<span data-ttu-id="9b09f-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9b09f-166">Version of the device configuration.</span></span> <span data-ttu-id="9b09f-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b09f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b09f-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="9b09f-168">usernameSource</span></span>|[<span data-ttu-id="9b09f-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="9b09f-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="9b09f-170">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー名の属性です。</span><span class="sxs-lookup"><span data-stu-id="9b09f-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9b09f-171">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="9b09f-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="9b09f-172">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="9b09f-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="9b09f-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="9b09f-173">usernameAADSource</span></span>|[<span data-ttu-id="9b09f-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="9b09f-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="9b09f-175">AAD フィールドには、電子メール プロファイルのユーザー名を取得するために使用するの名前です。</span><span class="sxs-lookup"><span data-stu-id="9b09f-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="9b09f-176">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="9b09f-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="9b09f-177">可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。</span><span class="sxs-lookup"><span data-stu-id="9b09f-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="9b09f-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="9b09f-178">userDomainNameSource</span></span>|[<span data-ttu-id="9b09f-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="9b09f-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="9b09f-180">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー ドメイン名属性です。</span><span class="sxs-lookup"><span data-stu-id="9b09f-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9b09f-181">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="9b09f-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="9b09f-182">使用可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="9b09f-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="9b09f-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="9b09f-183">customDomainName</span></span>|<span data-ttu-id="9b09f-184">String</span><span class="sxs-lookup"><span data-stu-id="9b09f-184">String</span></span>|<span data-ttu-id="9b09f-185">カスタム ドメイン名の値は、デバイスにインストールする前に、電子メール プロファイルを生成する際に使用します。</span><span class="sxs-lookup"><span data-stu-id="9b09f-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="9b09f-186">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="9b09f-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="9b09f-187">accountName</span><span class="sxs-lookup"><span data-stu-id="9b09f-187">accountName</span></span>|<span data-ttu-id="9b09f-188">String</span><span class="sxs-lookup"><span data-stu-id="9b09f-188">String</span></span>|<span data-ttu-id="9b09f-189">アカウントの名前です。</span><span class="sxs-lookup"><span data-stu-id="9b09f-189">Account name.</span></span>|
|<span data-ttu-id="9b09f-190">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="9b09f-190">syncCalendar</span></span>|<span data-ttu-id="9b09f-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b09f-191">Boolean</span></span>|<span data-ttu-id="9b09f-192">予定表を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9b09f-192">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="9b09f-193">syncContacts</span><span class="sxs-lookup"><span data-stu-id="9b09f-193">syncContacts</span></span>|<span data-ttu-id="9b09f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b09f-194">Boolean</span></span>|<span data-ttu-id="9b09f-195">連絡先を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9b09f-195">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="9b09f-196">syncTasks</span><span class="sxs-lookup"><span data-stu-id="9b09f-196">syncTasks</span></span>|<span data-ttu-id="9b09f-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b09f-197">Boolean</span></span>|<span data-ttu-id="9b09f-198">タスクを同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9b09f-198">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="9b09f-199">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="9b09f-199">durationOfEmailToSync</span></span>|[<span data-ttu-id="9b09f-200">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="9b09f-200">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="9b09f-201">同期するメールの期間です。使用可能な値: `userDefined`、 `oneDay`、 `threeDays`、 `oneWeek`、 `twoWeeks`、 `oneMonth`、 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="9b09f-201">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="9b09f-202">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="9b09f-202">emailAddressSource</span></span>|[<span data-ttu-id="9b09f-203">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="9b09f-203">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="9b09f-204">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたメール属性です。</span><span class="sxs-lookup"><span data-stu-id="9b09f-204">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9b09f-205">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="9b09f-205">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="9b09f-206">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="9b09f-206">emailSyncSchedule</span></span>|[<span data-ttu-id="9b09f-207">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="9b09f-207">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="9b09f-208">電子メールの同期のスケジュールです。</span><span class="sxs-lookup"><span data-stu-id="9b09f-208">Email sync schedule.</span></span> <span data-ttu-id="9b09f-209">可能な値は、`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage` です。</span><span class="sxs-lookup"><span data-stu-id="9b09f-209">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="9b09f-210">hostName</span><span class="sxs-lookup"><span data-stu-id="9b09f-210">hostName</span></span>|<span data-ttu-id="9b09f-211">String</span><span class="sxs-lookup"><span data-stu-id="9b09f-211">String</span></span>|<span data-ttu-id="9b09f-212">場所 (URL) の交換、ネイティブのメール アプリケーションに接続します。</span><span class="sxs-lookup"><span data-stu-id="9b09f-212">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="9b09f-213">requireSsl</span><span class="sxs-lookup"><span data-stu-id="9b09f-213">requireSsl</span></span>|<span data-ttu-id="9b09f-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b09f-214">Boolean</span></span>|<span data-ttu-id="9b09f-215">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9b09f-215">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="9b09f-216">応答</span><span class="sxs-lookup"><span data-stu-id="9b09f-216">Response</span></span>
<span data-ttu-id="9b09f-217">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9b09f-217">If successful, this method returns a `200 OK` response code and an updated [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b09f-218">例</span><span class="sxs-lookup"><span data-stu-id="9b09f-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b09f-219">要求</span><span class="sxs-lookup"><span data-stu-id="9b09f-219">Request</span></span>
<span data-ttu-id="9b09f-220">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9b09f-220">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 753

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSsl": true
}
```

### <a name="response"></a><span data-ttu-id="9b09f-221">応答</span><span class="sxs-lookup"><span data-stu-id="9b09f-221">Response</span></span>
<span data-ttu-id="9b09f-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9b09f-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 925

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
  "id": "9dc6f073-f073-9dc6-73f0-c69d73f0c69d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSsl": true
}
```




