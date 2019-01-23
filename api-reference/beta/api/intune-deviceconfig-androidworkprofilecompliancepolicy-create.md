---
title: AndroidWorkProfileCompliancePolicy を作成します。
description: 新しい androidWorkProfileCompliancePolicy オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b650a56ab36f4fc8062eefe8cb6cbd7f23be826
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401307"
---
# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="bf533-103">AndroidWorkProfileCompliancePolicy を作成します。</span><span class="sxs-lookup"><span data-stu-id="bf533-103">Create androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="bf533-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bf533-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bf533-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf533-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf533-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bf533-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf533-107">新しい[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bf533-107">Create a new [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf533-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="bf533-108">Prerequisites</span></span>
<span data-ttu-id="bf533-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf533-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bf533-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bf533-111">Permission type</span></span>|<span data-ttu-id="bf533-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bf533-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf533-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bf533-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bf533-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf533-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bf533-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bf533-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf533-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf533-116">Not supported.</span></span>|
|<span data-ttu-id="bf533-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bf533-117">Application</span></span>|<span data-ttu-id="bf533-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf533-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf533-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bf533-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="bf533-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bf533-120">Request headers</span></span>
|<span data-ttu-id="bf533-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bf533-121">Header</span></span>|<span data-ttu-id="bf533-122">値</span><span class="sxs-lookup"><span data-stu-id="bf533-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf533-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf533-123">Authorization</span></span>|<span data-ttu-id="bf533-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bf533-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf533-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bf533-125">Accept</span></span>|<span data-ttu-id="bf533-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bf533-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf533-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="bf533-127">Request body</span></span>
<span data-ttu-id="bf533-128">要求の本文に androidWorkProfileCompliancePolicy オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="bf533-128">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="bf533-129">次の表は、androidWorkProfileCompliancePolicy を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bf533-129">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="bf533-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf533-130">Property</span></span>|<span data-ttu-id="bf533-131">型</span><span class="sxs-lookup"><span data-stu-id="bf533-131">Type</span></span>|<span data-ttu-id="bf533-132">説明</span><span class="sxs-lookup"><span data-stu-id="bf533-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf533-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bf533-133">roleScopeTagIds</span></span>|<span data-ttu-id="bf533-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="bf533-134">String collection</span></span>|<span data-ttu-id="bf533-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="bf533-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bf533-136">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bf533-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bf533-137">id</span><span class="sxs-lookup"><span data-stu-id="bf533-137">id</span></span>|<span data-ttu-id="bf533-138">String</span><span class="sxs-lookup"><span data-stu-id="bf533-138">String</span></span>|<span data-ttu-id="bf533-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="bf533-139">Key of the entity.</span></span> <span data-ttu-id="bf533-140">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bf533-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bf533-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bf533-141">createdDateTime</span></span>|<span data-ttu-id="bf533-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf533-142">DateTimeOffset</span></span>|<span data-ttu-id="bf533-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="bf533-143">DateTime the object was created.</span></span> <span data-ttu-id="bf533-144">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bf533-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bf533-145">説明</span><span class="sxs-lookup"><span data-stu-id="bf533-145">description</span></span>|<span data-ttu-id="bf533-146">String</span><span class="sxs-lookup"><span data-stu-id="bf533-146">String</span></span>|<span data-ttu-id="bf533-147">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="bf533-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bf533-148">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bf533-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bf533-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf533-149">lastModifiedDateTime</span></span>|<span data-ttu-id="bf533-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf533-150">DateTimeOffset</span></span>|<span data-ttu-id="bf533-151">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="bf533-151">DateTime the object was last modified.</span></span> <span data-ttu-id="bf533-152">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bf533-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bf533-153">displayName</span><span class="sxs-lookup"><span data-stu-id="bf533-153">displayName</span></span>|<span data-ttu-id="bf533-154">String</span><span class="sxs-lookup"><span data-stu-id="bf533-154">String</span></span>|<span data-ttu-id="bf533-155">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="bf533-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bf533-156">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bf533-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bf533-157">version</span><span class="sxs-lookup"><span data-stu-id="bf533-157">version</span></span>|<span data-ttu-id="bf533-158">Int32</span><span class="sxs-lookup"><span data-stu-id="bf533-158">Int32</span></span>|<span data-ttu-id="bf533-159">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="bf533-159">Version of the device configuration.</span></span> <span data-ttu-id="bf533-160">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bf533-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bf533-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="bf533-161">passwordRequired</span></span>|<span data-ttu-id="bf533-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf533-162">Boolean</span></span>|<span data-ttu-id="bf533-163">デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="bf533-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="bf533-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="bf533-164">passwordMinimumLength</span></span>|<span data-ttu-id="bf533-165">Int32</span><span class="sxs-lookup"><span data-stu-id="bf533-165">Int32</span></span>|<span data-ttu-id="bf533-166">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="bf533-166">Minimum password length.</span></span> <span data-ttu-id="bf533-167">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="bf533-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="bf533-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="bf533-168">passwordRequiredType</span></span>|[<span data-ttu-id="bf533-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="bf533-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="bf533-170">パスワード内の文字の種類です。</span><span class="sxs-lookup"><span data-stu-id="bf533-170">Type of characters in password.</span></span> <span data-ttu-id="bf533-171">可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。</span><span class="sxs-lookup"><span data-stu-id="bf533-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="bf533-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="bf533-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="bf533-173">Int32</span><span class="sxs-lookup"><span data-stu-id="bf533-173">Int32</span></span>|<span data-ttu-id="bf533-174">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="bf533-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="bf533-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="bf533-175">passwordExpirationDays</span></span>|<span data-ttu-id="bf533-176">Int32</span><span class="sxs-lookup"><span data-stu-id="bf533-176">Int32</span></span>|<span data-ttu-id="bf533-177">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="bf533-177">Number of days before the password expires.</span></span> <span data-ttu-id="bf533-178">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="bf533-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="bf533-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="bf533-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="bf533-180">Int32</span><span class="sxs-lookup"><span data-stu-id="bf533-180">Int32</span></span>|<span data-ttu-id="bf533-181">禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="bf533-181">Number of previous passwords to block.</span></span> <span data-ttu-id="bf533-182">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="bf533-182">Valid values 1 to 24</span></span>|
|<span data-ttu-id="bf533-183">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="bf533-183">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="bf533-184">Int32</span><span class="sxs-lookup"><span data-stu-id="bf533-184">Int32</span></span>|<span data-ttu-id="bf533-185">工場出荷時リセットする前に許容されるサインインの障害の数です。</span><span class="sxs-lookup"><span data-stu-id="bf533-185">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="bf533-186">有効な値 1 ~ 16</span><span class="sxs-lookup"><span data-stu-id="bf533-186">Valid values 1 to 16</span></span>|
|<span data-ttu-id="bf533-187">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="bf533-187">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="bf533-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf533-188">Boolean</span></span>|<span data-ttu-id="bf533-189">デバイスが不明なソースからのアプリのインストールを許可しないことを要求します。</span><span class="sxs-lookup"><span data-stu-id="bf533-189">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="bf533-190">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="bf533-190">securityDisableUsbDebugging</span></span>|<span data-ttu-id="bf533-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf533-191">Boolean</span></span>|<span data-ttu-id="bf533-192">Android デバイスでの USB デバッグを無効にします。</span><span class="sxs-lookup"><span data-stu-id="bf533-192">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="bf533-193">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="bf533-193">securityRequireVerifyApps</span></span>|<span data-ttu-id="bf533-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf533-194">Boolean</span></span>|<span data-ttu-id="bf533-195">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="bf533-195">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="bf533-196">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="bf533-196">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="bf533-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf533-197">Boolean</span></span>|<span data-ttu-id="bf533-198">デバイスの脅威保護が有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="bf533-198">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="bf533-199">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="bf533-199">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="bf533-200">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="bf533-200">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="bf533-201">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="bf533-201">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="bf533-202">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="bf533-202">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="bf533-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="bf533-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="bf533-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf533-204">Boolean</span></span>|<span data-ttu-id="bf533-205">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="bf533-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="bf533-206">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="bf533-206">osMinimumVersion</span></span>|<span data-ttu-id="bf533-207">String</span><span class="sxs-lookup"><span data-stu-id="bf533-207">String</span></span>|<span data-ttu-id="bf533-208">Android の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="bf533-208">Minimum Android version.</span></span>|
|<span data-ttu-id="bf533-209">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="bf533-209">osMaximumVersion</span></span>|<span data-ttu-id="bf533-210">String</span><span class="sxs-lookup"><span data-stu-id="bf533-210">String</span></span>|<span data-ttu-id="bf533-211">Android の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="bf533-211">Maximum Android version.</span></span>|
|<span data-ttu-id="bf533-212">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="bf533-212">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="bf533-213">String</span><span class="sxs-lookup"><span data-stu-id="bf533-213">String</span></span>|<span data-ttu-id="bf533-214">Android セキュリティ パッチの最小レベル。</span><span class="sxs-lookup"><span data-stu-id="bf533-214">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="bf533-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="bf533-215">storageRequireEncryption</span></span>|<span data-ttu-id="bf533-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf533-216">Boolean</span></span>|<span data-ttu-id="bf533-217">Android デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="bf533-217">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="bf533-218">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="bf533-218">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="bf533-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf533-219">Boolean</span></span>|<span data-ttu-id="bf533-220">デバイスが SafetyNet の基本整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="bf533-220">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="bf533-221">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="bf533-221">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="bf533-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf533-222">Boolean</span></span>|<span data-ttu-id="bf533-223">デバイスが SafetyNet の認定デバイス チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="bf533-223">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="bf533-224">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="bf533-224">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="bf533-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf533-225">Boolean</span></span>|<span data-ttu-id="bf533-226">Google Play 開発者サービスがデバイスにインストールされて有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="bf533-226">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="bf533-227">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="bf533-227">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="bf533-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf533-228">Boolean</span></span>|<span data-ttu-id="bf533-229">デバイスに最新のセキュリティ プロバイダーが必要です。</span><span class="sxs-lookup"><span data-stu-id="bf533-229">Require the device to have up to date security providers.</span></span> <span data-ttu-id="bf533-230">デバイスで Google Play 開発者サービスが有効かつ最新の状態になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bf533-230">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="bf533-231">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="bf533-231">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="bf533-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf533-232">Boolean</span></span>|<span data-ttu-id="bf533-233">デバイスが会社のポータル クライアント アプリのランタイム整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="bf533-233">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="bf533-234">応答</span><span class="sxs-lookup"><span data-stu-id="bf533-234">Response</span></span>
<span data-ttu-id="bf533-235">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="bf533-235">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf533-236">例</span><span class="sxs-lookup"><span data-stu-id="bf533-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf533-237">要求</span><span class="sxs-lookup"><span data-stu-id="bf533-237">Request</span></span>
<span data-ttu-id="bf533-238">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bf533-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1287

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
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
  "securityRequireCompanyPortalAppIntegrity": true
}
```

### <a name="response"></a><span data-ttu-id="bf533-239">応答</span><span class="sxs-lookup"><span data-stu-id="bf533-239">Response</span></span>
<span data-ttu-id="bf533-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bf533-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1459

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
  "securityRequireCompanyPortalAppIntegrity": true
}
```




