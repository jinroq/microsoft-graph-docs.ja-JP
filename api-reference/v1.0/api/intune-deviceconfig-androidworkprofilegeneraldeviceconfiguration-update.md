---
title: AndroidWorkProfileGeneralDeviceConfiguration を更新します。
description: AndroidWorkProfileGeneralDeviceConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 7eb65cdcfeebc4ee10edde68fa952e5555861502
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305972"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="aee75-103">AndroidWorkProfileGeneralDeviceConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="aee75-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="aee75-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="aee75-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aee75-105">[AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="aee75-105">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aee75-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="aee75-106">Prerequisites</span></span>
<span data-ttu-id="aee75-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aee75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aee75-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aee75-109">Permission type</span></span>|<span data-ttu-id="aee75-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="aee75-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aee75-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aee75-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aee75-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aee75-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aee75-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aee75-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aee75-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aee75-114">Not supported.</span></span>|
|<span data-ttu-id="aee75-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aee75-115">Application</span></span>|<span data-ttu-id="aee75-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aee75-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aee75-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aee75-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="aee75-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aee75-118">Request headers</span></span>
|<span data-ttu-id="aee75-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aee75-119">Header</span></span>|<span data-ttu-id="aee75-120">値</span><span class="sxs-lookup"><span data-stu-id="aee75-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aee75-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aee75-121">Authorization</span></span>|<span data-ttu-id="aee75-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="aee75-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aee75-123">Accept</span><span class="sxs-lookup"><span data-stu-id="aee75-123">Accept</span></span>|<span data-ttu-id="aee75-124">application/json</span><span class="sxs-lookup"><span data-stu-id="aee75-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aee75-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="aee75-125">Request body</span></span>
<span data-ttu-id="aee75-126">要求の本文に[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="aee75-126">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="aee75-127">[AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="aee75-127">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="aee75-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aee75-128">Property</span></span>|<span data-ttu-id="aee75-129">種類</span><span class="sxs-lookup"><span data-stu-id="aee75-129">Type</span></span>|<span data-ttu-id="aee75-130">説明</span><span class="sxs-lookup"><span data-stu-id="aee75-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aee75-131">ID</span><span class="sxs-lookup"><span data-stu-id="aee75-131">id</span></span>|<span data-ttu-id="aee75-132">String</span><span class="sxs-lookup"><span data-stu-id="aee75-132">String</span></span>|<span data-ttu-id="aee75-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="aee75-133">Key of the entity.</span></span> <span data-ttu-id="aee75-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="aee75-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee75-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aee75-135">lastModifiedDateTime</span></span>|<span data-ttu-id="aee75-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aee75-136">DateTimeOffset</span></span>|<span data-ttu-id="aee75-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="aee75-137">DateTime the object was last modified.</span></span> <span data-ttu-id="aee75-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="aee75-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee75-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aee75-139">createdDateTime</span></span>|<span data-ttu-id="aee75-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aee75-140">DateTimeOffset</span></span>|<span data-ttu-id="aee75-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="aee75-141">DateTime the object was created.</span></span> <span data-ttu-id="aee75-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="aee75-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee75-143">説明</span><span class="sxs-lookup"><span data-stu-id="aee75-143">description</span></span>|<span data-ttu-id="aee75-144">String</span><span class="sxs-lookup"><span data-stu-id="aee75-144">String</span></span>|<span data-ttu-id="aee75-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="aee75-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aee75-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="aee75-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee75-147">displayName</span><span class="sxs-lookup"><span data-stu-id="aee75-147">displayName</span></span>|<span data-ttu-id="aee75-148">String</span><span class="sxs-lookup"><span data-stu-id="aee75-148">String</span></span>|<span data-ttu-id="aee75-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="aee75-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aee75-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="aee75-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee75-151">version</span><span class="sxs-lookup"><span data-stu-id="aee75-151">version</span></span>|<span data-ttu-id="aee75-152">Int32</span><span class="sxs-lookup"><span data-stu-id="aee75-152">Int32</span></span>|<span data-ttu-id="aee75-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="aee75-153">Version of the device configuration.</span></span> <span data-ttu-id="aee75-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="aee75-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee75-155">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="aee75-155">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="aee75-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="aee75-156">Boolean</span></span>|<span data-ttu-id="aee75-157">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="aee75-157">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="aee75-158">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="aee75-158">passwordBlockTrustAgents</span></span>|<span data-ttu-id="aee75-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="aee75-159">Boolean</span></span>|<span data-ttu-id="aee75-160">Smart Lock や他の信頼エージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="aee75-160">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="aee75-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="aee75-161">passwordExpirationDays</span></span>|<span data-ttu-id="aee75-162">Int32</span><span class="sxs-lookup"><span data-stu-id="aee75-162">Int32</span></span>|<span data-ttu-id="aee75-163">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="aee75-163">Number of days before the password expires.</span></span> <span data-ttu-id="aee75-164">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="aee75-164">Valid values 1 to 365</span></span>|
|<span data-ttu-id="aee75-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="aee75-165">passwordMinimumLength</span></span>|<span data-ttu-id="aee75-166">Int32</span><span class="sxs-lookup"><span data-stu-id="aee75-166">Int32</span></span>|<span data-ttu-id="aee75-167">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="aee75-167">Minimum length of passwords.</span></span> <span data-ttu-id="aee75-168">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="aee75-168">Valid values 4 to 16</span></span>|
|<span data-ttu-id="aee75-169">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="aee75-169">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="aee75-170">Int32</span><span class="sxs-lookup"><span data-stu-id="aee75-170">Int32</span></span>|<span data-ttu-id="aee75-171">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="aee75-171">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="aee75-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="aee75-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="aee75-173">Int32</span><span class="sxs-lookup"><span data-stu-id="aee75-173">Int32</span></span>|<span data-ttu-id="aee75-174">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="aee75-174">Number of previous passwords to block.</span></span> <span data-ttu-id="aee75-175">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="aee75-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="aee75-176">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="aee75-176">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="aee75-177">Int32</span><span class="sxs-lookup"><span data-stu-id="aee75-177">Int32</span></span>|<span data-ttu-id="aee75-178">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="aee75-178">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="aee75-179">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="aee75-179">Valid values 4 to 11</span></span>|
|<span data-ttu-id="aee75-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="aee75-180">passwordRequiredType</span></span>|[<span data-ttu-id="aee75-181">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="aee75-181">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="aee75-182">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="aee75-182">Type of password that is required.</span></span> <span data-ttu-id="aee75-183">可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="aee75-183">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="aee75-184">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="aee75-184">workProfileDataSharingType</span></span>|[<span data-ttu-id="aee75-185">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="aee75-185">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="aee75-186">共有するデータの種類を許可します。</span><span class="sxs-lookup"><span data-stu-id="aee75-186">Type of data sharing that is allowed.</span></span> <span data-ttu-id="aee75-187">可能な値は、`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions` です。</span><span class="sxs-lookup"><span data-stu-id="aee75-187">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="aee75-188">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="aee75-188">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="aee75-189">ブール型</span><span class="sxs-lookup"><span data-stu-id="aee75-189">Boolean</span></span>|<span data-ttu-id="aee75-190">デバイスがロックされているときに通知をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="aee75-190">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="aee75-191">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="aee75-191">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="aee75-192">ブール型</span><span class="sxs-lookup"><span data-stu-id="aee75-192">Boolean</span></span>|<span data-ttu-id="aee75-193">作業プロファイル内のアカウントを追加または削除したり、ユーザーをブロックします。</span><span class="sxs-lookup"><span data-stu-id="aee75-193">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="aee75-194">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="aee75-194">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="aee75-195">ブール型</span><span class="sxs-lookup"><span data-stu-id="aee75-195">Boolean</span></span>|<span data-ttu-id="aee75-196">企業の連絡先にアクセスするための bluetooth デバイスを使用できます。</span><span class="sxs-lookup"><span data-stu-id="aee75-196">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="aee75-197">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="aee75-197">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="aee75-198">ブール型</span><span class="sxs-lookup"><span data-stu-id="aee75-198">Boolean</span></span>|<span data-ttu-id="aee75-199">作業プロファイルで、画面の取り込みをブロックします。</span><span class="sxs-lookup"><span data-stu-id="aee75-199">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="aee75-200">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="aee75-200">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="aee75-201">ブール型</span><span class="sxs-lookup"><span data-stu-id="aee75-201">Boolean</span></span>|<span data-ttu-id="aee75-202">ブロックでは、作業プロファイル呼び出し元 ID を表示個人プロファイルにします。</span><span class="sxs-lookup"><span data-stu-id="aee75-202">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="aee75-203">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="aee75-203">workProfileBlockCamera</span></span>|<span data-ttu-id="aee75-204">ブール型</span><span class="sxs-lookup"><span data-stu-id="aee75-204">Boolean</span></span>|<span data-ttu-id="aee75-205">ブロック プロファイル カメラが動作します。</span><span class="sxs-lookup"><span data-stu-id="aee75-205">Block work profile camera.</span></span>|
|<span data-ttu-id="aee75-206">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="aee75-206">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="aee75-207">ブール型</span><span class="sxs-lookup"><span data-stu-id="aee75-207">Boolean</span></span>|<span data-ttu-id="aee75-208">個人プロファイルでは、作業プロファイルの連絡先可用性ブロックです。</span><span class="sxs-lookup"><span data-stu-id="aee75-208">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="aee75-209">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="aee75-209">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="aee75-210">ブール型</span><span class="sxs-lookup"><span data-stu-id="aee75-210">Boolean</span></span>|<span data-ttu-id="aee75-211">プロファイルのコピーと貼り付けが有効になっている間の設定を許可しない場合を示すブール値です。</span><span class="sxs-lookup"><span data-stu-id="aee75-211">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="aee75-212">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="aee75-212">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="aee75-213">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="aee75-213">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="aee75-214">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="aee75-214">Type of password that is required.</span></span> <span data-ttu-id="aee75-215">可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="aee75-215">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="aee75-216">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="aee75-216">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="aee75-217">ブール型</span><span class="sxs-lookup"><span data-stu-id="aee75-217">Boolean</span></span>|<span data-ttu-id="aee75-218">指紋をブロックするかどうかを示す作業プロファイルのロックを解除します。</span><span class="sxs-lookup"><span data-stu-id="aee75-218">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="aee75-219">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="aee75-219">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="aee75-220">ブール型</span><span class="sxs-lookup"><span data-stu-id="aee75-220">Boolean</span></span>|<span data-ttu-id="aee75-221">スマート ロックと作業プロファイルを他の信頼のエージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="aee75-221">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="aee75-222">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="aee75-222">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="aee75-223">Int32</span><span class="sxs-lookup"><span data-stu-id="aee75-223">Int32</span></span>|<span data-ttu-id="aee75-224">日前作業プロファイルのパスワードに、の有効期限が切れます。</span><span class="sxs-lookup"><span data-stu-id="aee75-224">Number of days before the work profile password expires.</span></span> <span data-ttu-id="aee75-225">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="aee75-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="aee75-226">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="aee75-226">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="aee75-227">Int32</span><span class="sxs-lookup"><span data-stu-id="aee75-227">Int32</span></span>|<span data-ttu-id="aee75-228">作業プロファイル パスワードの最小長。</span><span class="sxs-lookup"><span data-stu-id="aee75-228">Minimum length of work profile password.</span></span> <span data-ttu-id="aee75-229">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="aee75-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="aee75-230">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="aee75-230">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="aee75-231">Int32</span><span class="sxs-lookup"><span data-stu-id="aee75-231">Int32</span></span>|<span data-ttu-id="aee75-232">プロファイル パスワードの作業に必要な数字の最小数です。</span><span class="sxs-lookup"><span data-stu-id="aee75-232">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="aee75-233">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="aee75-233">Valid values 1 to 10</span></span>|
|<span data-ttu-id="aee75-234">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="aee75-234">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="aee75-235">Int32</span><span class="sxs-lookup"><span data-stu-id="aee75-235">Int32</span></span>|<span data-ttu-id="aee75-236">プロファイル パスワードの作業に必要なアルファベット以外の文字数の最小値です。</span><span class="sxs-lookup"><span data-stu-id="aee75-236">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="aee75-237">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="aee75-237">Valid values 1 to 10</span></span>|
|<span data-ttu-id="aee75-238">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="aee75-238">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="aee75-239">Int32</span><span class="sxs-lookup"><span data-stu-id="aee75-239">Int32</span></span>|<span data-ttu-id="aee75-240">プロファイル パスワードの作業で必要な文字数の最小値。</span><span class="sxs-lookup"><span data-stu-id="aee75-240">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="aee75-241">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="aee75-241">Valid values 1 to 10</span></span>|
|<span data-ttu-id="aee75-242">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="aee75-242">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="aee75-243">Int32</span><span class="sxs-lookup"><span data-stu-id="aee75-243">Int32</span></span>|<span data-ttu-id="aee75-244">作業プロファイルのパスワードに必要な小文字の文字数の最小値です。</span><span class="sxs-lookup"><span data-stu-id="aee75-244">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="aee75-245">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="aee75-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="aee75-246">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="aee75-246">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="aee75-247">Int32</span><span class="sxs-lookup"><span data-stu-id="aee75-247">Int32</span></span>|<span data-ttu-id="aee75-248">プロファイル パスワードの作業に必要な大文字の文字数の最小値。</span><span class="sxs-lookup"><span data-stu-id="aee75-248">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="aee75-249">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="aee75-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="aee75-250">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="aee75-250">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="aee75-251">Int32</span><span class="sxs-lookup"><span data-stu-id="aee75-251">Int32</span></span>|<span data-ttu-id="aee75-252">プロファイル パスワードの作業で必要なシンボル数の最小値です。</span><span class="sxs-lookup"><span data-stu-id="aee75-252">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="aee75-253">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="aee75-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="aee75-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="aee75-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="aee75-255">Int32</span><span class="sxs-lookup"><span data-stu-id="aee75-255">Int32</span></span>|<span data-ttu-id="aee75-256">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="aee75-256">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="aee75-257">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="aee75-257">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="aee75-258">Int32</span><span class="sxs-lookup"><span data-stu-id="aee75-258">Int32</span></span>|<span data-ttu-id="aee75-259">ブロックする前の作業プロファイル パスワードの数です。</span><span class="sxs-lookup"><span data-stu-id="aee75-259">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="aee75-260">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="aee75-260">Valid values 0 to 24</span></span>|
|<span data-ttu-id="aee75-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="aee75-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="aee75-262">Int32</span><span class="sxs-lookup"><span data-stu-id="aee75-262">Int32</span></span>|<span data-ttu-id="aee75-263">作業プロファイルが削除されるまでに許容される障害および削除されたすべての企業データの記号の数です。</span><span class="sxs-lookup"><span data-stu-id="aee75-263">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="aee75-264">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="aee75-264">Valid values 4 to 11</span></span>|
|<span data-ttu-id="aee75-265">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="aee75-265">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="aee75-266">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="aee75-266">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="aee75-267">必要な作業プロファイル パスワードの種類です。</span><span class="sxs-lookup"><span data-stu-id="aee75-267">Type of work profile password that is required.</span></span> <span data-ttu-id="aee75-268">可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="aee75-268">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="aee75-269">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="aee75-269">workProfileRequirePassword</span></span>|<span data-ttu-id="aee75-270">ブール型</span><span class="sxs-lookup"><span data-stu-id="aee75-270">Boolean</span></span>|<span data-ttu-id="aee75-271">パスワードが必要な作業プロファイルを</span><span class="sxs-lookup"><span data-stu-id="aee75-271">Password is required or not for work profile</span></span>|
|<span data-ttu-id="aee75-272">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="aee75-272">securityRequireVerifyApps</span></span>|<span data-ttu-id="aee75-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="aee75-273">Boolean</span></span>|<span data-ttu-id="aee75-274">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="aee75-274">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="aee75-275">応答</span><span class="sxs-lookup"><span data-stu-id="aee75-275">Response</span></span>
<span data-ttu-id="aee75-276">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="aee75-276">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aee75-277">例</span><span class="sxs-lookup"><span data-stu-id="aee75-277">Example</span></span>
### <a name="request"></a><span data-ttu-id="aee75-278">要求</span><span class="sxs-lookup"><span data-stu-id="aee75-278">Request</span></span>
<span data-ttu-id="aee75-279">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aee75-279">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1831

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="aee75-280">応答</span><span class="sxs-lookup"><span data-stu-id="aee75-280">Response</span></span>
<span data-ttu-id="aee75-p126">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aee75-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2003

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```



