---
title: AndroidWorkProfileGeneralDeviceConfiguration を更新します。
description: AndroidWorkProfileGeneralDeviceConfiguration オブジェクトのプロパティを更新します。
ms.openlocfilehash: 12584b1569dacb0c3b84862d5f519b40a49ae3e0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023060"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="916ed-103">AndroidWorkProfileGeneralDeviceConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="916ed-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="916ed-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="916ed-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="916ed-105">[AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="916ed-105">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="916ed-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="916ed-106">Prerequisites</span></span>
<span data-ttu-id="916ed-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="916ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="916ed-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="916ed-109">Permission type</span></span>|<span data-ttu-id="916ed-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="916ed-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="916ed-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="916ed-111">Delegated (work or school account)</span></span>|<span data-ttu-id="916ed-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="916ed-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="916ed-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="916ed-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="916ed-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="916ed-114">Not supported.</span></span>|
|<span data-ttu-id="916ed-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="916ed-115">Application</span></span>|<span data-ttu-id="916ed-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="916ed-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="916ed-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="916ed-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="916ed-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="916ed-118">Request headers</span></span>
|<span data-ttu-id="916ed-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="916ed-119">Header</span></span>|<span data-ttu-id="916ed-120">値</span><span class="sxs-lookup"><span data-stu-id="916ed-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="916ed-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="916ed-121">Authorization</span></span>|<span data-ttu-id="916ed-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="916ed-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="916ed-123">Accept</span><span class="sxs-lookup"><span data-stu-id="916ed-123">Accept</span></span>|<span data-ttu-id="916ed-124">application/json</span><span class="sxs-lookup"><span data-stu-id="916ed-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="916ed-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="916ed-125">Request body</span></span>
<span data-ttu-id="916ed-126">要求の本文に[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="916ed-126">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="916ed-127">[AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="916ed-127">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="916ed-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="916ed-128">Property</span></span>|<span data-ttu-id="916ed-129">型</span><span class="sxs-lookup"><span data-stu-id="916ed-129">Type</span></span>|<span data-ttu-id="916ed-130">説明</span><span class="sxs-lookup"><span data-stu-id="916ed-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="916ed-131">id</span><span class="sxs-lookup"><span data-stu-id="916ed-131">id</span></span>|<span data-ttu-id="916ed-132">String</span><span class="sxs-lookup"><span data-stu-id="916ed-132">String</span></span>|<span data-ttu-id="916ed-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="916ed-133">Key of the entity.</span></span> <span data-ttu-id="916ed-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="916ed-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="916ed-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="916ed-135">lastModifiedDateTime</span></span>|<span data-ttu-id="916ed-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="916ed-136">DateTimeOffset</span></span>|<span data-ttu-id="916ed-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="916ed-137">DateTime the object was last modified.</span></span> <span data-ttu-id="916ed-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="916ed-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="916ed-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="916ed-139">createdDateTime</span></span>|<span data-ttu-id="916ed-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="916ed-140">DateTimeOffset</span></span>|<span data-ttu-id="916ed-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="916ed-141">DateTime the object was created.</span></span> <span data-ttu-id="916ed-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="916ed-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="916ed-143">説明</span><span class="sxs-lookup"><span data-stu-id="916ed-143">description</span></span>|<span data-ttu-id="916ed-144">String</span><span class="sxs-lookup"><span data-stu-id="916ed-144">String</span></span>|<span data-ttu-id="916ed-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="916ed-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="916ed-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="916ed-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="916ed-147">displayName</span><span class="sxs-lookup"><span data-stu-id="916ed-147">displayName</span></span>|<span data-ttu-id="916ed-148">String</span><span class="sxs-lookup"><span data-stu-id="916ed-148">String</span></span>|<span data-ttu-id="916ed-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="916ed-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="916ed-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="916ed-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="916ed-151">version</span><span class="sxs-lookup"><span data-stu-id="916ed-151">version</span></span>|<span data-ttu-id="916ed-152">Int32</span><span class="sxs-lookup"><span data-stu-id="916ed-152">Int32</span></span>|<span data-ttu-id="916ed-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="916ed-153">Version of the device configuration.</span></span> <span data-ttu-id="916ed-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="916ed-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="916ed-155">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="916ed-155">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="916ed-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="916ed-156">Boolean</span></span>|<span data-ttu-id="916ed-157">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="916ed-157">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="916ed-158">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="916ed-158">passwordBlockTrustAgents</span></span>|<span data-ttu-id="916ed-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="916ed-159">Boolean</span></span>|<span data-ttu-id="916ed-160">Smart Lock や他の信頼エージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="916ed-160">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="916ed-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="916ed-161">passwordExpirationDays</span></span>|<span data-ttu-id="916ed-162">Int32</span><span class="sxs-lookup"><span data-stu-id="916ed-162">Int32</span></span>|<span data-ttu-id="916ed-163">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="916ed-163">Number of days before the password expires.</span></span> <span data-ttu-id="916ed-164">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="916ed-164">Valid values 1 to 365</span></span>|
|<span data-ttu-id="916ed-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="916ed-165">passwordMinimumLength</span></span>|<span data-ttu-id="916ed-166">Int32</span><span class="sxs-lookup"><span data-stu-id="916ed-166">Int32</span></span>|<span data-ttu-id="916ed-167">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="916ed-167">Minimum length of passwords.</span></span> <span data-ttu-id="916ed-168">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="916ed-168">Valid values 4 to 16</span></span>|
|<span data-ttu-id="916ed-169">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="916ed-169">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="916ed-170">Int32</span><span class="sxs-lookup"><span data-stu-id="916ed-170">Int32</span></span>|<span data-ttu-id="916ed-171">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="916ed-171">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="916ed-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="916ed-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="916ed-173">Int32</span><span class="sxs-lookup"><span data-stu-id="916ed-173">Int32</span></span>|<span data-ttu-id="916ed-174">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="916ed-174">Number of previous passwords to block.</span></span> <span data-ttu-id="916ed-175">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="916ed-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="916ed-176">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="916ed-176">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="916ed-177">Int32</span><span class="sxs-lookup"><span data-stu-id="916ed-177">Int32</span></span>|<span data-ttu-id="916ed-178">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="916ed-178">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="916ed-179">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="916ed-179">Valid values 4 to 11</span></span>|
|<span data-ttu-id="916ed-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="916ed-180">passwordRequiredType</span></span>|[<span data-ttu-id="916ed-181">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="916ed-181">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="916ed-182">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="916ed-182">Type of password that is required.</span></span> <span data-ttu-id="916ed-183">可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="916ed-183">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="916ed-184">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="916ed-184">workProfileDataSharingType</span></span>|[<span data-ttu-id="916ed-185">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="916ed-185">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="916ed-186">共有するデータの種類を許可します。</span><span class="sxs-lookup"><span data-stu-id="916ed-186">Type of data sharing that is allowed.</span></span> <span data-ttu-id="916ed-187">可能な値は、`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions` です。</span><span class="sxs-lookup"><span data-stu-id="916ed-187">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="916ed-188">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="916ed-188">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="916ed-189">ブール値</span><span class="sxs-lookup"><span data-stu-id="916ed-189">Boolean</span></span>|<span data-ttu-id="916ed-190">デバイスがロックされているときに通知をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="916ed-190">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="916ed-191">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="916ed-191">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="916ed-192">ブール値</span><span class="sxs-lookup"><span data-stu-id="916ed-192">Boolean</span></span>|<span data-ttu-id="916ed-193">作業プロファイル内のアカウントを追加または削除したり、ユーザーをブロックします。</span><span class="sxs-lookup"><span data-stu-id="916ed-193">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="916ed-194">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="916ed-194">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="916ed-195">ブール値</span><span class="sxs-lookup"><span data-stu-id="916ed-195">Boolean</span></span>|<span data-ttu-id="916ed-196">企業の連絡先にアクセスするための bluetooth デバイスを使用できます。</span><span class="sxs-lookup"><span data-stu-id="916ed-196">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="916ed-197">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="916ed-197">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="916ed-198">ブール値</span><span class="sxs-lookup"><span data-stu-id="916ed-198">Boolean</span></span>|<span data-ttu-id="916ed-199">作業プロファイルで、画面の取り込みをブロックします。</span><span class="sxs-lookup"><span data-stu-id="916ed-199">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="916ed-200">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="916ed-200">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="916ed-201">ブール値</span><span class="sxs-lookup"><span data-stu-id="916ed-201">Boolean</span></span>|<span data-ttu-id="916ed-202">ブロックでは、作業プロファイル呼び出し元 ID を表示個人プロファイルにします。</span><span class="sxs-lookup"><span data-stu-id="916ed-202">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="916ed-203">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="916ed-203">workProfileBlockCamera</span></span>|<span data-ttu-id="916ed-204">ブール値</span><span class="sxs-lookup"><span data-stu-id="916ed-204">Boolean</span></span>|<span data-ttu-id="916ed-205">ブロック プロファイル カメラが動作します。</span><span class="sxs-lookup"><span data-stu-id="916ed-205">Block work profile camera.</span></span>|
|<span data-ttu-id="916ed-206">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="916ed-206">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="916ed-207">ブール値</span><span class="sxs-lookup"><span data-stu-id="916ed-207">Boolean</span></span>|<span data-ttu-id="916ed-208">個人プロファイルでは、作業プロファイルの連絡先可用性ブロックです。</span><span class="sxs-lookup"><span data-stu-id="916ed-208">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="916ed-209">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="916ed-209">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="916ed-210">ブール値</span><span class="sxs-lookup"><span data-stu-id="916ed-210">Boolean</span></span>|<span data-ttu-id="916ed-211">プロファイルのコピーと貼り付けが有効になっている間の設定を許可しない場合を示すブール値です。</span><span class="sxs-lookup"><span data-stu-id="916ed-211">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="916ed-212">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="916ed-212">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="916ed-213">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="916ed-213">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="916ed-214">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="916ed-214">Type of password that is required.</span></span> <span data-ttu-id="916ed-215">可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="916ed-215">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="916ed-216">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="916ed-216">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="916ed-217">ブール値</span><span class="sxs-lookup"><span data-stu-id="916ed-217">Boolean</span></span>|<span data-ttu-id="916ed-218">指紋をブロックするかどうかを示す作業プロファイルのロックを解除します。</span><span class="sxs-lookup"><span data-stu-id="916ed-218">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="916ed-219">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="916ed-219">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="916ed-220">ブール値</span><span class="sxs-lookup"><span data-stu-id="916ed-220">Boolean</span></span>|<span data-ttu-id="916ed-221">スマート ロックと作業プロファイルを他の信頼のエージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="916ed-221">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="916ed-222">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="916ed-222">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="916ed-223">Int32</span><span class="sxs-lookup"><span data-stu-id="916ed-223">Int32</span></span>|<span data-ttu-id="916ed-224">日前作業プロファイルのパスワードに、の有効期限が切れます。</span><span class="sxs-lookup"><span data-stu-id="916ed-224">Number of days before the work profile password expires.</span></span> <span data-ttu-id="916ed-225">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="916ed-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="916ed-226">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="916ed-226">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="916ed-227">Int32</span><span class="sxs-lookup"><span data-stu-id="916ed-227">Int32</span></span>|<span data-ttu-id="916ed-228">作業プロファイル パスワードの最小長。</span><span class="sxs-lookup"><span data-stu-id="916ed-228">Minimum length of work profile password.</span></span> <span data-ttu-id="916ed-229">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="916ed-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="916ed-230">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="916ed-230">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="916ed-231">Int32</span><span class="sxs-lookup"><span data-stu-id="916ed-231">Int32</span></span>|<span data-ttu-id="916ed-232">プロファイル パスワードの作業に必要な数字の最小数です。</span><span class="sxs-lookup"><span data-stu-id="916ed-232">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="916ed-233">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="916ed-233">Valid values 1 to 10</span></span>|
|<span data-ttu-id="916ed-234">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="916ed-234">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="916ed-235">Int32</span><span class="sxs-lookup"><span data-stu-id="916ed-235">Int32</span></span>|<span data-ttu-id="916ed-236">プロファイル パスワードの作業に必要なアルファベット以外の文字数の最小値です。</span><span class="sxs-lookup"><span data-stu-id="916ed-236">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="916ed-237">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="916ed-237">Valid values 1 to 10</span></span>|
|<span data-ttu-id="916ed-238">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="916ed-238">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="916ed-239">Int32</span><span class="sxs-lookup"><span data-stu-id="916ed-239">Int32</span></span>|<span data-ttu-id="916ed-240">プロファイル パスワードの作業で必要な文字数の最小値。</span><span class="sxs-lookup"><span data-stu-id="916ed-240">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="916ed-241">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="916ed-241">Valid values 1 to 10</span></span>|
|<span data-ttu-id="916ed-242">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="916ed-242">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="916ed-243">Int32</span><span class="sxs-lookup"><span data-stu-id="916ed-243">Int32</span></span>|<span data-ttu-id="916ed-244">作業プロファイルのパスワードに必要な小文字の文字数の最小値です。</span><span class="sxs-lookup"><span data-stu-id="916ed-244">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="916ed-245">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="916ed-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="916ed-246">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="916ed-246">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="916ed-247">Int32</span><span class="sxs-lookup"><span data-stu-id="916ed-247">Int32</span></span>|<span data-ttu-id="916ed-248">プロファイル パスワードの作業に必要な大文字の文字数の最小値。</span><span class="sxs-lookup"><span data-stu-id="916ed-248">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="916ed-249">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="916ed-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="916ed-250">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="916ed-250">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="916ed-251">Int32</span><span class="sxs-lookup"><span data-stu-id="916ed-251">Int32</span></span>|<span data-ttu-id="916ed-252">プロファイル パスワードの作業で必要なシンボル数の最小値です。</span><span class="sxs-lookup"><span data-stu-id="916ed-252">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="916ed-253">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="916ed-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="916ed-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="916ed-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="916ed-255">Int32</span><span class="sxs-lookup"><span data-stu-id="916ed-255">Int32</span></span>|<span data-ttu-id="916ed-256">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="916ed-256">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="916ed-257">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="916ed-257">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="916ed-258">Int32</span><span class="sxs-lookup"><span data-stu-id="916ed-258">Int32</span></span>|<span data-ttu-id="916ed-259">ブロックする前の作業プロファイル パスワードの数です。</span><span class="sxs-lookup"><span data-stu-id="916ed-259">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="916ed-260">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="916ed-260">Valid values 0 to 24</span></span>|
|<span data-ttu-id="916ed-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="916ed-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="916ed-262">Int32</span><span class="sxs-lookup"><span data-stu-id="916ed-262">Int32</span></span>|<span data-ttu-id="916ed-263">作業プロファイルが削除されるまでに許容される障害および削除されたすべての企業データの記号の数です。</span><span class="sxs-lookup"><span data-stu-id="916ed-263">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="916ed-264">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="916ed-264">Valid values 4 to 11</span></span>|
|<span data-ttu-id="916ed-265">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="916ed-265">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="916ed-266">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="916ed-266">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="916ed-267">必要な作業プロファイル パスワードの種類です。</span><span class="sxs-lookup"><span data-stu-id="916ed-267">Type of work profile password that is required.</span></span> <span data-ttu-id="916ed-268">可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="916ed-268">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="916ed-269">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="916ed-269">workProfileRequirePassword</span></span>|<span data-ttu-id="916ed-270">ブール値</span><span class="sxs-lookup"><span data-stu-id="916ed-270">Boolean</span></span>|<span data-ttu-id="916ed-271">パスワードが必要な作業プロファイルを</span><span class="sxs-lookup"><span data-stu-id="916ed-271">Password is required or not for work profile</span></span>|
|<span data-ttu-id="916ed-272">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="916ed-272">securityRequireVerifyApps</span></span>|<span data-ttu-id="916ed-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="916ed-273">Boolean</span></span>|<span data-ttu-id="916ed-274">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="916ed-274">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="916ed-275">応答</span><span class="sxs-lookup"><span data-stu-id="916ed-275">Response</span></span>
<span data-ttu-id="916ed-276">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="916ed-276">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="916ed-277">例</span><span class="sxs-lookup"><span data-stu-id="916ed-277">Example</span></span>
### <a name="request"></a><span data-ttu-id="916ed-278">要求</span><span class="sxs-lookup"><span data-stu-id="916ed-278">Request</span></span>
<span data-ttu-id="916ed-279">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="916ed-279">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="916ed-280">応答</span><span class="sxs-lookup"><span data-stu-id="916ed-280">Response</span></span>
<span data-ttu-id="916ed-p126">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="916ed-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



