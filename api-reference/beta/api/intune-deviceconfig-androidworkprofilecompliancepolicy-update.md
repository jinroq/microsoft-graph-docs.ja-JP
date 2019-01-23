---
title: AndroidWorkProfileCompliancePolicy を更新します。
description: AndroidWorkProfileCompliancePolicy オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ead60a0683738de51947e1186e8821f55651ca15
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402805"
---
# <a name="update-androidworkprofilecompliancepolicy"></a><span data-ttu-id="638bf-103">AndroidWorkProfileCompliancePolicy を更新します。</span><span class="sxs-lookup"><span data-stu-id="638bf-103">Update androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="638bf-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="638bf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="638bf-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="638bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="638bf-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="638bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="638bf-107">[AndroidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="638bf-107">Update the properties of a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="638bf-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="638bf-108">Prerequisites</span></span>
<span data-ttu-id="638bf-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="638bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="638bf-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="638bf-111">Permission type</span></span>|<span data-ttu-id="638bf-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="638bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="638bf-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="638bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="638bf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="638bf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="638bf-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="638bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="638bf-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="638bf-116">Not supported.</span></span>|
|<span data-ttu-id="638bf-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="638bf-117">Application</span></span>|<span data-ttu-id="638bf-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="638bf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="638bf-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="638bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="638bf-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="638bf-120">Request headers</span></span>
|<span data-ttu-id="638bf-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="638bf-121">Header</span></span>|<span data-ttu-id="638bf-122">値</span><span class="sxs-lookup"><span data-stu-id="638bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="638bf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="638bf-123">Authorization</span></span>|<span data-ttu-id="638bf-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="638bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="638bf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="638bf-125">Accept</span></span>|<span data-ttu-id="638bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="638bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="638bf-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="638bf-127">Request body</span></span>
<span data-ttu-id="638bf-128">要求の本文に[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="638bf-128">In the request body, supply a JSON representation for the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="638bf-129">[AndroidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="638bf-129">The following table shows the properties that are required when you create the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md).</span></span>

|<span data-ttu-id="638bf-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="638bf-130">Property</span></span>|<span data-ttu-id="638bf-131">型</span><span class="sxs-lookup"><span data-stu-id="638bf-131">Type</span></span>|<span data-ttu-id="638bf-132">説明</span><span class="sxs-lookup"><span data-stu-id="638bf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="638bf-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="638bf-133">roleScopeTagIds</span></span>|<span data-ttu-id="638bf-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="638bf-134">String collection</span></span>|<span data-ttu-id="638bf-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="638bf-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="638bf-136">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="638bf-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="638bf-137">id</span><span class="sxs-lookup"><span data-stu-id="638bf-137">id</span></span>|<span data-ttu-id="638bf-138">String</span><span class="sxs-lookup"><span data-stu-id="638bf-138">String</span></span>|<span data-ttu-id="638bf-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="638bf-139">Key of the entity.</span></span> <span data-ttu-id="638bf-140">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="638bf-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="638bf-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="638bf-141">createdDateTime</span></span>|<span data-ttu-id="638bf-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="638bf-142">DateTimeOffset</span></span>|<span data-ttu-id="638bf-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="638bf-143">DateTime the object was created.</span></span> <span data-ttu-id="638bf-144">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="638bf-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="638bf-145">説明</span><span class="sxs-lookup"><span data-stu-id="638bf-145">description</span></span>|<span data-ttu-id="638bf-146">String</span><span class="sxs-lookup"><span data-stu-id="638bf-146">String</span></span>|<span data-ttu-id="638bf-147">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="638bf-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="638bf-148">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="638bf-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="638bf-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="638bf-149">lastModifiedDateTime</span></span>|<span data-ttu-id="638bf-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="638bf-150">DateTimeOffset</span></span>|<span data-ttu-id="638bf-151">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="638bf-151">DateTime the object was last modified.</span></span> <span data-ttu-id="638bf-152">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="638bf-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="638bf-153">displayName</span><span class="sxs-lookup"><span data-stu-id="638bf-153">displayName</span></span>|<span data-ttu-id="638bf-154">String</span><span class="sxs-lookup"><span data-stu-id="638bf-154">String</span></span>|<span data-ttu-id="638bf-155">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="638bf-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="638bf-156">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="638bf-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="638bf-157">version</span><span class="sxs-lookup"><span data-stu-id="638bf-157">version</span></span>|<span data-ttu-id="638bf-158">Int32</span><span class="sxs-lookup"><span data-stu-id="638bf-158">Int32</span></span>|<span data-ttu-id="638bf-159">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="638bf-159">Version of the device configuration.</span></span> <span data-ttu-id="638bf-160">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="638bf-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="638bf-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="638bf-161">passwordRequired</span></span>|<span data-ttu-id="638bf-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="638bf-162">Boolean</span></span>|<span data-ttu-id="638bf-163">デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="638bf-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="638bf-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="638bf-164">passwordMinimumLength</span></span>|<span data-ttu-id="638bf-165">Int32</span><span class="sxs-lookup"><span data-stu-id="638bf-165">Int32</span></span>|<span data-ttu-id="638bf-166">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="638bf-166">Minimum password length.</span></span> <span data-ttu-id="638bf-167">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="638bf-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="638bf-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="638bf-168">passwordRequiredType</span></span>|[<span data-ttu-id="638bf-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="638bf-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="638bf-170">パスワード内の文字の種類です。</span><span class="sxs-lookup"><span data-stu-id="638bf-170">Type of characters in password.</span></span> <span data-ttu-id="638bf-171">可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。</span><span class="sxs-lookup"><span data-stu-id="638bf-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="638bf-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="638bf-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="638bf-173">Int32</span><span class="sxs-lookup"><span data-stu-id="638bf-173">Int32</span></span>|<span data-ttu-id="638bf-174">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="638bf-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="638bf-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="638bf-175">passwordExpirationDays</span></span>|<span data-ttu-id="638bf-176">Int32</span><span class="sxs-lookup"><span data-stu-id="638bf-176">Int32</span></span>|<span data-ttu-id="638bf-177">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="638bf-177">Number of days before the password expires.</span></span> <span data-ttu-id="638bf-178">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="638bf-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="638bf-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="638bf-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="638bf-180">Int32</span><span class="sxs-lookup"><span data-stu-id="638bf-180">Int32</span></span>|<span data-ttu-id="638bf-181">禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="638bf-181">Number of previous passwords to block.</span></span> <span data-ttu-id="638bf-182">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="638bf-182">Valid values 1 to 24</span></span>|
|<span data-ttu-id="638bf-183">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="638bf-183">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="638bf-184">Int32</span><span class="sxs-lookup"><span data-stu-id="638bf-184">Int32</span></span>|<span data-ttu-id="638bf-185">工場出荷時リセットする前に許容されるサインインの障害の数です。</span><span class="sxs-lookup"><span data-stu-id="638bf-185">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="638bf-186">有効な値 1 ~ 16</span><span class="sxs-lookup"><span data-stu-id="638bf-186">Valid values 1 to 16</span></span>|
|<span data-ttu-id="638bf-187">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="638bf-187">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="638bf-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="638bf-188">Boolean</span></span>|<span data-ttu-id="638bf-189">デバイスが不明なソースからのアプリのインストールを許可しないことを要求します。</span><span class="sxs-lookup"><span data-stu-id="638bf-189">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="638bf-190">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="638bf-190">securityDisableUsbDebugging</span></span>|<span data-ttu-id="638bf-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="638bf-191">Boolean</span></span>|<span data-ttu-id="638bf-192">Android デバイスでの USB デバッグを無効にします。</span><span class="sxs-lookup"><span data-stu-id="638bf-192">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="638bf-193">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="638bf-193">securityRequireVerifyApps</span></span>|<span data-ttu-id="638bf-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="638bf-194">Boolean</span></span>|<span data-ttu-id="638bf-195">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="638bf-195">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="638bf-196">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="638bf-196">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="638bf-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="638bf-197">Boolean</span></span>|<span data-ttu-id="638bf-198">デバイスの脅威保護が有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="638bf-198">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="638bf-199">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="638bf-199">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="638bf-200">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="638bf-200">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="638bf-201">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="638bf-201">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="638bf-202">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="638bf-202">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="638bf-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="638bf-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="638bf-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="638bf-204">Boolean</span></span>|<span data-ttu-id="638bf-205">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="638bf-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="638bf-206">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="638bf-206">osMinimumVersion</span></span>|<span data-ttu-id="638bf-207">String</span><span class="sxs-lookup"><span data-stu-id="638bf-207">String</span></span>|<span data-ttu-id="638bf-208">Android の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="638bf-208">Minimum Android version.</span></span>|
|<span data-ttu-id="638bf-209">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="638bf-209">osMaximumVersion</span></span>|<span data-ttu-id="638bf-210">String</span><span class="sxs-lookup"><span data-stu-id="638bf-210">String</span></span>|<span data-ttu-id="638bf-211">Android の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="638bf-211">Maximum Android version.</span></span>|
|<span data-ttu-id="638bf-212">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="638bf-212">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="638bf-213">String</span><span class="sxs-lookup"><span data-stu-id="638bf-213">String</span></span>|<span data-ttu-id="638bf-214">Android セキュリティ パッチの最小レベル。</span><span class="sxs-lookup"><span data-stu-id="638bf-214">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="638bf-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="638bf-215">storageRequireEncryption</span></span>|<span data-ttu-id="638bf-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="638bf-216">Boolean</span></span>|<span data-ttu-id="638bf-217">Android デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="638bf-217">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="638bf-218">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="638bf-218">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="638bf-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="638bf-219">Boolean</span></span>|<span data-ttu-id="638bf-220">デバイスが SafetyNet の基本整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="638bf-220">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="638bf-221">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="638bf-221">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="638bf-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="638bf-222">Boolean</span></span>|<span data-ttu-id="638bf-223">デバイスが SafetyNet の認定デバイス チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="638bf-223">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="638bf-224">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="638bf-224">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="638bf-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="638bf-225">Boolean</span></span>|<span data-ttu-id="638bf-226">Google Play 開発者サービスがデバイスにインストールされて有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="638bf-226">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="638bf-227">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="638bf-227">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="638bf-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="638bf-228">Boolean</span></span>|<span data-ttu-id="638bf-229">デバイスに最新のセキュリティ プロバイダーが必要です。</span><span class="sxs-lookup"><span data-stu-id="638bf-229">Require the device to have up to date security providers.</span></span> <span data-ttu-id="638bf-230">デバイスで Google Play 開発者サービスが有効かつ最新の状態になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="638bf-230">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="638bf-231">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="638bf-231">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="638bf-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="638bf-232">Boolean</span></span>|<span data-ttu-id="638bf-233">デバイスが会社のポータル クライアント アプリのランタイム整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="638bf-233">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="638bf-234">応答</span><span class="sxs-lookup"><span data-stu-id="638bf-234">Response</span></span>
<span data-ttu-id="638bf-235">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="638bf-235">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="638bf-236">例</span><span class="sxs-lookup"><span data-stu-id="638bf-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="638bf-237">要求</span><span class="sxs-lookup"><span data-stu-id="638bf-237">Request</span></span>
<span data-ttu-id="638bf-238">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="638bf-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="638bf-239">応答</span><span class="sxs-lookup"><span data-stu-id="638bf-239">Response</span></span>
<span data-ttu-id="638bf-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="638bf-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




