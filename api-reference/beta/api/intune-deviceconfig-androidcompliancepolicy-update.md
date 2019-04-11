---
title: Update androidCompliancePolicy
description: androidCompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f9f2158e3948c3bd144c63b1ac86ed0806502c7b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785434"
---
# <a name="update-androidcompliancepolicy"></a><span data-ttu-id="8e7c2-103">Update androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="8e7c2-103">Update androidCompliancePolicy</span></span>

> <span data-ttu-id="8e7c2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e7c2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e7c2-106">[androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-106">Update the properties of a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e7c2-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8e7c2-107">Prerequisites</span></span>
<span data-ttu-id="8e7c2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e7c2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8e7c2-110">Permission type</span></span>|<span data-ttu-id="8e7c2-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8e7c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e7c2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8e7c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8e7c2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e7c2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e7c2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8e7c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e7c2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-115">Not supported.</span></span>|
|<span data-ttu-id="8e7c2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8e7c2-116">Application</span></span>|<span data-ttu-id="8e7c2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e7c2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8e7c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="8e7c2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8e7c2-119">Request headers</span></span>
|<span data-ttu-id="8e7c2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8e7c2-120">Header</span></span>|<span data-ttu-id="8e7c2-121">値</span><span class="sxs-lookup"><span data-stu-id="8e7c2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e7c2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e7c2-122">Authorization</span></span>|<span data-ttu-id="8e7c2-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e7c2-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8e7c2-124">Accept</span></span>|<span data-ttu-id="8e7c2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8e7c2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e7c2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8e7c2-126">Request body</span></span>
<span data-ttu-id="8e7c2-127">要求本文において、[androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) オブジェクト用の JSON 表記を提供します。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-127">In the request body, supply a JSON representation for the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

<span data-ttu-id="8e7c2-128">次の表に、[androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-128">The following table shows the properties that are required when you create the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span></span>

|<span data-ttu-id="8e7c2-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e7c2-129">Property</span></span>|<span data-ttu-id="8e7c2-130">型</span><span class="sxs-lookup"><span data-stu-id="8e7c2-130">Type</span></span>|<span data-ttu-id="8e7c2-131">説明</span><span class="sxs-lookup"><span data-stu-id="8e7c2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e7c2-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8e7c2-132">roleScopeTagIds</span></span>|<span data-ttu-id="8e7c2-133">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8e7c2-133">String collection</span></span>|<span data-ttu-id="8e7c2-134">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8e7c2-135">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e7c2-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8e7c2-136">id</span><span class="sxs-lookup"><span data-stu-id="8e7c2-136">id</span></span>|<span data-ttu-id="8e7c2-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8e7c2-137">String</span></span>|<span data-ttu-id="8e7c2-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-138">Key of the entity.</span></span> <span data-ttu-id="8e7c2-139">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e7c2-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8e7c2-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e7c2-140">createdDateTime</span></span>|<span data-ttu-id="8e7c2-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e7c2-141">DateTimeOffset</span></span>|<span data-ttu-id="8e7c2-142">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-142">DateTime the object was created.</span></span> <span data-ttu-id="8e7c2-143">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e7c2-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8e7c2-144">説明</span><span class="sxs-lookup"><span data-stu-id="8e7c2-144">description</span></span>|<span data-ttu-id="8e7c2-145">String</span><span class="sxs-lookup"><span data-stu-id="8e7c2-145">String</span></span>|<span data-ttu-id="8e7c2-146">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8e7c2-147">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e7c2-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8e7c2-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e7c2-148">lastModifiedDateTime</span></span>|<span data-ttu-id="8e7c2-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e7c2-149">DateTimeOffset</span></span>|<span data-ttu-id="8e7c2-150">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-150">DateTime the object was last modified.</span></span> <span data-ttu-id="8e7c2-151">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e7c2-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8e7c2-152">displayName</span><span class="sxs-lookup"><span data-stu-id="8e7c2-152">displayName</span></span>|<span data-ttu-id="8e7c2-153">String</span><span class="sxs-lookup"><span data-stu-id="8e7c2-153">String</span></span>|<span data-ttu-id="8e7c2-154">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8e7c2-155">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e7c2-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8e7c2-156">version</span><span class="sxs-lookup"><span data-stu-id="8e7c2-156">version</span></span>|<span data-ttu-id="8e7c2-157">Int32</span><span class="sxs-lookup"><span data-stu-id="8e7c2-157">Int32</span></span>|<span data-ttu-id="8e7c2-158">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-158">Version of the device configuration.</span></span> <span data-ttu-id="8e7c2-159">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e7c2-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8e7c2-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="8e7c2-160">passwordRequired</span></span>|<span data-ttu-id="8e7c2-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e7c2-161">Boolean</span></span>|<span data-ttu-id="8e7c2-162">デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="8e7c2-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8e7c2-163">passwordMinimumLength</span></span>|<span data-ttu-id="8e7c2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8e7c2-164">Int32</span></span>|<span data-ttu-id="8e7c2-165">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-165">Minimum password length.</span></span> <span data-ttu-id="8e7c2-166">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="8e7c2-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="8e7c2-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8e7c2-167">passwordRequiredType</span></span>|[<span data-ttu-id="8e7c2-168">androidrequiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="8e7c2-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="8e7c2-169">パスワードの文字の種類。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-169">Type of characters in password.</span></span> <span data-ttu-id="8e7c2-170">可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="8e7c2-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="8e7c2-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="8e7c2-172">Int32</span><span class="sxs-lookup"><span data-stu-id="8e7c2-172">Int32</span></span>|<span data-ttu-id="8e7c2-173">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="8e7c2-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8e7c2-174">passwordExpirationDays</span></span>|<span data-ttu-id="8e7c2-175">Int32</span><span class="sxs-lookup"><span data-stu-id="8e7c2-175">Int32</span></span>|<span data-ttu-id="8e7c2-176">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-176">Number of days before the password expires.</span></span> <span data-ttu-id="8e7c2-177">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="8e7c2-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="8e7c2-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8e7c2-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8e7c2-179">Int32</span><span class="sxs-lookup"><span data-stu-id="8e7c2-179">Int32</span></span>|<span data-ttu-id="8e7c2-180">禁止する、以前のパスワードの数です。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-180">Number of previous passwords to block.</span></span> <span data-ttu-id="8e7c2-181">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="8e7c2-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="8e7c2-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="8e7c2-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="8e7c2-183">Int32</span><span class="sxs-lookup"><span data-stu-id="8e7c2-183">Int32</span></span>|<span data-ttu-id="8e7c2-184">出荷時のリセットまでに許可されるサインインの失敗回数。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="8e7c2-185">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="8e7c2-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8e7c2-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="8e7c2-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="8e7c2-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e7c2-187">Boolean</span></span>|<span data-ttu-id="8e7c2-188">デバイスが不明なソースからのアプリのインストールを許可しないことを要求します。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="8e7c2-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="8e7c2-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="8e7c2-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e7c2-190">Boolean</span></span>|<span data-ttu-id="8e7c2-191">Android デバイスでの USB デバッグを無効にします。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="8e7c2-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="8e7c2-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="8e7c2-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e7c2-193">Boolean</span></span>|<span data-ttu-id="8e7c2-194">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="8e7c2-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="8e7c2-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="8e7c2-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e7c2-196">Boolean</span></span>|<span data-ttu-id="8e7c2-197">デバイスの脅威保護が有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="8e7c2-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8e7c2-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="8e7c2-199">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="8e7c2-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="8e7c2-200">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="8e7c2-201">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="8e7c2-202">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="8e7c2-202">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="8e7c2-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e7c2-203">Boolean</span></span>|<span data-ttu-id="8e7c2-204">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-204">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="8e7c2-205">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8e7c2-205">osMinimumVersion</span></span>|<span data-ttu-id="8e7c2-206">文字列</span><span class="sxs-lookup"><span data-stu-id="8e7c2-206">String</span></span>|<span data-ttu-id="8e7c2-207">Android の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-207">Minimum Android version.</span></span>|
|<span data-ttu-id="8e7c2-208">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8e7c2-208">osMaximumVersion</span></span>|<span data-ttu-id="8e7c2-209">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8e7c2-209">String</span></span>|<span data-ttu-id="8e7c2-210">Android の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-210">Maximum Android version.</span></span>|
|<span data-ttu-id="8e7c2-211">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="8e7c2-211">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="8e7c2-212">String</span><span class="sxs-lookup"><span data-stu-id="8e7c2-212">String</span></span>|<span data-ttu-id="8e7c2-213">Android セキュリティ パッチの最小レベル。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-213">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="8e7c2-214">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="8e7c2-214">storageRequireEncryption</span></span>|<span data-ttu-id="8e7c2-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e7c2-215">Boolean</span></span>|<span data-ttu-id="8e7c2-216">Android デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-216">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="8e7c2-217">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="8e7c2-217">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="8e7c2-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e7c2-218">Boolean</span></span>|<span data-ttu-id="8e7c2-219">デバイスが SafetyNet の基本整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-219">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="8e7c2-220">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="8e7c2-220">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="8e7c2-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e7c2-221">Boolean</span></span>|<span data-ttu-id="8e7c2-222">デバイスが SafetyNet の認定デバイス チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-222">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="8e7c2-223">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="8e7c2-223">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="8e7c2-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e7c2-224">Boolean</span></span>|<span data-ttu-id="8e7c2-225">Google Play 開発者サービスがデバイスにインストールされて有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-225">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="8e7c2-226">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="8e7c2-226">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="8e7c2-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e7c2-227">Boolean</span></span>|<span data-ttu-id="8e7c2-228">デバイスに最新のセキュリティ プロバイダーが必要です。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-228">Require the device to have up to date security providers.</span></span> <span data-ttu-id="8e7c2-229">デバイスで Google Play 開発者サービスが有効かつ最新の状態になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-229">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="8e7c2-230">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="8e7c2-230">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="8e7c2-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e7c2-231">Boolean</span></span>|<span data-ttu-id="8e7c2-232">デバイスが会社のポータル クライアント アプリのランタイム整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-232">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="8e7c2-233">conditionStatementId</span><span class="sxs-lookup"><span data-stu-id="8e7c2-233">conditionStatementId</span></span>|<span data-ttu-id="8e7c2-234">文字列</span><span class="sxs-lookup"><span data-stu-id="8e7c2-234">String</span></span>|<span data-ttu-id="8e7c2-235">条件ステートメントの id。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-235">Condition statement id.</span></span>|
|<span data-ttu-id="8e7c2-236">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="8e7c2-236">restrictedApps</span></span>|<span data-ttu-id="8e7c2-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8e7c2-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="8e7c2-238">デバイスに、指定されたアプリがインストールされていないことを要求します。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-238">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="8e7c2-239">このコレクションには、最大100個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-239">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="8e7c2-240">応答</span><span class="sxs-lookup"><span data-stu-id="8e7c2-240">Response</span></span>
<span data-ttu-id="8e7c2-241">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-241">If successful, this method returns a `200 OK` response code and an updated [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e7c2-242">例</span><span class="sxs-lookup"><span data-stu-id="8e7c2-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e7c2-243">要求</span><span class="sxs-lookup"><span data-stu-id="8e7c2-243">Request</span></span>
<span data-ttu-id="8e7c2-244">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-244">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="8e7c2-245">応答</span><span class="sxs-lookup"><span data-stu-id="8e7c2-245">Response</span></span>
<span data-ttu-id="8e7c2-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8e7c2-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





