---
title: androidWorkProfileCompliancePolicy の更新
description: androidWorkProfileCompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83e13d2275869cb0ed3d2c0f7358d7e7dfddd25b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982708"
---
# <a name="update-androidworkprofilecompliancepolicy"></a><span data-ttu-id="f9402-103">androidWorkProfileCompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="f9402-103">Update androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="f9402-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f9402-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9402-105">[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f9402-105">Update the properties of a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9402-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f9402-106">Prerequisites</span></span>
<span data-ttu-id="f9402-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9402-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9402-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f9402-109">Permission type</span></span>|<span data-ttu-id="f9402-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f9402-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9402-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f9402-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f9402-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9402-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f9402-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f9402-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9402-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9402-114">Not supported.</span></span>|
|<span data-ttu-id="f9402-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f9402-115">Application</span></span>|<span data-ttu-id="f9402-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9402-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9402-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f9402-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="f9402-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9402-118">Request headers</span></span>
|<span data-ttu-id="f9402-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9402-119">Header</span></span>|<span data-ttu-id="f9402-120">値</span><span class="sxs-lookup"><span data-stu-id="f9402-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9402-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9402-121">Authorization</span></span>|<span data-ttu-id="f9402-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f9402-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9402-123">承諾</span><span class="sxs-lookup"><span data-stu-id="f9402-123">Accept</span></span>|<span data-ttu-id="f9402-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f9402-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9402-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f9402-125">Request body</span></span>
<span data-ttu-id="f9402-126">要求本文で、 [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f9402-126">In the request body, supply a JSON representation for the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="f9402-127">次の表に、 [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f9402-127">The following table shows the properties that are required when you create the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md).</span></span>

