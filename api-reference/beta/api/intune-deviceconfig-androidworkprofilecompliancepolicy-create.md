---
title: AndroidWorkProfileCompliancePolicy を作成します。
description: 新しい androidWorkProfileCompliancePolicy オブジェクトを作成します。
ms.openlocfilehash: a937c1aab21264cda0920d662d2e13b379b42e8d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068609"
---
# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="0e3bb-103">AndroidWorkProfileCompliancePolicy を作成します。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-103">Create androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="0e3bb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e3bb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e3bb-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e3bb-107">新しい[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-107">Create a new [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0e3bb-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0e3bb-108">Prerequisites</span></span>
<span data-ttu-id="0e3bb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e3bb-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0e3bb-111">Permission type</span></span>|<span data-ttu-id="0e3bb-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0e3bb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e3bb-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0e3bb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e3bb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e3bb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e3bb-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0e3bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e3bb-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-116">Not supported.</span></span>|
|<span data-ttu-id="0e3bb-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0e3bb-117">Application</span></span>|<span data-ttu-id="0e3bb-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e3bb-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0e3bb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="0e3bb-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0e3bb-120">Request headers</span></span>
|<span data-ttu-id="0e3bb-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0e3bb-121">Header</span></span>|<span data-ttu-id="0e3bb-122">値</span><span class="sxs-lookup"><span data-stu-id="0e3bb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e3bb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e3bb-123">Authorization</span></span>|<span data-ttu-id="0e3bb-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e3bb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0e3bb-125">Accept</span></span>|<span data-ttu-id="0e3bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e3bb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e3bb-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0e3bb-127">Request body</span></span>
<span data-ttu-id="0e3bb-128">要求の本文に androidWorkProfileCompliancePolicy オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-128">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="0e3bb-129">次の表は、androidWorkProfileCompliancePolicy を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-129">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="0e3bb-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e3bb-130">Property</span></span>|<span data-ttu-id="0e3bb-131">型</span><span class="sxs-lookup"><span data-stu-id="0e3bb-131">Type</span></span>|<span data-ttu-id="0e3bb-132">説明</span><span class="sxs-lookup"><span data-stu-id="0e3bb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e3bb-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0e3bb-133">roleScopeTagIds</span></span>|<span data-ttu-id="0e3bb-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0e3bb-134">String collection</span></span>|<span data-ttu-id="0e3bb-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0e3bb-136">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0e3bb-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0e3bb-137">id</span><span class="sxs-lookup"><span data-stu-id="0e3bb-137">id</span></span>|<span data-ttu-id="0e3bb-138">String</span><span class="sxs-lookup"><span data-stu-id="0e3bb-138">String</span></span>|<span data-ttu-id="0e3bb-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-139">Key of the entity.</span></span> <span data-ttu-id="0e3bb-140">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0e3bb-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0e3bb-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e3bb-141">createdDateTime</span></span>|<span data-ttu-id="0e3bb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e3bb-142">DateTimeOffset</span></span>|<span data-ttu-id="0e3bb-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-143">DateTime the object was created.</span></span> <span data-ttu-id="0e3bb-144">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0e3bb-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0e3bb-145">説明</span><span class="sxs-lookup"><span data-stu-id="0e3bb-145">description</span></span>|<span data-ttu-id="0e3bb-146">String</span><span class="sxs-lookup"><span data-stu-id="0e3bb-146">String</span></span>|<span data-ttu-id="0e3bb-147">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0e3bb-148">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0e3bb-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0e3bb-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e3bb-149">lastModifiedDateTime</span></span>|<span data-ttu-id="0e3bb-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e3bb-150">DateTimeOffset</span></span>|<span data-ttu-id="0e3bb-151">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-151">DateTime the object was last modified.</span></span> <span data-ttu-id="0e3bb-152">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0e3bb-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0e3bb-153">displayName</span><span class="sxs-lookup"><span data-stu-id="0e3bb-153">displayName</span></span>|<span data-ttu-id="0e3bb-154">String</span><span class="sxs-lookup"><span data-stu-id="0e3bb-154">String</span></span>|<span data-ttu-id="0e3bb-155">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0e3bb-156">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0e3bb-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0e3bb-157">version</span><span class="sxs-lookup"><span data-stu-id="0e3bb-157">version</span></span>|<span data-ttu-id="0e3bb-158">Int32</span><span class="sxs-lookup"><span data-stu-id="0e3bb-158">Int32</span></span>|<span data-ttu-id="0e3bb-159">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-159">Version of the device configuration.</span></span> <span data-ttu-id="0e3bb-160">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0e3bb-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0e3bb-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="0e3bb-161">passwordRequired</span></span>|<span data-ttu-id="0e3bb-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e3bb-162">Boolean</span></span>|<span data-ttu-id="0e3bb-163">デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="0e3bb-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0e3bb-164">passwordMinimumLength</span></span>|<span data-ttu-id="0e3bb-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0e3bb-165">Int32</span></span>|<span data-ttu-id="0e3bb-166">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-166">Minimum password length.</span></span> <span data-ttu-id="0e3bb-167">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="0e3bb-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="0e3bb-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0e3bb-168">passwordRequiredType</span></span>|[<span data-ttu-id="0e3bb-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0e3bb-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="0e3bb-170">パスワード内の文字の種類です。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-170">Type of characters in password.</span></span> <span data-ttu-id="0e3bb-171">可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="0e3bb-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="0e3bb-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="0e3bb-173">Int32</span><span class="sxs-lookup"><span data-stu-id="0e3bb-173">Int32</span></span>|<span data-ttu-id="0e3bb-174">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="0e3bb-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0e3bb-175">passwordExpirationDays</span></span>|<span data-ttu-id="0e3bb-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0e3bb-176">Int32</span></span>|<span data-ttu-id="0e3bb-177">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-177">Number of days before the password expires.</span></span> <span data-ttu-id="0e3bb-178">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="0e3bb-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="0e3bb-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0e3bb-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0e3bb-180">Int32</span><span class="sxs-lookup"><span data-stu-id="0e3bb-180">Int32</span></span>|<span data-ttu-id="0e3bb-181">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-181">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="0e3bb-182">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="0e3bb-182">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="0e3bb-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e3bb-183">Boolean</span></span>|<span data-ttu-id="0e3bb-184">デバイスが不明なソースからのアプリのインストールを許可しないことを要求します。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-184">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="0e3bb-185">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="0e3bb-185">securityDisableUsbDebugging</span></span>|<span data-ttu-id="0e3bb-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e3bb-186">Boolean</span></span>|<span data-ttu-id="0e3bb-187">Android デバイスでの USB デバッグを無効にします。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-187">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="0e3bb-188">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="0e3bb-188">securityRequireVerifyApps</span></span>|<span data-ttu-id="0e3bb-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e3bb-189">Boolean</span></span>|<span data-ttu-id="0e3bb-190">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-190">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="0e3bb-191">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="0e3bb-191">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="0e3bb-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e3bb-192">Boolean</span></span>|<span data-ttu-id="0e3bb-193">デバイスの脅威保護が有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-193">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="0e3bb-194">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0e3bb-194">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="0e3bb-195">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="0e3bb-195">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="0e3bb-196">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-196">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="0e3bb-197">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-197">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="0e3bb-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="0e3bb-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="0e3bb-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e3bb-199">Boolean</span></span>|<span data-ttu-id="0e3bb-200">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="0e3bb-201">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0e3bb-201">osMinimumVersion</span></span>|<span data-ttu-id="0e3bb-202">String</span><span class="sxs-lookup"><span data-stu-id="0e3bb-202">String</span></span>|<span data-ttu-id="0e3bb-203">Android の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-203">Minimum Android version.</span></span>|
|<span data-ttu-id="0e3bb-204">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0e3bb-204">osMaximumVersion</span></span>|<span data-ttu-id="0e3bb-205">String</span><span class="sxs-lookup"><span data-stu-id="0e3bb-205">String</span></span>|<span data-ttu-id="0e3bb-206">Android の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-206">Maximum Android version.</span></span>|
|<span data-ttu-id="0e3bb-207">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="0e3bb-207">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="0e3bb-208">String</span><span class="sxs-lookup"><span data-stu-id="0e3bb-208">String</span></span>|<span data-ttu-id="0e3bb-209">Android セキュリティ パッチの最小レベル。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-209">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="0e3bb-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="0e3bb-210">storageRequireEncryption</span></span>|<span data-ttu-id="0e3bb-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e3bb-211">Boolean</span></span>|<span data-ttu-id="0e3bb-212">Android デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-212">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="0e3bb-213">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="0e3bb-213">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="0e3bb-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e3bb-214">Boolean</span></span>|<span data-ttu-id="0e3bb-215">デバイスが SafetyNet の基本整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-215">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="0e3bb-216">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="0e3bb-216">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="0e3bb-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e3bb-217">Boolean</span></span>|<span data-ttu-id="0e3bb-218">デバイスが SafetyNet の認定デバイス チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-218">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="0e3bb-219">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="0e3bb-219">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="0e3bb-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e3bb-220">Boolean</span></span>|<span data-ttu-id="0e3bb-221">Google Play 開発者サービスがデバイスにインストールされて有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-221">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="0e3bb-222">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="0e3bb-222">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="0e3bb-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e3bb-223">Boolean</span></span>|<span data-ttu-id="0e3bb-224">デバイスに最新のセキュリティ プロバイダーが必要です。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-224">Require the device to have up to date security providers.</span></span> <span data-ttu-id="0e3bb-225">デバイスで Google Play 開発者サービスが有効かつ最新の状態になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-225">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="0e3bb-226">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="0e3bb-226">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="0e3bb-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e3bb-227">Boolean</span></span>|<span data-ttu-id="0e3bb-228">デバイスが会社のポータル クライアント アプリのランタイム整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-228">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="0e3bb-229">応答</span><span class="sxs-lookup"><span data-stu-id="0e3bb-229">Response</span></span>
<span data-ttu-id="0e3bb-230">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-230">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e3bb-231">例</span><span class="sxs-lookup"><span data-stu-id="0e3bb-231">Example</span></span>
### <a name="request"></a><span data-ttu-id="0e3bb-232">要求</span><span class="sxs-lookup"><span data-stu-id="0e3bb-232">Request</span></span>
<span data-ttu-id="0e3bb-233">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-233">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1296

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="0e3bb-234">応答</span><span class="sxs-lookup"><span data-stu-id="0e3bb-234">Response</span></span>
<span data-ttu-id="0e3bb-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0e3bb-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





