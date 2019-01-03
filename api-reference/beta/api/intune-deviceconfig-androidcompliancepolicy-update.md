---
title: Update androidCompliancePolicy
description: androidCompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: cf9ea204b260e53fb762e63b139e57e9efe97662
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315366"
---
# <a name="update-androidcompliancepolicy"></a><span data-ttu-id="26177-103">Update androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="26177-103">Update androidCompliancePolicy</span></span>

> <span data-ttu-id="26177-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="26177-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26177-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26177-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="26177-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="26177-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26177-107">[androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="26177-107">Update the properties of a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="26177-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="26177-108">Prerequisites</span></span>
<span data-ttu-id="26177-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26177-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26177-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="26177-111">Permission type</span></span>|<span data-ttu-id="26177-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="26177-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26177-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="26177-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26177-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26177-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="26177-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="26177-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26177-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26177-116">Not supported.</span></span>|
|<span data-ttu-id="26177-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="26177-117">Application</span></span>|<span data-ttu-id="26177-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26177-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26177-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="26177-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="26177-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26177-120">Request headers</span></span>
|<span data-ttu-id="26177-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26177-121">Header</span></span>|<span data-ttu-id="26177-122">値</span><span class="sxs-lookup"><span data-stu-id="26177-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26177-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="26177-123">Authorization</span></span>|<span data-ttu-id="26177-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="26177-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26177-125">Accept</span><span class="sxs-lookup"><span data-stu-id="26177-125">Accept</span></span>|<span data-ttu-id="26177-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26177-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26177-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="26177-127">Request body</span></span>
<span data-ttu-id="26177-128">要求本文において、[androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) オブジェクト用の JSON 表記を提供します。</span><span class="sxs-lookup"><span data-stu-id="26177-128">In the request body, supply a JSON representation for the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

