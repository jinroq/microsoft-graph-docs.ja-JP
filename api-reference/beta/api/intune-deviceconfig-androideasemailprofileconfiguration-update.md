---
title: AndroidEasEmailProfileConfiguration を更新します。
description: AndroidEasEmailProfileConfiguration オブジェクトのプロパティを更新します。
ms.openlocfilehash: 77087b66a00ab8628ac1558e0c03cd6f7f52f48f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073124"
---
# <a name="update-androideasemailprofileconfiguration"></a><span data-ttu-id="4b215-103">AndroidEasEmailProfileConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="4b215-103">Update androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="4b215-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4b215-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b215-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b215-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b215-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4b215-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b215-107">[AndroidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4b215-107">Update the properties of a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4b215-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4b215-108">Prerequisites</span></span>
<span data-ttu-id="4b215-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4b215-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b215-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4b215-111">Permission type</span></span>|<span data-ttu-id="4b215-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4b215-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b215-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4b215-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b215-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b215-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b215-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4b215-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b215-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b215-116">Not supported.</span></span>|
|<span data-ttu-id="4b215-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4b215-117">Application</span></span>|<span data-ttu-id="4b215-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b215-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b215-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4b215-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4b215-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4b215-120">Request headers</span></span>
|<span data-ttu-id="4b215-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4b215-121">Header</span></span>|<span data-ttu-id="4b215-122">値</span><span class="sxs-lookup"><span data-stu-id="4b215-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b215-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b215-123">Authorization</span></span>|<span data-ttu-id="4b215-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4b215-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b215-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4b215-125">Accept</span></span>|<span data-ttu-id="4b215-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b215-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b215-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4b215-127">Request body</span></span>
<span data-ttu-id="4b215-128">要求の本文に[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="4b215-128">In the request body, supply a JSON representation for the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="4b215-129">[AndroidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="4b215-129">The following table shows the properties that are required when you create the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="4b215-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b215-130">Property</span></span>|<span data-ttu-id="4b215-131">型</span><span class="sxs-lookup"><span data-stu-id="4b215-131">Type</span></span>|<span data-ttu-id="4b215-132">説明</span><span class="sxs-lookup"><span data-stu-id="4b215-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b215-133">id</span><span class="sxs-lookup"><span data-stu-id="4b215-133">id</span></span>|<span data-ttu-id="4b215-134">String</span><span class="sxs-lookup"><span data-stu-id="4b215-134">String</span></span>|<span data-ttu-id="4b215-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4b215-135">Key of the entity.</span></span> <span data-ttu-id="4b215-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4b215-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b215-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b215-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4b215-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b215-138">DateTimeOffset</span></span>|<span data-ttu-id="4b215-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4b215-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4b215-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4b215-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b215-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4b215-141">roleScopeTagIds</span></span>|<span data-ttu-id="4b215-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4b215-142">String collection</span></span>|<span data-ttu-id="4b215-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="4b215-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4b215-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4b215-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b215-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4b215-145">supportsScopeTags</span></span>|<span data-ttu-id="4b215-146">ブール値</span><span class="sxs-lookup"><span data-stu-id="4b215-146">Boolean</span></span>|<span data-ttu-id="4b215-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4b215-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4b215-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="4b215-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4b215-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="4b215-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4b215-150">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="4b215-150">This property is read-only.</span></span> <span data-ttu-id="4b215-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4b215-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b215-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b215-152">createdDateTime</span></span>|<span data-ttu-id="4b215-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b215-153">DateTimeOffset</span></span>|<span data-ttu-id="4b215-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4b215-154">DateTime the object was created.</span></span> <span data-ttu-id="4b215-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4b215-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b215-156">説明</span><span class="sxs-lookup"><span data-stu-id="4b215-156">description</span></span>|<span data-ttu-id="4b215-157">String</span><span class="sxs-lookup"><span data-stu-id="4b215-157">String</span></span>|<span data-ttu-id="4b215-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="4b215-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4b215-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4b215-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b215-160">displayName</span><span class="sxs-lookup"><span data-stu-id="4b215-160">displayName</span></span>|<span data-ttu-id="4b215-161">String</span><span class="sxs-lookup"><span data-stu-id="4b215-161">String</span></span>|<span data-ttu-id="4b215-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="4b215-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4b215-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4b215-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b215-164">version</span><span class="sxs-lookup"><span data-stu-id="4b215-164">version</span></span>|<span data-ttu-id="4b215-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4b215-165">Int32</span></span>|<span data-ttu-id="4b215-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="4b215-166">Version of the device configuration.</span></span> <span data-ttu-id="4b215-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4b215-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b215-168">accountName</span><span class="sxs-lookup"><span data-stu-id="4b215-168">accountName</span></span>|<span data-ttu-id="4b215-169">String</span><span class="sxs-lookup"><span data-stu-id="4b215-169">String</span></span>|<span data-ttu-id="4b215-170">Exchange ActiveSync アカウント名、EA (this) プロファイルの名前としてユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="4b215-170">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="4b215-171">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4b215-171">authenticationMethod</span></span>|[<span data-ttu-id="4b215-172">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4b215-172">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="4b215-173">Exchange ActiveSync の認証方法です。</span><span class="sxs-lookup"><span data-stu-id="4b215-173">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="4b215-174">使用可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="4b215-174">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="4b215-175">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="4b215-175">syncCalendar</span></span>|<span data-ttu-id="4b215-176">ブール値</span><span class="sxs-lookup"><span data-stu-id="4b215-176">Boolean</span></span>|<span data-ttu-id="4b215-177">カレンダーの同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="4b215-177">Toggles syncing the calendar.</span></span> <span data-ttu-id="4b215-178">場合は、デバイスで予定表の場合は false に設定がオフになっているとなります。</span><span class="sxs-lookup"><span data-stu-id="4b215-178">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="4b215-179">syncContacts</span><span class="sxs-lookup"><span data-stu-id="4b215-179">syncContacts</span></span>|<span data-ttu-id="4b215-180">ブール値</span><span class="sxs-lookup"><span data-stu-id="4b215-180">Boolean</span></span>|<span data-ttu-id="4b215-181">連絡先の同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="4b215-181">Toggles syncing contacts.</span></span> <span data-ttu-id="4b215-182">場合は取引先担当者の場合は false に設定は、デバイスの電源が切れます。</span><span class="sxs-lookup"><span data-stu-id="4b215-182">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="4b215-183">syncTasks</span><span class="sxs-lookup"><span data-stu-id="4b215-183">syncTasks</span></span>|<span data-ttu-id="4b215-184">ブール値</span><span class="sxs-lookup"><span data-stu-id="4b215-184">Boolean</span></span>|<span data-ttu-id="4b215-185">タスクの同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="4b215-185">Toggles syncing tasks.</span></span> <span data-ttu-id="4b215-186">場合はタスクの場合は false に設定は、デバイスの電源が切れます。</span><span class="sxs-lookup"><span data-stu-id="4b215-186">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="4b215-187">syncNotes</span><span class="sxs-lookup"><span data-stu-id="4b215-187">syncNotes</span></span>|<span data-ttu-id="4b215-188">ブール値</span><span class="sxs-lookup"><span data-stu-id="4b215-188">Boolean</span></span>|<span data-ttu-id="4b215-189">メモの同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="4b215-189">Toggles syncing notes.</span></span> <span data-ttu-id="4b215-190">場合はメモを false に設定は、デバイスの電源が切れます。</span><span class="sxs-lookup"><span data-stu-id="4b215-190">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="4b215-191">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="4b215-191">durationOfEmailToSync</span></span>|[<span data-ttu-id="4b215-192">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="4b215-192">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="4b215-193">電子メールの時間の期間に同期する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4b215-193">Duration of time email should be synced to.</span></span> <span data-ttu-id="4b215-194">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="4b215-194">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="4b215-195">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="4b215-195">emailAddressSource</span></span>|[<span data-ttu-id="4b215-196">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="4b215-196">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="4b215-197">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたメール属性です。</span><span class="sxs-lookup"><span data-stu-id="4b215-197">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4b215-198">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="4b215-198">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="4b215-199">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="4b215-199">emailSyncSchedule</span></span>|[<span data-ttu-id="4b215-200">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="4b215-200">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="4b215-201">電子メールの同期のスケジュールです。</span><span class="sxs-lookup"><span data-stu-id="4b215-201">Email sync schedule.</span></span> <span data-ttu-id="4b215-202">可能な値は、`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage` です。</span><span class="sxs-lookup"><span data-stu-id="4b215-202">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="4b215-203">hostName</span><span class="sxs-lookup"><span data-stu-id="4b215-203">hostName</span></span>|<span data-ttu-id="4b215-204">String</span><span class="sxs-lookup"><span data-stu-id="4b215-204">String</span></span>|<span data-ttu-id="4b215-205">Exchange の場所 (URL) ネイティブのメール アプリケーションに接続します。</span><span class="sxs-lookup"><span data-stu-id="4b215-205">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="4b215-206">requireSmime</span><span class="sxs-lookup"><span data-stu-id="4b215-206">requireSmime</span></span>|<span data-ttu-id="4b215-207">ブール値</span><span class="sxs-lookup"><span data-stu-id="4b215-207">Boolean</span></span>|<span data-ttu-id="4b215-208">S/MIME 証明書を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4b215-208">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="4b215-209">requireSsl</span><span class="sxs-lookup"><span data-stu-id="4b215-209">requireSsl</span></span>|<span data-ttu-id="4b215-210">ブール値</span><span class="sxs-lookup"><span data-stu-id="4b215-210">Boolean</span></span>|<span data-ttu-id="4b215-211">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4b215-211">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="4b215-212">usernameSource</span><span class="sxs-lookup"><span data-stu-id="4b215-212">usernameSource</span></span>|[<span data-ttu-id="4b215-213">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="4b215-213">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="4b215-214">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー名の属性です。</span><span class="sxs-lookup"><span data-stu-id="4b215-214">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4b215-215">可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="4b215-215">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="4b215-216">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="4b215-216">userDomainNameSource</span></span>|[<span data-ttu-id="4b215-217">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="4b215-217">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="4b215-218">AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー ドメイン名属性です。</span><span class="sxs-lookup"><span data-stu-id="4b215-218">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4b215-219">使用可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="4b215-219">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="4b215-220">customDomainName</span><span class="sxs-lookup"><span data-stu-id="4b215-220">customDomainName</span></span>|<span data-ttu-id="4b215-221">String</span><span class="sxs-lookup"><span data-stu-id="4b215-221">String</span></span>|<span data-ttu-id="4b215-222">カスタム ドメイン名の値は、デバイスにインストールする前に、電子メール プロファイルを生成する際に使用します。</span><span class="sxs-lookup"><span data-stu-id="4b215-222">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="4b215-223">応答</span><span class="sxs-lookup"><span data-stu-id="4b215-223">Response</span></span>
<span data-ttu-id="4b215-224">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4b215-224">If successful, this method returns a `200 OK` response code and an updated [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b215-225">例</span><span class="sxs-lookup"><span data-stu-id="4b215-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="4b215-226">要求</span><span class="sxs-lookup"><span data-stu-id="4b215-226">Request</span></span>
<span data-ttu-id="4b215-227">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4b215-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 783

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value"
}
```

### <a name="response"></a><span data-ttu-id="4b215-228">応答</span><span class="sxs-lookup"><span data-stu-id="4b215-228">Response</span></span>
<span data-ttu-id="4b215-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4b215-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 965

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "id": "ee5e5610-5610-ee5e-1056-5eee10565eee",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value"
}
```





