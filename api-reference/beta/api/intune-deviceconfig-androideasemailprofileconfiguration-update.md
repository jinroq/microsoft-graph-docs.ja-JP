---
title: androideasemailprofileconfiguration 更新
description: androide asemailprofil/オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 52e9f239daae0f524c9063fea5d2ac7942c1fe3c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158045"
---
# <a name="update-androideasemailprofileconfiguration"></a><span data-ttu-id="6fcf8-103">androideasemailprofileconfiguration 更新</span><span class="sxs-lookup"><span data-stu-id="6fcf8-103">Update androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="6fcf8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fcf8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fcf8-106">[androide asemailprofil/](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-106">Update the properties of a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fcf8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6fcf8-107">Prerequisites</span></span>
<span data-ttu-id="6fcf8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6fcf8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6fcf8-110">Permission type</span></span>|<span data-ttu-id="6fcf8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6fcf8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fcf8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6fcf8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6fcf8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fcf8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6fcf8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6fcf8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fcf8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-115">Not supported.</span></span>|
|<span data-ttu-id="6fcf8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6fcf8-116">Application</span></span>|<span data-ttu-id="6fcf8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fcf8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6fcf8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6fcf8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6fcf8-119">Request headers</span></span>
|<span data-ttu-id="6fcf8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6fcf8-120">Header</span></span>|<span data-ttu-id="6fcf8-121">値</span><span class="sxs-lookup"><span data-stu-id="6fcf8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fcf8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fcf8-122">Authorization</span></span>|<span data-ttu-id="6fcf8-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fcf8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6fcf8-124">Accept</span></span>|<span data-ttu-id="6fcf8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6fcf8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fcf8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6fcf8-126">Request body</span></span>
<span data-ttu-id="6fcf8-127">要求本文で、 [androide asemailprofil/](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) /スキーマオブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-127">In the request body, supply a JSON representation for the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="6fcf8-128">次の表に、 [androide asemailprofilの](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-128">The following table shows the properties that are required when you create the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="6fcf8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6fcf8-129">Property</span></span>|<span data-ttu-id="6fcf8-130">型</span><span class="sxs-lookup"><span data-stu-id="6fcf8-130">Type</span></span>|<span data-ttu-id="6fcf8-131">説明</span><span class="sxs-lookup"><span data-stu-id="6fcf8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fcf8-132">id</span><span class="sxs-lookup"><span data-stu-id="6fcf8-132">id</span></span>|<span data-ttu-id="6fcf8-133">文字列</span><span class="sxs-lookup"><span data-stu-id="6fcf8-133">String</span></span>|<span data-ttu-id="6fcf8-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-134">Key of the entity.</span></span> <span data-ttu-id="6fcf8-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6fcf8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fcf8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fcf8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6fcf8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fcf8-137">DateTimeOffset</span></span>|<span data-ttu-id="6fcf8-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6fcf8-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6fcf8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fcf8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6fcf8-140">roleScopeTagIds</span></span>|<span data-ttu-id="6fcf8-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6fcf8-141">String collection</span></span>|<span data-ttu-id="6fcf8-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6fcf8-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6fcf8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fcf8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6fcf8-144">supportsScopeTags</span></span>|<span data-ttu-id="6fcf8-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fcf8-145">Boolean</span></span>|<span data-ttu-id="6fcf8-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6fcf8-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6fcf8-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6fcf8-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-149">This property is read-only.</span></span> <span data-ttu-id="6fcf8-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6fcf8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fcf8-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6fcf8-151">createdDateTime</span></span>|<span data-ttu-id="6fcf8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fcf8-152">DateTimeOffset</span></span>|<span data-ttu-id="6fcf8-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-153">DateTime the object was created.</span></span> <span data-ttu-id="6fcf8-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6fcf8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fcf8-155">説明</span><span class="sxs-lookup"><span data-stu-id="6fcf8-155">description</span></span>|<span data-ttu-id="6fcf8-156">String</span><span class="sxs-lookup"><span data-stu-id="6fcf8-156">String</span></span>|<span data-ttu-id="6fcf8-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6fcf8-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6fcf8-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fcf8-159">displayName</span><span class="sxs-lookup"><span data-stu-id="6fcf8-159">displayName</span></span>|<span data-ttu-id="6fcf8-160">String</span><span class="sxs-lookup"><span data-stu-id="6fcf8-160">String</span></span>|<span data-ttu-id="6fcf8-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6fcf8-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6fcf8-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fcf8-163">version</span><span class="sxs-lookup"><span data-stu-id="6fcf8-163">version</span></span>|<span data-ttu-id="6fcf8-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6fcf8-164">Int32</span></span>|<span data-ttu-id="6fcf8-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-165">Version of the device configuration.</span></span> <span data-ttu-id="6fcf8-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6fcf8-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fcf8-167">accountName</span><span class="sxs-lookup"><span data-stu-id="6fcf8-167">accountName</span></span>|<span data-ttu-id="6fcf8-168">String</span><span class="sxs-lookup"><span data-stu-id="6fcf8-168">String</span></span>|<span data-ttu-id="6fcf8-169">ユーザーに ea (この) プロファイルの名前として表示される Exchange ActiveSync アカウント名。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-169">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="6fcf8-170">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6fcf8-170">authenticationMethod</span></span>|[<span data-ttu-id="6fcf8-171">easauthenticationmethod</span><span class="sxs-lookup"><span data-stu-id="6fcf8-171">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="6fcf8-172">Exchange ActiveSync の認証方法。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-172">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="6fcf8-173">使用可能な値は、`usernameAndPassword`、`certificate` です。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-173">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="6fcf8-174">synccalendar</span><span class="sxs-lookup"><span data-stu-id="6fcf8-174">syncCalendar</span></span>|<span data-ttu-id="6fcf8-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fcf8-175">Boolean</span></span>|<span data-ttu-id="6fcf8-176">予定表の同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-176">Toggles syncing the calendar.</span></span> <span data-ttu-id="6fcf8-177">false カレンダーに設定すると、デバイスで無効になります。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-177">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="6fcf8-178">synccontacts</span><span class="sxs-lookup"><span data-stu-id="6fcf8-178">syncContacts</span></span>|<span data-ttu-id="6fcf8-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fcf8-179">Boolean</span></span>|<span data-ttu-id="6fcf8-180">連絡先の同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-180">Toggles syncing contacts.</span></span> <span data-ttu-id="6fcf8-181">false に設定すると、デバイスで [連絡先] がオフになります。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-181">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="6fcf8-182">synctasks</span><span class="sxs-lookup"><span data-stu-id="6fcf8-182">syncTasks</span></span>|<span data-ttu-id="6fcf8-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fcf8-183">Boolean</span></span>|<span data-ttu-id="6fcf8-184">タスクの同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-184">Toggles syncing tasks.</span></span> <span data-ttu-id="6fcf8-185">false タスクに設定した場合は、デバイスで無効になります。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-185">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="6fcf8-186">syncnotes</span><span class="sxs-lookup"><span data-stu-id="6fcf8-186">syncNotes</span></span>|<span data-ttu-id="6fcf8-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fcf8-187">Boolean</span></span>|<span data-ttu-id="6fcf8-188">メモの同期を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-188">Toggles syncing notes.</span></span> <span data-ttu-id="6fcf8-189">false に設定すると、デバイスでは、メモがオフになります。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-189">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="6fcf8-190">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="6fcf8-190">durationOfEmailToSync</span></span>|[<span data-ttu-id="6fcf8-191">emailsyncduration</span><span class="sxs-lookup"><span data-stu-id="6fcf8-191">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="6fcf8-192">電子メールを同期する時間の長さ。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-192">Duration of time email should be synced to.</span></span> <span data-ttu-id="6fcf8-193">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-193">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="6fcf8-194">emailaddresssource</span><span class="sxs-lookup"><span data-stu-id="6fcf8-194">emailAddressSource</span></span>|[<span data-ttu-id="6fcf8-195">useremailsource</span><span class="sxs-lookup"><span data-stu-id="6fcf8-195">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="6fcf8-196">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-196">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6fcf8-197">使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-197">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="6fcf8-198">emailsyncschedule</span><span class="sxs-lookup"><span data-stu-id="6fcf8-198">emailSyncSchedule</span></span>|[<span data-ttu-id="6fcf8-199">emailsyncschedule</span><span class="sxs-lookup"><span data-stu-id="6fcf8-199">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="6fcf8-200">電子メール同期スケジュール。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-200">Email sync schedule.</span></span> <span data-ttu-id="6fcf8-201">可能な値は、`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage` です。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-201">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="6fcf8-202">hostName</span><span class="sxs-lookup"><span data-stu-id="6fcf8-202">hostName</span></span>|<span data-ttu-id="6fcf8-203">String</span><span class="sxs-lookup"><span data-stu-id="6fcf8-203">String</span></span>|<span data-ttu-id="6fcf8-204">ネイティブメールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-204">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="6fcf8-205">requireSmime</span><span class="sxs-lookup"><span data-stu-id="6fcf8-205">requireSmime</span></span>|<span data-ttu-id="6fcf8-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fcf8-206">Boolean</span></span>|<span data-ttu-id="6fcf8-207">S/MIME 証明書を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-207">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="6fcf8-208">requireSsl</span><span class="sxs-lookup"><span data-stu-id="6fcf8-208">requireSsl</span></span>|<span data-ttu-id="6fcf8-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fcf8-209">Boolean</span></span>|<span data-ttu-id="6fcf8-210">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-210">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="6fcf8-211">usernameSource</span><span class="sxs-lookup"><span data-stu-id="6fcf8-211">usernameSource</span></span>|[<span data-ttu-id="6fcf8-212">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="6fcf8-212">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="6fcf8-213">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-213">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6fcf8-214">使用可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-214">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="6fcf8-215">userdomainnamesource</span><span class="sxs-lookup"><span data-stu-id="6fcf8-215">userDomainNameSource</span></span>|[<span data-ttu-id="6fcf8-216">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="6fcf8-216">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="6fcf8-217">userdomainname 属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-217">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6fcf8-218">使用可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-218">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="6fcf8-219">customdomainname</span><span class="sxs-lookup"><span data-stu-id="6fcf8-219">customDomainName</span></span>|<span data-ttu-id="6fcf8-220">String</span><span class="sxs-lookup"><span data-stu-id="6fcf8-220">String</span></span>|<span data-ttu-id="6fcf8-221">デバイスにインストールする前に電子メールプロファイルを生成するときに使用するカスタムドメイン名の値。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-221">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="6fcf8-222">応答</span><span class="sxs-lookup"><span data-stu-id="6fcf8-222">Response</span></span>
<span data-ttu-id="6fcf8-223">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androide asemailprofilの](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-223">If successful, this method returns a `200 OK` response code and an updated [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fcf8-224">例</span><span class="sxs-lookup"><span data-stu-id="6fcf8-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fcf8-225">要求</span><span class="sxs-lookup"><span data-stu-id="6fcf8-225">Request</span></span>
<span data-ttu-id="6fcf8-226">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 793

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
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

### <a name="response"></a><span data-ttu-id="6fcf8-227">応答</span><span class="sxs-lookup"><span data-stu-id="6fcf8-227">Response</span></span>
<span data-ttu-id="6fcf8-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6fcf8-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