|<span data-ttu-id="f9402-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9402-128">Property</span></span>|<span data-ttu-id="f9402-129">型</span><span class="sxs-lookup"><span data-stu-id="f9402-129">Type</span></span>|<span data-ttu-id="f9402-130">説明</span><span class="sxs-lookup"><span data-stu-id="f9402-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9402-131">id</span><span class="sxs-lookup"><span data-stu-id="f9402-131">id</span></span>|<span data-ttu-id="f9402-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f9402-132">String</span></span>|<span data-ttu-id="f9402-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f9402-133">Key of the entity.</span></span> <span data-ttu-id="f9402-134">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f9402-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f9402-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f9402-135">createdDateTime</span></span>|<span data-ttu-id="f9402-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9402-136">DateTimeOffset</span></span>|<span data-ttu-id="f9402-137">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f9402-137">DateTime the object was created.</span></span> <span data-ttu-id="f9402-138">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f9402-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f9402-139">description</span><span class="sxs-lookup"><span data-stu-id="f9402-139">description</span></span>|<span data-ttu-id="f9402-140">String</span><span class="sxs-lookup"><span data-stu-id="f9402-140">String</span></span>|<span data-ttu-id="f9402-141">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="f9402-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f9402-142">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f9402-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f9402-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9402-143">lastModifiedDateTime</span></span>|<span data-ttu-id="f9402-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9402-144">DateTimeOffset</span></span>|<span data-ttu-id="f9402-145">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="f9402-145">DateTime the object was last modified.</span></span> <span data-ttu-id="f9402-146">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f9402-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f9402-147">displayName</span><span class="sxs-lookup"><span data-stu-id="f9402-147">displayName</span></span>|<span data-ttu-id="f9402-148">String</span><span class="sxs-lookup"><span data-stu-id="f9402-148">String</span></span>|<span data-ttu-id="f9402-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="f9402-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f9402-150">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f9402-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f9402-151">version</span><span class="sxs-lookup"><span data-stu-id="f9402-151">version</span></span>|<span data-ttu-id="f9402-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f9402-152">Int32</span></span>|<span data-ttu-id="f9402-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f9402-153">Version of the device configuration.</span></span> <span data-ttu-id="f9402-154">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f9402-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f9402-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f9402-155">passwordRequired</span></span>|<span data-ttu-id="f9402-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9402-156">Boolean</span></span>|<span data-ttu-id="f9402-157">デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="f9402-157">Require a password to unlock device.</span></span>|
|<span data-ttu-id="f9402-158">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f9402-158">passwordMinimumLength</span></span>|<span data-ttu-id="f9402-159">Int32</span><span class="sxs-lookup"><span data-stu-id="f9402-159">Int32</span></span>|<span data-ttu-id="f9402-160">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="f9402-160">Minimum password length.</span></span> <span data-ttu-id="f9402-161">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="f9402-161">Valid values 4 to 16</span></span>|
|<span data-ttu-id="f9402-162">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f9402-162">passwordRequiredType</span></span>|[<span data-ttu-id="f9402-163">androidrequiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="f9402-163">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="f9402-164">パスワードの文字の種類。</span><span class="sxs-lookup"><span data-stu-id="f9402-164">Type of characters in password.</span></span> <span data-ttu-id="f9402-165">可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。</span><span class="sxs-lookup"><span data-stu-id="f9402-165">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="f9402-166">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f9402-166">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f9402-167">Int32</span><span class="sxs-lookup"><span data-stu-id="f9402-167">Int32</span></span>|<span data-ttu-id="f9402-168">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="f9402-168">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="f9402-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f9402-169">passwordExpirationDays</span></span>|<span data-ttu-id="f9402-170">Int32</span><span class="sxs-lookup"><span data-stu-id="f9402-170">Int32</span></span>|<span data-ttu-id="f9402-171">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="f9402-171">Number of days before the password expires.</span></span> <span data-ttu-id="f9402-172">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="f9402-172">Valid values 1 to 365</span></span>|
|<span data-ttu-id="f9402-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f9402-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f9402-174">Int32</span><span class="sxs-lookup"><span data-stu-id="f9402-174">Int32</span></span>|<span data-ttu-id="f9402-175">禁止する、以前のパスワードの数です。</span><span class="sxs-lookup"><span data-stu-id="f9402-175">Number of previous passwords to block.</span></span> <span data-ttu-id="f9402-176">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="f9402-176">Valid values 1 to 24</span></span>|
|<span data-ttu-id="f9402-177">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="f9402-177">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="f9402-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9402-178">Boolean</span></span>|<span data-ttu-id="f9402-179">デバイスが不明なソースからのアプリのインストールを許可しないことを要求します。</span><span class="sxs-lookup"><span data-stu-id="f9402-179">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="f9402-180">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="f9402-180">securityDisableUsbDebugging</span></span>|<span data-ttu-id="f9402-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9402-181">Boolean</span></span>|<span data-ttu-id="f9402-182">Android デバイスでの USB デバッグを無効にします。</span><span class="sxs-lookup"><span data-stu-id="f9402-182">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="f9402-183">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="f9402-183">securityRequireVerifyApps</span></span>|<span data-ttu-id="f9402-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9402-184">Boolean</span></span>|<span data-ttu-id="f9402-185">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="f9402-185">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="f9402-186">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="f9402-186">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="f9402-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9402-187">Boolean</span></span>|<span data-ttu-id="f9402-188">デバイスの脅威保護が有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="f9402-188">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="f9402-189">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="f9402-189">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="f9402-190">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="f9402-190">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="f9402-191">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="f9402-191">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="f9402-192">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="f9402-192">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="f9402-193">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="f9402-193">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="f9402-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9402-194">Boolean</span></span>|<span data-ttu-id="f9402-195">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="f9402-195">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="f9402-196">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f9402-196">osMinimumVersion</span></span>|<span data-ttu-id="f9402-197">String</span><span class="sxs-lookup"><span data-stu-id="f9402-197">String</span></span>|<span data-ttu-id="f9402-198">Android の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="f9402-198">Minimum Android version.</span></span>|
|<span data-ttu-id="f9402-199">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f9402-199">osMaximumVersion</span></span>|<span data-ttu-id="f9402-200">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f9402-200">String</span></span>|<span data-ttu-id="f9402-201">Android の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="f9402-201">Maximum Android version.</span></span>|
|<span data-ttu-id="f9402-202">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="f9402-202">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="f9402-203">String</span><span class="sxs-lookup"><span data-stu-id="f9402-203">String</span></span>|<span data-ttu-id="f9402-204">Android セキュリティ パッチの最小レベル。</span><span class="sxs-lookup"><span data-stu-id="f9402-204">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="f9402-205">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f9402-205">storageRequireEncryption</span></span>|<span data-ttu-id="f9402-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9402-206">Boolean</span></span>|<span data-ttu-id="f9402-207">Android デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="f9402-207">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="f9402-208">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="f9402-208">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="f9402-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9402-209">Boolean</span></span>|<span data-ttu-id="f9402-210">デバイスが SafetyNet の基本整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="f9402-210">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="f9402-211">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="f9402-211">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="f9402-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9402-212">Boolean</span></span>|<span data-ttu-id="f9402-213">デバイスが SafetyNet の認定デバイス チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="f9402-213">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="f9402-214">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="f9402-214">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="f9402-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9402-215">Boolean</span></span>|<span data-ttu-id="f9402-216">Google Play 開発者サービスがデバイスにインストールされて有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="f9402-216">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="f9402-217">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="f9402-217">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="f9402-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9402-218">Boolean</span></span>|<span data-ttu-id="f9402-219">デバイスに最新のセキュリティ プロバイダーが必要です。</span><span class="sxs-lookup"><span data-stu-id="f9402-219">Require the device to have up to date security providers.</span></span> <span data-ttu-id="f9402-220">デバイスで Google Play 開発者サービスが有効かつ最新の状態になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f9402-220">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="f9402-221">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="f9402-221">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="f9402-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9402-222">Boolean</span></span>|<span data-ttu-id="f9402-223">デバイスが会社のポータル クライアント アプリのランタイム整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="f9402-223">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="f9402-224">応答</span><span class="sxs-lookup"><span data-stu-id="f9402-224">Response</span></span>
<span data-ttu-id="f9402-225">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f9402-225">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9402-226">例</span><span class="sxs-lookup"><span data-stu-id="f9402-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9402-227">要求</span><span class="sxs-lookup"><span data-stu-id="f9402-227">Request</span></span>
<span data-ttu-id="f9402-228">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f9402-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1170

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="f9402-229">応答</span><span class="sxs-lookup"><span data-stu-id="f9402-229">Response</span></span>
<span data-ttu-id="f9402-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f9402-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1342

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
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