<span data-ttu-id="26177-129">次の表に、[androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="26177-129">The following table shows the properties that are required when you create the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span></span>

|<span data-ttu-id="26177-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26177-130">Property</span></span>|<span data-ttu-id="26177-131">種類</span><span class="sxs-lookup"><span data-stu-id="26177-131">Type</span></span>|<span data-ttu-id="26177-132">説明</span><span class="sxs-lookup"><span data-stu-id="26177-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26177-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="26177-133">roleScopeTagIds</span></span>|<span data-ttu-id="26177-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="26177-134">String collection</span></span>|<span data-ttu-id="26177-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="26177-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="26177-136">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26177-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26177-137">id</span><span class="sxs-lookup"><span data-stu-id="26177-137">id</span></span>|<span data-ttu-id="26177-138">String</span><span class="sxs-lookup"><span data-stu-id="26177-138">String</span></span>|<span data-ttu-id="26177-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="26177-139">Key of the entity.</span></span> <span data-ttu-id="26177-140">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26177-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26177-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26177-141">createdDateTime</span></span>|<span data-ttu-id="26177-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26177-142">DateTimeOffset</span></span>|<span data-ttu-id="26177-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="26177-143">DateTime the object was created.</span></span> <span data-ttu-id="26177-144">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26177-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26177-145">説明</span><span class="sxs-lookup"><span data-stu-id="26177-145">description</span></span>|<span data-ttu-id="26177-146">String</span><span class="sxs-lookup"><span data-stu-id="26177-146">String</span></span>|<span data-ttu-id="26177-147">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="26177-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="26177-148">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26177-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26177-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26177-149">lastModifiedDateTime</span></span>|<span data-ttu-id="26177-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26177-150">DateTimeOffset</span></span>|<span data-ttu-id="26177-151">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="26177-151">DateTime the object was last modified.</span></span> <span data-ttu-id="26177-152">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26177-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26177-153">displayName</span><span class="sxs-lookup"><span data-stu-id="26177-153">displayName</span></span>|<span data-ttu-id="26177-154">String</span><span class="sxs-lookup"><span data-stu-id="26177-154">String</span></span>|<span data-ttu-id="26177-155">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="26177-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="26177-156">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26177-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26177-157">version</span><span class="sxs-lookup"><span data-stu-id="26177-157">version</span></span>|<span data-ttu-id="26177-158">Int32</span><span class="sxs-lookup"><span data-stu-id="26177-158">Int32</span></span>|<span data-ttu-id="26177-159">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="26177-159">Version of the device configuration.</span></span> <span data-ttu-id="26177-160">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="26177-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26177-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="26177-161">passwordRequired</span></span>|<span data-ttu-id="26177-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="26177-162">Boolean</span></span>|<span data-ttu-id="26177-163">デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="26177-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="26177-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="26177-164">passwordMinimumLength</span></span>|<span data-ttu-id="26177-165">Int32</span><span class="sxs-lookup"><span data-stu-id="26177-165">Int32</span></span>|<span data-ttu-id="26177-166">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="26177-166">Minimum password length.</span></span> <span data-ttu-id="26177-167">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="26177-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="26177-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="26177-168">passwordRequiredType</span></span>|[<span data-ttu-id="26177-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="26177-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="26177-170">パスワード内の文字の種類です。</span><span class="sxs-lookup"><span data-stu-id="26177-170">Type of characters in password.</span></span> <span data-ttu-id="26177-171">可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。</span><span class="sxs-lookup"><span data-stu-id="26177-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="26177-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="26177-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="26177-173">Int32</span><span class="sxs-lookup"><span data-stu-id="26177-173">Int32</span></span>|<span data-ttu-id="26177-174">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="26177-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="26177-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="26177-175">passwordExpirationDays</span></span>|<span data-ttu-id="26177-176">Int32</span><span class="sxs-lookup"><span data-stu-id="26177-176">Int32</span></span>|<span data-ttu-id="26177-177">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="26177-177">Number of days before the password expires.</span></span> <span data-ttu-id="26177-178">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="26177-178">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="26177-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="26177-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="26177-180">Int32</span><span class="sxs-lookup"><span data-stu-id="26177-180">Int32</span></span>|<span data-ttu-id="26177-181">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="26177-181">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="26177-182">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="26177-182">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="26177-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="26177-183">Boolean</span></span>|<span data-ttu-id="26177-184">デバイスが不明なソースからのアプリのインストールを許可しないことを要求します。</span><span class="sxs-lookup"><span data-stu-id="26177-184">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="26177-185">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="26177-185">securityDisableUsbDebugging</span></span>|<span data-ttu-id="26177-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="26177-186">Boolean</span></span>|<span data-ttu-id="26177-187">Android デバイスでの USB デバッグを無効にします。</span><span class="sxs-lookup"><span data-stu-id="26177-187">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="26177-188">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="26177-188">securityRequireVerifyApps</span></span>|<span data-ttu-id="26177-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="26177-189">Boolean</span></span>|<span data-ttu-id="26177-190">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="26177-190">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="26177-191">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="26177-191">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="26177-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="26177-192">Boolean</span></span>|<span data-ttu-id="26177-193">デバイスの脅威保護が有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="26177-193">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="26177-194">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="26177-194">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="26177-195">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="26177-195">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="26177-196">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="26177-196">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="26177-197">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="26177-197">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="26177-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="26177-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="26177-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="26177-199">Boolean</span></span>|<span data-ttu-id="26177-200">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="26177-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="26177-201">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="26177-201">osMinimumVersion</span></span>|<span data-ttu-id="26177-202">String</span><span class="sxs-lookup"><span data-stu-id="26177-202">String</span></span>|<span data-ttu-id="26177-203">Android の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="26177-203">Minimum Android version.</span></span>|
|<span data-ttu-id="26177-204">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="26177-204">osMaximumVersion</span></span>|<span data-ttu-id="26177-205">String</span><span class="sxs-lookup"><span data-stu-id="26177-205">String</span></span>|<span data-ttu-id="26177-206">Android の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="26177-206">Maximum Android version.</span></span>|
|<span data-ttu-id="26177-207">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="26177-207">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="26177-208">String</span><span class="sxs-lookup"><span data-stu-id="26177-208">String</span></span>|<span data-ttu-id="26177-209">Android セキュリティ パッチの最小レベル。</span><span class="sxs-lookup"><span data-stu-id="26177-209">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="26177-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="26177-210">storageRequireEncryption</span></span>|<span data-ttu-id="26177-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="26177-211">Boolean</span></span>|<span data-ttu-id="26177-212">Android デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="26177-212">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="26177-213">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="26177-213">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="26177-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="26177-214">Boolean</span></span>|<span data-ttu-id="26177-215">デバイスが SafetyNet の基本整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="26177-215">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="26177-216">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="26177-216">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="26177-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="26177-217">Boolean</span></span>|<span data-ttu-id="26177-218">デバイスが SafetyNet の認定デバイス チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="26177-218">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="26177-219">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="26177-219">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="26177-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="26177-220">Boolean</span></span>|<span data-ttu-id="26177-221">Google Play 開発者サービスがデバイスにインストールされて有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="26177-221">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="26177-222">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="26177-222">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="26177-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="26177-223">Boolean</span></span>|<span data-ttu-id="26177-224">デバイスに最新のセキュリティ プロバイダーが必要です。</span><span class="sxs-lookup"><span data-stu-id="26177-224">Require the device to have up to date security providers.</span></span> <span data-ttu-id="26177-225">デバイスで Google Play 開発者サービスが有効かつ最新の状態になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="26177-225">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="26177-226">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="26177-226">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="26177-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="26177-227">Boolean</span></span>|<span data-ttu-id="26177-228">デバイスが会社のポータル クライアント アプリのランタイム整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="26177-228">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="26177-229">conditionStatementId</span><span class="sxs-lookup"><span data-stu-id="26177-229">conditionStatementId</span></span>|<span data-ttu-id="26177-230">String</span><span class="sxs-lookup"><span data-stu-id="26177-230">String</span></span>|<span data-ttu-id="26177-231">条件ステートメントの id です。</span><span class="sxs-lookup"><span data-stu-id="26177-231">Condition statement id.</span></span>|
|<span data-ttu-id="26177-232">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="26177-232">restrictedApps</span></span>|<span data-ttu-id="26177-233">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="26177-233">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="26177-234">デバイスには、特定のアプリケーションがインストールされていない必要があります。</span><span class="sxs-lookup"><span data-stu-id="26177-234">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="26177-235">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="26177-235">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="26177-236">応答</span><span class="sxs-lookup"><span data-stu-id="26177-236">Response</span></span>
<span data-ttu-id="26177-237">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="26177-237">If successful, this method returns a `200 OK` response code and an updated [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26177-238">例</span><span class="sxs-lookup"><span data-stu-id="26177-238">Example</span></span>
### <a name="request"></a><span data-ttu-id="26177-239">要求</span><span class="sxs-lookup"><span data-stu-id="26177-239">Request</span></span>
<span data-ttu-id="26177-240">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="26177-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1535

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
  "securityRequireCompanyPortalAppIntegrity": true,
  "conditionStatementId": "Condition Statement Id value",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="26177-241">応答</span><span class="sxs-lookup"><span data-stu-id="26177-241">Response</span></span>
<span data-ttu-id="26177-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="26177-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1705

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "752c820f-820f-752c-0f82-2c750f822c75",
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
  "securityRequireCompanyPortalAppIntegrity": true,
  "conditionStatementId": "Condition Statement Id value",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```




