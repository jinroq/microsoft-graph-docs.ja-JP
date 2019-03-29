---
title: Create sharedPCConfiguration
description: 新しい sharedPCConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 921a7fa12adabe6c71ec3c3e26c626c15d9d4513
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983212"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="b7ab3-103">Create sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="b7ab3-103">Create sharedPCConfiguration</span></span>

> <span data-ttu-id="b7ab3-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7ab3-105">新しい [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-105">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7ab3-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b7ab3-106">Prerequisites</span></span>
<span data-ttu-id="b7ab3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7ab3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b7ab3-109">Permission type</span></span>|<span data-ttu-id="b7ab3-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b7ab3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7ab3-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b7ab3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b7ab3-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7ab3-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b7ab3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b7ab3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7ab3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-114">Not supported.</span></span>|
|<span data-ttu-id="b7ab3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b7ab3-115">Application</span></span>|<span data-ttu-id="b7ab3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7ab3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b7ab3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b7ab3-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7ab3-118">Request headers</span></span>
|<span data-ttu-id="b7ab3-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7ab3-119">Header</span></span>|<span data-ttu-id="b7ab3-120">値</span><span class="sxs-lookup"><span data-stu-id="b7ab3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7ab3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7ab3-121">Authorization</span></span>|<span data-ttu-id="b7ab3-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7ab3-123">承諾</span><span class="sxs-lookup"><span data-stu-id="b7ab3-123">Accept</span></span>|<span data-ttu-id="b7ab3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b7ab3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7ab3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b7ab3-125">Request body</span></span>
<span data-ttu-id="b7ab3-126">要求本文で、sharedPCConfiguration オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-126">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="b7ab3-127">次の表に、sharedPCConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-127">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="b7ab3-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7ab3-128">Property</span></span>|<span data-ttu-id="b7ab3-129">型</span><span class="sxs-lookup"><span data-stu-id="b7ab3-129">Type</span></span>|<span data-ttu-id="b7ab3-130">説明</span><span class="sxs-lookup"><span data-stu-id="b7ab3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7ab3-131">id</span><span class="sxs-lookup"><span data-stu-id="b7ab3-131">id</span></span>|<span data-ttu-id="b7ab3-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b7ab3-132">String</span></span>|<span data-ttu-id="b7ab3-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-133">Key of the entity.</span></span> <span data-ttu-id="b7ab3-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7ab3-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7ab3-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b7ab3-135">lastModifiedDateTime</span></span>|<span data-ttu-id="b7ab3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7ab3-136">DateTimeOffset</span></span>|<span data-ttu-id="b7ab3-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-137">DateTime the object was last modified.</span></span> <span data-ttu-id="b7ab3-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7ab3-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7ab3-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b7ab3-139">createdDateTime</span></span>|<span data-ttu-id="b7ab3-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7ab3-140">DateTimeOffset</span></span>|<span data-ttu-id="b7ab3-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-141">DateTime the object was created.</span></span> <span data-ttu-id="b7ab3-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7ab3-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7ab3-143">description</span><span class="sxs-lookup"><span data-stu-id="b7ab3-143">description</span></span>|<span data-ttu-id="b7ab3-144">String</span><span class="sxs-lookup"><span data-stu-id="b7ab3-144">String</span></span>|<span data-ttu-id="b7ab3-145">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b7ab3-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7ab3-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7ab3-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b7ab3-147">displayName</span></span>|<span data-ttu-id="b7ab3-148">String</span><span class="sxs-lookup"><span data-stu-id="b7ab3-148">String</span></span>|<span data-ttu-id="b7ab3-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b7ab3-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7ab3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7ab3-151">version</span><span class="sxs-lookup"><span data-stu-id="b7ab3-151">version</span></span>|<span data-ttu-id="b7ab3-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b7ab3-152">Int32</span></span>|<span data-ttu-id="b7ab3-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-153">Version of the device configuration.</span></span> <span data-ttu-id="b7ab3-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7ab3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7ab3-155">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="b7ab3-155">accountManagerPolicy</span></span>|[<span data-ttu-id="b7ab3-156">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="b7ab3-156">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="b7ab3-157">共有の PC 上でアカウントを管理する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-157">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="b7ab3-158">disableAccountManager が false の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-158">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="b7ab3-159">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="b7ab3-159">allowedAccounts</span></span>|[<span data-ttu-id="b7ab3-160">sharedpcallowedaccounttype</span><span class="sxs-lookup"><span data-stu-id="b7ab3-160">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="b7ab3-161">共有の PC で使用できるアカウントの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-161">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="b7ab3-162">可能な値は、`guest`、`domain` です。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-162">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="b7ab3-163">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="b7ab3-163">allowLocalStorage</span></span>|<span data-ttu-id="b7ab3-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7ab3-164">Boolean</span></span>|<span data-ttu-id="b7ab3-165">共有の PC でローカル ストレージを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-165">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="b7ab3-166">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="b7ab3-166">disableAccountManager</span></span>|<span data-ttu-id="b7ab3-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7ab3-167">Boolean</span></span>|<span data-ttu-id="b7ab3-168">共有 PC モードのアカウント マネージャーを無効にします。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-168">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="b7ab3-169">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="b7ab3-169">disableEduPolicies</span></span>|<span data-ttu-id="b7ab3-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7ab3-170">Boolean</span></span>|<span data-ttu-id="b7ab3-171">既定の共有 PC 教育環境ポリシーを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-171">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="b7ab3-172">Windows 10 RS2 以降では、このポリシーは Enabled を true に設定しなくても適用されます。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-172">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="b7ab3-173">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="b7ab3-173">disablePowerPolicies</span></span>|<span data-ttu-id="b7ab3-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7ab3-174">Boolean</span></span>|<span data-ttu-id="b7ab3-175">既定の共有 PC 電源ポリシーを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-175">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="b7ab3-176">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="b7ab3-176">disableSignInOnResume</span></span>|<span data-ttu-id="b7ab3-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7ab3-177">Boolean</span></span>|<span data-ttu-id="b7ab3-178">デバイスがスリープ モードから再開するたびにサインインを求める設定を無効にします。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-178">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="b7ab3-179">enabled</span><span class="sxs-lookup"><span data-stu-id="b7ab3-179">enabled</span></span>|<span data-ttu-id="b7ab3-180">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="b7ab3-180">Boolean</span></span>|<span data-ttu-id="b7ab3-181">共有 PC モードを有効にし、共有 PC のポリシーを適用します。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-181">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="b7ab3-182">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="b7ab3-182">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="b7ab3-183">Int32</span><span class="sxs-lookup"><span data-stu-id="b7ab3-183">Int32</span></span>|<span data-ttu-id="b7ab3-184">PC がスリープ状態になるまでにデバイスがアイドル状態を続ける時間を秒単位で指定します。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-184">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="b7ab3-185">この値を 0 に設定すると、スリープ タイムアウトは発生しなくなります。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-185">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="b7ab3-186">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="b7ab3-186">kioskAppDisplayName</span></span>|<span data-ttu-id="b7ab3-187">String</span><span class="sxs-lookup"><span data-stu-id="b7ab3-187">String</span></span>|<span data-ttu-id="b7ab3-188">SetKioskAppUserModelId で指定されたアプリを起動するサインイン画面に表示されるアカウントの表示テキストを指定します。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-188">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="b7ab3-189">KioskAppUserModelId が設定されている場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-189">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="b7ab3-190">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="b7ab3-190">kioskAppUserModelId</span></span>|<span data-ttu-id="b7ab3-191">String</span><span class="sxs-lookup"><span data-stu-id="b7ab3-191">String</span></span>|<span data-ttu-id="b7ab3-192">割り当てられたアクセスで使用するアプリのアプリケーション ユーザー モデル ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-192">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="b7ab3-193">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="b7ab3-193">maintenanceStartTime</span></span>|<span data-ttu-id="b7ab3-194">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b7ab3-194">TimeOfDay</span></span>|<span data-ttu-id="b7ab3-195">毎日のメンテナンス時間の開始時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-195">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="b7ab3-196">応答</span><span class="sxs-lookup"><span data-stu-id="b7ab3-196">Response</span></span>
<span data-ttu-id="b7ab3-197">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-197">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7ab3-198">例</span><span class="sxs-lookup"><span data-stu-id="b7ab3-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7ab3-199">要求</span><span class="sxs-lookup"><span data-stu-id="b7ab3-199">Request</span></span>
<span data-ttu-id="b7ab3-200">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 860

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```

### <a name="response"></a><span data-ttu-id="b7ab3-201">応答</span><span class="sxs-lookup"><span data-stu-id="b7ab3-201">Response</span></span>
<span data-ttu-id="b7ab3-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b7ab3-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1032

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```



