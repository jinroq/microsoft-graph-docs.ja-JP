---
title: Windows10EasEmailProfileConfiguration を作成します。
description: 新しい windows10EasEmailProfileConfiguration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6960e145cf5677dc85ae02baed7aec8dae16e773
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411296"
---
# <a name="create-windows10easemailprofileconfiguration"></a><span data-ttu-id="43d54-103">Windows10EasEmailProfileConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="43d54-103">Create windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="43d54-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="43d54-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="43d54-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43d54-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43d54-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="43d54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43d54-107">新しい[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="43d54-107">Create a new [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43d54-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="43d54-108">Prerequisites</span></span>
<span data-ttu-id="43d54-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43d54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="43d54-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="43d54-111">Permission type</span></span>|<span data-ttu-id="43d54-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="43d54-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43d54-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="43d54-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43d54-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43d54-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="43d54-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="43d54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43d54-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43d54-116">Not supported.</span></span>|
|<span data-ttu-id="43d54-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="43d54-117">Application</span></span>|<span data-ttu-id="43d54-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43d54-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43d54-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="43d54-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="43d54-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43d54-120">Request headers</span></span>
|<span data-ttu-id="43d54-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43d54-121">Header</span></span>|<span data-ttu-id="43d54-122">値</span><span class="sxs-lookup"><span data-stu-id="43d54-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43d54-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="43d54-123">Authorization</span></span>|<span data-ttu-id="43d54-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="43d54-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43d54-125">Accept</span><span class="sxs-lookup"><span data-stu-id="43d54-125">Accept</span></span>|<span data-ttu-id="43d54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43d54-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43d54-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="43d54-127">Request body</span></span>
<span data-ttu-id="43d54-128">要求の本文に windows10EasEmailProfileConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="43d54-128">In the request body, supply a JSON representation for the windows10EasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="43d54-129">次の表は、windows10EasEmailProfileConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="43d54-129">The following table shows the properties that are required when you create the windows10EasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="43d54-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43d54-130">Property</span></span>|<span data-ttu-id="43d54-131">型</span><span class="sxs-lookup"><span data-stu-id="43d54-131">Type</span></span>|<span data-ttu-id="43d54-132">説明</span><span class="sxs-lookup"><span data-stu-id="43d54-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43d54-133">id</span><span class="sxs-lookup"><span data-stu-id="43d54-133">id</span></span>|<span data-ttu-id="43d54-134">String</span><span class="sxs-lookup"><span data-stu-id="43d54-134">String</span></span>|<span data-ttu-id="43d54-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="43d54-135">Key of the entity.</span></span> <span data-ttu-id="43d54-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43d54-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43d54-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43d54-137">lastModifiedDateTime</span></span>|<span data-ttu-id="43d54-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43d54-138">DateTimeOffset</span></span>|<span data-ttu-id="43d54-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="43d54-139">DateTime the object was last modified.</span></span> <span data-ttu-id="43d54-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43d54-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43d54-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="43d54-141">roleScopeTagIds</span></span>|<span data-ttu-id="43d54-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="43d54-142">String collection</span></span>|<span data-ttu-id="43d54-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="43d54-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="43d54-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43d54-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43d54-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="43d54-145">supportsScopeTags</span></span>|<span data-ttu-id="43d54-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="43d54-146">Boolean</span></span>|<span data-ttu-id="43d54-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="43d54-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="43d54-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="43d54-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="43d54-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="43d54-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="43d54-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="43d54-150">This property is read-only.</span></span> <span data-ttu-id="43d54-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43d54-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43d54-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43d54-152">createdDateTime</span></span>|<span data-ttu-id="43d54-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43d54-153">DateTimeOffset</span></span>|<span data-ttu-id="43d54-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="43d54-154">DateTime the object was created.</span></span> <span data-ttu-id="43d54-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43d54-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43d54-156">説明</span><span class="sxs-lookup"><span data-stu-id="43d54-156">description</span></span>|<span data-ttu-id="43d54-157">String</span><span class="sxs-lookup"><span data-stu-id="43d54-157">String</span></span>|<span data-ttu-id="43d54-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="43d54-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="43d54-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43d54-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43d54-160">displayName</span><span class="sxs-lookup"><span data-stu-id="43d54-160">displayName</span></span>|<span data-ttu-id="43d54-161">String</span><span class="sxs-lookup"><span data-stu-id="43d54-161">String</span></span>|<span data-ttu-id="43d54-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="43d54-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="43d54-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43d54-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43d54-164">version</span><span class="sxs-lookup"><span data-stu-id="43d54-164">version</span></span>|<span data-ttu-id="43d54-165">Int32</span><span class="sxs-lookup"><span data-stu-id="43d54-165">Int32</span></span>|<span data-ttu-id="43d54-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="43d54-166">Version of the device configuration.</span></span> <span data-ttu-id="43d54-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43d54-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43d54-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="43d54-168">usernameSource</span></span>|[<span data-ttu-id="43d54-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="43d54-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="43d54-170">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー名の属性です。</span><span class="sxs-lookup"><span data-stu-id="43d54-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="43d54-171">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="43d54-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="43d54-172">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="43d54-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="43d54-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="43d54-173">usernameAADSource</span></span>|[<span data-ttu-id="43d54-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="43d54-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="43d54-175">AAD フィールドには、電子メール プロファイルのユーザー名を取得するために使用するの名前です。</span><span class="sxs-lookup"><span data-stu-id="43d54-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="43d54-176">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="43d54-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="43d54-177">可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。</span><span class="sxs-lookup"><span data-stu-id="43d54-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="43d54-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="43d54-178">userDomainNameSource</span></span>|[<span data-ttu-id="43d54-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="43d54-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="43d54-180">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー ドメイン名属性です。</span><span class="sxs-lookup"><span data-stu-id="43d54-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="43d54-181">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="43d54-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="43d54-182">使用可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="43d54-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="43d54-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="43d54-183">customDomainName</span></span>|<span data-ttu-id="43d54-184">String</span><span class="sxs-lookup"><span data-stu-id="43d54-184">String</span></span>|<span data-ttu-id="43d54-185">カスタム ドメイン名の値は、デバイスにインストールする前に、電子メール プロファイルを生成する際に使用します。</span><span class="sxs-lookup"><span data-stu-id="43d54-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="43d54-186">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="43d54-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="43d54-187">accountName</span><span class="sxs-lookup"><span data-stu-id="43d54-187">accountName</span></span>|<span data-ttu-id="43d54-188">String</span><span class="sxs-lookup"><span data-stu-id="43d54-188">String</span></span>|<span data-ttu-id="43d54-189">アカウントの名前です。</span><span class="sxs-lookup"><span data-stu-id="43d54-189">Account name.</span></span>|
|<span data-ttu-id="43d54-190">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="43d54-190">syncCalendar</span></span>|<span data-ttu-id="43d54-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="43d54-191">Boolean</span></span>|<span data-ttu-id="43d54-192">予定表を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="43d54-192">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="43d54-193">syncContacts</span><span class="sxs-lookup"><span data-stu-id="43d54-193">syncContacts</span></span>|<span data-ttu-id="43d54-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="43d54-194">Boolean</span></span>|<span data-ttu-id="43d54-195">連絡先を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="43d54-195">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="43d54-196">syncTasks</span><span class="sxs-lookup"><span data-stu-id="43d54-196">syncTasks</span></span>|<span data-ttu-id="43d54-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="43d54-197">Boolean</span></span>|<span data-ttu-id="43d54-198">タスクを同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="43d54-198">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="43d54-199">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="43d54-199">durationOfEmailToSync</span></span>|[<span data-ttu-id="43d54-200">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="43d54-200">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="43d54-201">同期するメールの期間です。使用可能な値: `userDefined`、 `oneDay`、 `threeDays`、 `oneWeek`、 `twoWeeks`、 `oneMonth`、 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="43d54-201">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="43d54-202">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="43d54-202">emailAddressSource</span></span>|[<span data-ttu-id="43d54-203">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="43d54-203">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="43d54-204">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたメール属性です。</span><span class="sxs-lookup"><span data-stu-id="43d54-204">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="43d54-205">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="43d54-205">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="43d54-206">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="43d54-206">emailSyncSchedule</span></span>|[<span data-ttu-id="43d54-207">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="43d54-207">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="43d54-208">電子メールの同期のスケジュールです。</span><span class="sxs-lookup"><span data-stu-id="43d54-208">Email sync schedule.</span></span> <span data-ttu-id="43d54-209">可能な値は、`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage` です。</span><span class="sxs-lookup"><span data-stu-id="43d54-209">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="43d54-210">hostName</span><span class="sxs-lookup"><span data-stu-id="43d54-210">hostName</span></span>|<span data-ttu-id="43d54-211">String</span><span class="sxs-lookup"><span data-stu-id="43d54-211">String</span></span>|<span data-ttu-id="43d54-212">場所 (URL) の交換、ネイティブのメール アプリケーションに接続します。</span><span class="sxs-lookup"><span data-stu-id="43d54-212">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="43d54-213">requireSsl</span><span class="sxs-lookup"><span data-stu-id="43d54-213">requireSsl</span></span>|<span data-ttu-id="43d54-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="43d54-214">Boolean</span></span>|<span data-ttu-id="43d54-215">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="43d54-215">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="43d54-216">応答</span><span class="sxs-lookup"><span data-stu-id="43d54-216">Response</span></span>
<span data-ttu-id="43d54-217">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="43d54-217">If successful, this method returns a `201 Created` response code and a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43d54-218">例</span><span class="sxs-lookup"><span data-stu-id="43d54-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="43d54-219">要求</span><span class="sxs-lookup"><span data-stu-id="43d54-219">Request</span></span>
<span data-ttu-id="43d54-220">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="43d54-220">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="43d54-221">応答</span><span class="sxs-lookup"><span data-stu-id="43d54-221">Response</span></span>
<span data-ttu-id="43d54-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="43d54-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




