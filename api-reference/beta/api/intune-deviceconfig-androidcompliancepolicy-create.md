---
title: androidCompliancePolicy の作成
description: 新しい androidCompliancePolicy オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8762ff323b94480d41ae27b1b5e2bd747b0e0894
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35958306"
---
# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="96874-103">androidCompliancePolicy の作成</span><span class="sxs-lookup"><span data-stu-id="96874-103">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="96874-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96874-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96874-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="96874-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96874-106">新しい [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="96874-106">Create a new [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96874-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="96874-107">Prerequisites</span></span>
<span data-ttu-id="96874-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="96874-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96874-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="96874-110">Permission type</span></span>|<span data-ttu-id="96874-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="96874-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96874-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="96874-112">Delegated (work or school account)</span></span>|<span data-ttu-id="96874-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96874-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="96874-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="96874-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96874-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96874-115">Not supported.</span></span>|
|<span data-ttu-id="96874-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="96874-116">Application</span></span>|<span data-ttu-id="96874-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96874-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96874-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="96874-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="96874-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96874-119">Request headers</span></span>
|<span data-ttu-id="96874-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96874-120">Header</span></span>|<span data-ttu-id="96874-121">値</span><span class="sxs-lookup"><span data-stu-id="96874-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96874-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="96874-122">Authorization</span></span>|<span data-ttu-id="96874-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="96874-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96874-124">承諾</span><span class="sxs-lookup"><span data-stu-id="96874-124">Accept</span></span>|<span data-ttu-id="96874-125">application/json</span><span class="sxs-lookup"><span data-stu-id="96874-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96874-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="96874-126">Request body</span></span>
<span data-ttu-id="96874-127">要求本文において、androidCompliancePolicy オブジェクトの JSON 表記を提供します。</span><span class="sxs-lookup"><span data-stu-id="96874-127">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="96874-128">次の表に、androidCompliancePolicy 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="96874-128">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="96874-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96874-129">Property</span></span>|<span data-ttu-id="96874-130">型</span><span class="sxs-lookup"><span data-stu-id="96874-130">Type</span></span>|<span data-ttu-id="96874-131">説明</span><span class="sxs-lookup"><span data-stu-id="96874-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96874-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="96874-132">roleScopeTagIds</span></span>|<span data-ttu-id="96874-133">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="96874-133">String collection</span></span>|<span data-ttu-id="96874-134">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="96874-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="96874-135">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96874-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96874-136">id</span><span class="sxs-lookup"><span data-stu-id="96874-136">id</span></span>|<span data-ttu-id="96874-137">文字列</span><span class="sxs-lookup"><span data-stu-id="96874-137">String</span></span>|<span data-ttu-id="96874-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="96874-138">Key of the entity.</span></span> <span data-ttu-id="96874-139">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96874-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96874-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96874-140">createdDateTime</span></span>|<span data-ttu-id="96874-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96874-141">DateTimeOffset</span></span>|<span data-ttu-id="96874-142">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="96874-142">DateTime the object was created.</span></span> <span data-ttu-id="96874-143">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96874-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96874-144">description</span><span class="sxs-lookup"><span data-stu-id="96874-144">description</span></span>|<span data-ttu-id="96874-145">String</span><span class="sxs-lookup"><span data-stu-id="96874-145">String</span></span>|<span data-ttu-id="96874-146">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="96874-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="96874-147">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96874-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96874-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96874-148">lastModifiedDateTime</span></span>|<span data-ttu-id="96874-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96874-149">DateTimeOffset</span></span>|<span data-ttu-id="96874-150">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="96874-150">DateTime the object was last modified.</span></span> <span data-ttu-id="96874-151">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96874-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96874-152">displayName</span><span class="sxs-lookup"><span data-stu-id="96874-152">displayName</span></span>|<span data-ttu-id="96874-153">String</span><span class="sxs-lookup"><span data-stu-id="96874-153">String</span></span>|<span data-ttu-id="96874-154">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="96874-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="96874-155">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96874-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96874-156">version</span><span class="sxs-lookup"><span data-stu-id="96874-156">version</span></span>|<span data-ttu-id="96874-157">Int32</span><span class="sxs-lookup"><span data-stu-id="96874-157">Int32</span></span>|<span data-ttu-id="96874-158">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="96874-158">Version of the device configuration.</span></span> <span data-ttu-id="96874-159">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96874-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96874-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="96874-160">passwordRequired</span></span>|<span data-ttu-id="96874-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="96874-161">Boolean</span></span>|<span data-ttu-id="96874-162">デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="96874-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="96874-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="96874-163">passwordMinimumLength</span></span>|<span data-ttu-id="96874-164">Int32</span><span class="sxs-lookup"><span data-stu-id="96874-164">Int32</span></span>|<span data-ttu-id="96874-165">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="96874-165">Minimum password length.</span></span> <span data-ttu-id="96874-166">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="96874-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="96874-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="96874-167">passwordRequiredType</span></span>|[<span data-ttu-id="96874-168">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="96874-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="96874-169">パスワードの文字の種類。</span><span class="sxs-lookup"><span data-stu-id="96874-169">Type of characters in password.</span></span> <span data-ttu-id="96874-170">可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。</span><span class="sxs-lookup"><span data-stu-id="96874-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="96874-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="96874-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="96874-172">Int32</span><span class="sxs-lookup"><span data-stu-id="96874-172">Int32</span></span>|<span data-ttu-id="96874-173">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="96874-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="96874-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="96874-174">passwordExpirationDays</span></span>|<span data-ttu-id="96874-175">Int32</span><span class="sxs-lookup"><span data-stu-id="96874-175">Int32</span></span>|<span data-ttu-id="96874-176">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="96874-176">Number of days before the password expires.</span></span> <span data-ttu-id="96874-177">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="96874-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="96874-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="96874-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="96874-179">Int32</span><span class="sxs-lookup"><span data-stu-id="96874-179">Int32</span></span>|<span data-ttu-id="96874-180">禁止する、以前のパスワードの数です。</span><span class="sxs-lookup"><span data-stu-id="96874-180">Number of previous passwords to block.</span></span> <span data-ttu-id="96874-181">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="96874-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="96874-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="96874-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="96874-183">Int32</span><span class="sxs-lookup"><span data-stu-id="96874-183">Int32</span></span>|<span data-ttu-id="96874-184">出荷時のリセットまでに許可されるサインインの失敗回数。</span><span class="sxs-lookup"><span data-stu-id="96874-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="96874-185">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="96874-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="96874-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="96874-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="96874-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="96874-187">Boolean</span></span>|<span data-ttu-id="96874-188">デバイスが不明なソースからのアプリのインストールを許可しないことを要求します。</span><span class="sxs-lookup"><span data-stu-id="96874-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="96874-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="96874-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="96874-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="96874-190">Boolean</span></span>|<span data-ttu-id="96874-191">Android デバイスでの USB デバッグを無効にします。</span><span class="sxs-lookup"><span data-stu-id="96874-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="96874-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="96874-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="96874-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="96874-193">Boolean</span></span>|<span data-ttu-id="96874-194">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="96874-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="96874-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="96874-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="96874-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="96874-196">Boolean</span></span>|<span data-ttu-id="96874-197">デバイスの脅威保護が有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="96874-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="96874-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="96874-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="96874-199">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="96874-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="96874-200">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="96874-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="96874-201">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="96874-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="96874-202">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="96874-202">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="96874-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="96874-203">Boolean</span></span>|<span data-ttu-id="96874-204">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="96874-204">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="96874-205">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="96874-205">osMinimumVersion</span></span>|<span data-ttu-id="96874-206">String</span><span class="sxs-lookup"><span data-stu-id="96874-206">String</span></span>|<span data-ttu-id="96874-207">Android の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="96874-207">Minimum Android version.</span></span>|
|<span data-ttu-id="96874-208">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="96874-208">osMaximumVersion</span></span>|<span data-ttu-id="96874-209">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="96874-209">String</span></span>|<span data-ttu-id="96874-210">Android の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="96874-210">Maximum Android version.</span></span>|
|<span data-ttu-id="96874-211">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="96874-211">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="96874-212">String</span><span class="sxs-lookup"><span data-stu-id="96874-212">String</span></span>|<span data-ttu-id="96874-213">Android セキュリティ パッチの最小レベル。</span><span class="sxs-lookup"><span data-stu-id="96874-213">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="96874-214">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="96874-214">storageRequireEncryption</span></span>|<span data-ttu-id="96874-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="96874-215">Boolean</span></span>|<span data-ttu-id="96874-216">Android デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="96874-216">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="96874-217">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="96874-217">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="96874-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="96874-218">Boolean</span></span>|<span data-ttu-id="96874-219">デバイスが SafetyNet の基本整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="96874-219">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="96874-220">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="96874-220">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="96874-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="96874-221">Boolean</span></span>|<span data-ttu-id="96874-222">デバイスが SafetyNet の認定デバイス チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="96874-222">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="96874-223">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="96874-223">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="96874-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="96874-224">Boolean</span></span>|<span data-ttu-id="96874-225">Google Play 開発者サービスがデバイスにインストールされて有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="96874-225">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="96874-226">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="96874-226">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="96874-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="96874-227">Boolean</span></span>|<span data-ttu-id="96874-228">デバイスに最新のセキュリティ プロバイダーが必要です。</span><span class="sxs-lookup"><span data-stu-id="96874-228">Require the device to have up to date security providers.</span></span> <span data-ttu-id="96874-229">デバイスで Google Play 開発者サービスが有効かつ最新の状態になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="96874-229">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="96874-230">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="96874-230">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="96874-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="96874-231">Boolean</span></span>|<span data-ttu-id="96874-232">デバイスが会社のポータル クライアント アプリのランタイム整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="96874-232">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="96874-233">conditionStatementId</span><span class="sxs-lookup"><span data-stu-id="96874-233">conditionStatementId</span></span>|<span data-ttu-id="96874-234">String</span><span class="sxs-lookup"><span data-stu-id="96874-234">String</span></span>|<span data-ttu-id="96874-235">条件ステートメントの id。</span><span class="sxs-lookup"><span data-stu-id="96874-235">Condition statement id.</span></span>|
|<span data-ttu-id="96874-236">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="96874-236">restrictedApps</span></span>|<span data-ttu-id="96874-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="96874-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="96874-238">デバイスに、指定されたアプリがインストールされていないことを要求します。</span><span class="sxs-lookup"><span data-stu-id="96874-238">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="96874-239">このコレクションには、最大100個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="96874-239">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="96874-240">応答</span><span class="sxs-lookup"><span data-stu-id="96874-240">Response</span></span>
<span data-ttu-id="96874-241">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="96874-241">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96874-242">例</span><span class="sxs-lookup"><span data-stu-id="96874-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="96874-243">要求</span><span class="sxs-lookup"><span data-stu-id="96874-243">Request</span></span>
<span data-ttu-id="96874-244">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="96874-244">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1588

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
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

### <a name="response"></a><span data-ttu-id="96874-245">応答</span><span class="sxs-lookup"><span data-stu-id="96874-245">Response</span></span>
<span data-ttu-id="96874-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="96874-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1760

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
  "passwordSignInFailureCountBeforeFactoryReset": 12,
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





