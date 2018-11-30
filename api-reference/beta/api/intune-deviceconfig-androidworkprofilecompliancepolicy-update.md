---
title: AndroidWorkProfileCompliancePolicy を更新します。
description: AndroidWorkProfileCompliancePolicy オブジェクトのプロパティを更新します。
ms.openlocfilehash: c37253c788fdbc7212cbb4ea729b1e4dd45cd6e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070991"
---
# <a name="update-androidworkprofilecompliancepolicy"></a><span data-ttu-id="82882-103">AndroidWorkProfileCompliancePolicy を更新します。</span><span class="sxs-lookup"><span data-stu-id="82882-103">Update androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="82882-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="82882-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82882-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82882-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82882-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="82882-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82882-107">[AndroidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="82882-107">Update the properties of a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="82882-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="82882-108">Prerequisites</span></span>
<span data-ttu-id="82882-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82882-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82882-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="82882-111">Permission type</span></span>|<span data-ttu-id="82882-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="82882-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82882-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="82882-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82882-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82882-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82882-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="82882-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82882-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82882-116">Not supported.</span></span>|
|<span data-ttu-id="82882-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="82882-117">Application</span></span>|<span data-ttu-id="82882-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82882-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82882-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="82882-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="82882-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82882-120">Request headers</span></span>
|<span data-ttu-id="82882-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82882-121">Header</span></span>|<span data-ttu-id="82882-122">値</span><span class="sxs-lookup"><span data-stu-id="82882-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82882-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="82882-123">Authorization</span></span>|<span data-ttu-id="82882-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="82882-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82882-125">Accept</span><span class="sxs-lookup"><span data-stu-id="82882-125">Accept</span></span>|<span data-ttu-id="82882-126">application/json</span><span class="sxs-lookup"><span data-stu-id="82882-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82882-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="82882-127">Request body</span></span>
<span data-ttu-id="82882-128">要求の本文に[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="82882-128">In the request body, supply a JSON representation for the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="82882-129">[AndroidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="82882-129">The following table shows the properties that are required when you create the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md).</span></span>

|<span data-ttu-id="82882-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82882-130">Property</span></span>|<span data-ttu-id="82882-131">型</span><span class="sxs-lookup"><span data-stu-id="82882-131">Type</span></span>|<span data-ttu-id="82882-132">説明</span><span class="sxs-lookup"><span data-stu-id="82882-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82882-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="82882-133">roleScopeTagIds</span></span>|<span data-ttu-id="82882-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="82882-134">String collection</span></span>|<span data-ttu-id="82882-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="82882-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="82882-136">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82882-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="82882-137">id</span><span class="sxs-lookup"><span data-stu-id="82882-137">id</span></span>|<span data-ttu-id="82882-138">String</span><span class="sxs-lookup"><span data-stu-id="82882-138">String</span></span>|<span data-ttu-id="82882-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="82882-139">Key of the entity.</span></span> <span data-ttu-id="82882-140">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82882-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="82882-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82882-141">createdDateTime</span></span>|<span data-ttu-id="82882-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82882-142">DateTimeOffset</span></span>|<span data-ttu-id="82882-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="82882-143">DateTime the object was created.</span></span> <span data-ttu-id="82882-144">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82882-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="82882-145">説明</span><span class="sxs-lookup"><span data-stu-id="82882-145">description</span></span>|<span data-ttu-id="82882-146">String</span><span class="sxs-lookup"><span data-stu-id="82882-146">String</span></span>|<span data-ttu-id="82882-147">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="82882-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="82882-148">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82882-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="82882-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82882-149">lastModifiedDateTime</span></span>|<span data-ttu-id="82882-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82882-150">DateTimeOffset</span></span>|<span data-ttu-id="82882-151">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="82882-151">DateTime the object was last modified.</span></span> <span data-ttu-id="82882-152">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82882-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="82882-153">displayName</span><span class="sxs-lookup"><span data-stu-id="82882-153">displayName</span></span>|<span data-ttu-id="82882-154">String</span><span class="sxs-lookup"><span data-stu-id="82882-154">String</span></span>|<span data-ttu-id="82882-155">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="82882-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="82882-156">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82882-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="82882-157">version</span><span class="sxs-lookup"><span data-stu-id="82882-157">version</span></span>|<span data-ttu-id="82882-158">Int32</span><span class="sxs-lookup"><span data-stu-id="82882-158">Int32</span></span>|<span data-ttu-id="82882-159">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="82882-159">Version of the device configuration.</span></span> <span data-ttu-id="82882-160">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82882-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="82882-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="82882-161">passwordRequired</span></span>|<span data-ttu-id="82882-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="82882-162">Boolean</span></span>|<span data-ttu-id="82882-163">デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="82882-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="82882-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="82882-164">passwordMinimumLength</span></span>|<span data-ttu-id="82882-165">Int32</span><span class="sxs-lookup"><span data-stu-id="82882-165">Int32</span></span>|<span data-ttu-id="82882-166">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="82882-166">Minimum password length.</span></span> <span data-ttu-id="82882-167">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="82882-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="82882-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="82882-168">passwordRequiredType</span></span>|[<span data-ttu-id="82882-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="82882-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="82882-170">パスワード内の文字の種類です。</span><span class="sxs-lookup"><span data-stu-id="82882-170">Type of characters in password.</span></span> <span data-ttu-id="82882-171">可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。</span><span class="sxs-lookup"><span data-stu-id="82882-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="82882-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="82882-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="82882-173">Int32</span><span class="sxs-lookup"><span data-stu-id="82882-173">Int32</span></span>|<span data-ttu-id="82882-174">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="82882-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="82882-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="82882-175">passwordExpirationDays</span></span>|<span data-ttu-id="82882-176">Int32</span><span class="sxs-lookup"><span data-stu-id="82882-176">Int32</span></span>|<span data-ttu-id="82882-177">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="82882-177">Number of days before the password expires.</span></span> <span data-ttu-id="82882-178">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="82882-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="82882-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="82882-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="82882-180">Int32</span><span class="sxs-lookup"><span data-stu-id="82882-180">Int32</span></span>|<span data-ttu-id="82882-181">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="82882-181">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="82882-182">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="82882-182">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="82882-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="82882-183">Boolean</span></span>|<span data-ttu-id="82882-184">デバイスが不明なソースからのアプリのインストールを許可しないことを要求します。</span><span class="sxs-lookup"><span data-stu-id="82882-184">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="82882-185">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="82882-185">securityDisableUsbDebugging</span></span>|<span data-ttu-id="82882-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="82882-186">Boolean</span></span>|<span data-ttu-id="82882-187">Android デバイスでの USB デバッグを無効にします。</span><span class="sxs-lookup"><span data-stu-id="82882-187">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="82882-188">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="82882-188">securityRequireVerifyApps</span></span>|<span data-ttu-id="82882-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="82882-189">Boolean</span></span>|<span data-ttu-id="82882-190">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="82882-190">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="82882-191">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="82882-191">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="82882-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="82882-192">Boolean</span></span>|<span data-ttu-id="82882-193">デバイスの脅威保護が有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="82882-193">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="82882-194">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="82882-194">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="82882-195">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="82882-195">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="82882-196">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="82882-196">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="82882-197">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="82882-197">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="82882-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="82882-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="82882-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="82882-199">Boolean</span></span>|<span data-ttu-id="82882-200">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="82882-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="82882-201">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="82882-201">osMinimumVersion</span></span>|<span data-ttu-id="82882-202">String</span><span class="sxs-lookup"><span data-stu-id="82882-202">String</span></span>|<span data-ttu-id="82882-203">Android の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="82882-203">Minimum Android version.</span></span>|
|<span data-ttu-id="82882-204">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="82882-204">osMaximumVersion</span></span>|<span data-ttu-id="82882-205">String</span><span class="sxs-lookup"><span data-stu-id="82882-205">String</span></span>|<span data-ttu-id="82882-206">Android の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="82882-206">Maximum Android version.</span></span>|
|<span data-ttu-id="82882-207">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="82882-207">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="82882-208">String</span><span class="sxs-lookup"><span data-stu-id="82882-208">String</span></span>|<span data-ttu-id="82882-209">Android セキュリティ パッチの最小レベル。</span><span class="sxs-lookup"><span data-stu-id="82882-209">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="82882-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="82882-210">storageRequireEncryption</span></span>|<span data-ttu-id="82882-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="82882-211">Boolean</span></span>|<span data-ttu-id="82882-212">Android デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="82882-212">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="82882-213">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="82882-213">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="82882-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="82882-214">Boolean</span></span>|<span data-ttu-id="82882-215">デバイスが SafetyNet の基本整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="82882-215">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="82882-216">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="82882-216">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="82882-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="82882-217">Boolean</span></span>|<span data-ttu-id="82882-218">デバイスが SafetyNet の認定デバイス チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="82882-218">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="82882-219">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="82882-219">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="82882-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="82882-220">Boolean</span></span>|<span data-ttu-id="82882-221">Google Play 開発者サービスがデバイスにインストールされて有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="82882-221">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="82882-222">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="82882-222">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="82882-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="82882-223">Boolean</span></span>|<span data-ttu-id="82882-224">デバイスに最新のセキュリティ プロバイダーが必要です。</span><span class="sxs-lookup"><span data-stu-id="82882-224">Require the device to have up to date security providers.</span></span> <span data-ttu-id="82882-225">デバイスで Google Play 開発者サービスが有効かつ最新の状態になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="82882-225">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="82882-226">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="82882-226">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="82882-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="82882-227">Boolean</span></span>|<span data-ttu-id="82882-228">デバイスが会社のポータル クライアント アプリのランタイム整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="82882-228">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="82882-229">応答</span><span class="sxs-lookup"><span data-stu-id="82882-229">Response</span></span>
<span data-ttu-id="82882-230">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="82882-230">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82882-231">例</span><span class="sxs-lookup"><span data-stu-id="82882-231">Example</span></span>
### <a name="request"></a><span data-ttu-id="82882-232">要求</span><span class="sxs-lookup"><span data-stu-id="82882-232">Request</span></span>
<span data-ttu-id="82882-233">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="82882-233">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1223

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```

### <a name="response"></a><span data-ttu-id="82882-234">応答</span><span class="sxs-lookup"><span data-stu-id="82882-234">Response</span></span>
<span data-ttu-id="82882-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="82882-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1404

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "4e385271-5271-4e38-7152-384e7152384e",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```




