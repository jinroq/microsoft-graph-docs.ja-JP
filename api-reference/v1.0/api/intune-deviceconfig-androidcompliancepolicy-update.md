---
title: Update androidCompliancePolicy
description: androidCompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fbd709c0b0111240fd2e6b7f79e2888f3f94dd8e
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262259"
---
# <a name="update-androidcompliancepolicy"></a><span data-ttu-id="089da-103">Update androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="089da-103">Update androidCompliancePolicy</span></span>

> <span data-ttu-id="089da-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="089da-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="089da-105">[androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="089da-105">Update the properties of a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="089da-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="089da-106">Prerequisites</span></span>
<span data-ttu-id="089da-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="089da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="089da-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="089da-109">Permission type</span></span>|<span data-ttu-id="089da-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="089da-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="089da-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="089da-111">Delegated (work or school account)</span></span>|<span data-ttu-id="089da-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="089da-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="089da-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="089da-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="089da-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="089da-114">Not supported.</span></span>|
|<span data-ttu-id="089da-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="089da-115">Application</span></span>|<span data-ttu-id="089da-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="089da-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="089da-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="089da-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="089da-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="089da-118">Request headers</span></span>
|<span data-ttu-id="089da-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="089da-119">Header</span></span>|<span data-ttu-id="089da-120">値</span><span class="sxs-lookup"><span data-stu-id="089da-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="089da-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="089da-121">Authorization</span></span>|<span data-ttu-id="089da-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="089da-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="089da-123">承諾</span><span class="sxs-lookup"><span data-stu-id="089da-123">Accept</span></span>|<span data-ttu-id="089da-124">application/json</span><span class="sxs-lookup"><span data-stu-id="089da-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="089da-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="089da-125">Request body</span></span>
<span data-ttu-id="089da-126">要求本文において、[androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) オブジェクト用の JSON 表記を提供します。</span><span class="sxs-lookup"><span data-stu-id="089da-126">In the request body, supply a JSON representation for the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

<span data-ttu-id="089da-127">次の表に、[androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="089da-127">The following table shows the properties that are required when you create the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span></span>

|<span data-ttu-id="089da-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="089da-128">Property</span></span>|<span data-ttu-id="089da-129">型</span><span class="sxs-lookup"><span data-stu-id="089da-129">Type</span></span>|<span data-ttu-id="089da-130">説明</span><span class="sxs-lookup"><span data-stu-id="089da-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="089da-131">id</span><span class="sxs-lookup"><span data-stu-id="089da-131">id</span></span>|<span data-ttu-id="089da-132">文字列</span><span class="sxs-lookup"><span data-stu-id="089da-132">String</span></span>|<span data-ttu-id="089da-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="089da-133">Key of the entity.</span></span> <span data-ttu-id="089da-134">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="089da-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="089da-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="089da-135">createdDateTime</span></span>|<span data-ttu-id="089da-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="089da-136">DateTimeOffset</span></span>|<span data-ttu-id="089da-137">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="089da-137">DateTime the object was created.</span></span> <span data-ttu-id="089da-138">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="089da-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="089da-139">説明</span><span class="sxs-lookup"><span data-stu-id="089da-139">description</span></span>|<span data-ttu-id="089da-140">文字列</span><span class="sxs-lookup"><span data-stu-id="089da-140">String</span></span>|<span data-ttu-id="089da-141">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="089da-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="089da-142">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="089da-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="089da-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="089da-143">lastModifiedDateTime</span></span>|<span data-ttu-id="089da-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="089da-144">DateTimeOffset</span></span>|<span data-ttu-id="089da-145">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="089da-145">DateTime the object was last modified.</span></span> <span data-ttu-id="089da-146">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="089da-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="089da-147">displayName</span><span class="sxs-lookup"><span data-stu-id="089da-147">displayName</span></span>|<span data-ttu-id="089da-148">String</span><span class="sxs-lookup"><span data-stu-id="089da-148">String</span></span>|<span data-ttu-id="089da-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="089da-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="089da-150">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="089da-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="089da-151">version</span><span class="sxs-lookup"><span data-stu-id="089da-151">version</span></span>|<span data-ttu-id="089da-152">Int32</span><span class="sxs-lookup"><span data-stu-id="089da-152">Int32</span></span>|<span data-ttu-id="089da-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="089da-153">Version of the device configuration.</span></span> <span data-ttu-id="089da-154">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="089da-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="089da-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="089da-155">passwordRequired</span></span>|<span data-ttu-id="089da-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="089da-156">Boolean</span></span>|<span data-ttu-id="089da-157">デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="089da-157">Require a password to unlock device.</span></span>|
|<span data-ttu-id="089da-158">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="089da-158">passwordMinimumLength</span></span>|<span data-ttu-id="089da-159">Int32</span><span class="sxs-lookup"><span data-stu-id="089da-159">Int32</span></span>|<span data-ttu-id="089da-160">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="089da-160">Minimum password length.</span></span> <span data-ttu-id="089da-161">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="089da-161">Valid values 4 to 16</span></span>|
|<span data-ttu-id="089da-162">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="089da-162">passwordRequiredType</span></span>|[<span data-ttu-id="089da-163">androidrequiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="089da-163">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="089da-164">パスワードの文字の種類。</span><span class="sxs-lookup"><span data-stu-id="089da-164">Type of characters in password.</span></span> <span data-ttu-id="089da-165">可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。</span><span class="sxs-lookup"><span data-stu-id="089da-165">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="089da-166">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="089da-166">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="089da-167">Int32</span><span class="sxs-lookup"><span data-stu-id="089da-167">Int32</span></span>|<span data-ttu-id="089da-168">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="089da-168">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="089da-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="089da-169">passwordExpirationDays</span></span>|<span data-ttu-id="089da-170">Int32</span><span class="sxs-lookup"><span data-stu-id="089da-170">Int32</span></span>|<span data-ttu-id="089da-171">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="089da-171">Number of days before the password expires.</span></span> <span data-ttu-id="089da-172">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="089da-172">Valid values 1 to 365</span></span>|
|<span data-ttu-id="089da-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="089da-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="089da-174">Int32</span><span class="sxs-lookup"><span data-stu-id="089da-174">Int32</span></span>|<span data-ttu-id="089da-175">禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="089da-175">Number of previous passwords to block.</span></span> <span data-ttu-id="089da-176">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="089da-176">Valid values 1 to 24</span></span>|
|<span data-ttu-id="089da-177">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="089da-177">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="089da-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="089da-178">Boolean</span></span>|<span data-ttu-id="089da-179">デバイスが不明なソースからのアプリのインストールを許可しないことを要求します。</span><span class="sxs-lookup"><span data-stu-id="089da-179">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="089da-180">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="089da-180">securityDisableUsbDebugging</span></span>|<span data-ttu-id="089da-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="089da-181">Boolean</span></span>|<span data-ttu-id="089da-182">Android デバイスでの USB デバッグを無効にします。</span><span class="sxs-lookup"><span data-stu-id="089da-182">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="089da-183">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="089da-183">securityRequireVerifyApps</span></span>|<span data-ttu-id="089da-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="089da-184">Boolean</span></span>|<span data-ttu-id="089da-185">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="089da-185">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="089da-186">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="089da-186">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="089da-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="089da-187">Boolean</span></span>|<span data-ttu-id="089da-188">デバイスの脅威保護が有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="089da-188">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="089da-189">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="089da-189">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="089da-190">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="089da-190">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="089da-191">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="089da-191">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="089da-192">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="089da-192">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="089da-193">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="089da-193">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="089da-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="089da-194">Boolean</span></span>|<span data-ttu-id="089da-195">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="089da-195">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="089da-196">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="089da-196">osMinimumVersion</span></span>|<span data-ttu-id="089da-197">String</span><span class="sxs-lookup"><span data-stu-id="089da-197">String</span></span>|<span data-ttu-id="089da-198">Android の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="089da-198">Minimum Android version.</span></span>|
|<span data-ttu-id="089da-199">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="089da-199">osMaximumVersion</span></span>|<span data-ttu-id="089da-200">String</span><span class="sxs-lookup"><span data-stu-id="089da-200">String</span></span>|<span data-ttu-id="089da-201">Android の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="089da-201">Maximum Android version.</span></span>|
|<span data-ttu-id="089da-202">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="089da-202">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="089da-203">String</span><span class="sxs-lookup"><span data-stu-id="089da-203">String</span></span>|<span data-ttu-id="089da-204">Android セキュリティ パッチの最小レベル。</span><span class="sxs-lookup"><span data-stu-id="089da-204">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="089da-205">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="089da-205">storageRequireEncryption</span></span>|<span data-ttu-id="089da-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="089da-206">Boolean</span></span>|<span data-ttu-id="089da-207">Android デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="089da-207">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="089da-208">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="089da-208">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="089da-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="089da-209">Boolean</span></span>|<span data-ttu-id="089da-210">デバイスが SafetyNet の基本整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="089da-210">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="089da-211">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="089da-211">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="089da-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="089da-212">Boolean</span></span>|<span data-ttu-id="089da-213">デバイスが SafetyNet の認定デバイス チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="089da-213">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="089da-214">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="089da-214">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="089da-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="089da-215">Boolean</span></span>|<span data-ttu-id="089da-216">Google Play 開発者サービスがデバイスにインストールされて有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="089da-216">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="089da-217">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="089da-217">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="089da-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="089da-218">Boolean</span></span>|<span data-ttu-id="089da-219">デバイスに最新のセキュリティ プロバイダーが必要です。</span><span class="sxs-lookup"><span data-stu-id="089da-219">Require the device to have up to date security providers.</span></span> <span data-ttu-id="089da-220">デバイスで Google Play 開発者サービスが有効かつ最新の状態になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="089da-220">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="089da-221">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="089da-221">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="089da-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="089da-222">Boolean</span></span>|<span data-ttu-id="089da-223">デバイスが会社のポータル クライアント アプリのランタイム整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="089da-223">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="089da-224">応答</span><span class="sxs-lookup"><span data-stu-id="089da-224">Response</span></span>
<span data-ttu-id="089da-225">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="089da-225">If successful, this method returns a `200 OK` response code and an updated [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="089da-226">例</span><span class="sxs-lookup"><span data-stu-id="089da-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="089da-227">要求</span><span class="sxs-lookup"><span data-stu-id="089da-227">Request</span></span>
<span data-ttu-id="089da-228">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="089da-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1159

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="089da-229">応答</span><span class="sxs-lookup"><span data-stu-id="089da-229">Response</span></span>
<span data-ttu-id="089da-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="089da-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1331

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
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
  "securityRequireCompanyPortalAppIntegrity": true
}
```



