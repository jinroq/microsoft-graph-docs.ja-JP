---
title: windows10MobileCompliancePolicy の更新
description: windows10MobileCompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eacb148516599e99437c3f8461338b01630c2afb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32516547"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="8ef00-103">windows10MobileCompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="8ef00-103">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="8ef00-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ef00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ef00-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8ef00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ef00-106">[windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8ef00-106">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ef00-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8ef00-107">Prerequisites</span></span>
<span data-ttu-id="8ef00-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ef00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ef00-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8ef00-110">Permission type</span></span>|<span data-ttu-id="8ef00-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8ef00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ef00-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8ef00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8ef00-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ef00-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ef00-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8ef00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ef00-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ef00-115">Not supported.</span></span>|
|<span data-ttu-id="8ef00-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8ef00-116">Application</span></span>|<span data-ttu-id="8ef00-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ef00-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ef00-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8ef00-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="8ef00-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ef00-119">Request headers</span></span>
|<span data-ttu-id="8ef00-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ef00-120">Header</span></span>|<span data-ttu-id="8ef00-121">値</span><span class="sxs-lookup"><span data-stu-id="8ef00-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ef00-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ef00-122">Authorization</span></span>|<span data-ttu-id="8ef00-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8ef00-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ef00-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8ef00-124">Accept</span></span>|<span data-ttu-id="8ef00-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8ef00-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ef00-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8ef00-126">Request body</span></span>
<span data-ttu-id="8ef00-127">要求本文で、[windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8ef00-127">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="8ef00-128">次の表に、[windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8ef00-128">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="8ef00-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ef00-129">Property</span></span>|<span data-ttu-id="8ef00-130">型</span><span class="sxs-lookup"><span data-stu-id="8ef00-130">Type</span></span>|<span data-ttu-id="8ef00-131">説明</span><span class="sxs-lookup"><span data-stu-id="8ef00-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ef00-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8ef00-132">roleScopeTagIds</span></span>|<span data-ttu-id="8ef00-133">String collection</span><span class="sxs-lookup"><span data-stu-id="8ef00-133">String collection</span></span>|<span data-ttu-id="8ef00-134">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="8ef00-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8ef00-135">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8ef00-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ef00-136">id</span><span class="sxs-lookup"><span data-stu-id="8ef00-136">id</span></span>|<span data-ttu-id="8ef00-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8ef00-137">String</span></span>|<span data-ttu-id="8ef00-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8ef00-138">Key of the entity.</span></span> <span data-ttu-id="8ef00-139">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8ef00-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ef00-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ef00-140">createdDateTime</span></span>|<span data-ttu-id="8ef00-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ef00-141">DateTimeOffset</span></span>|<span data-ttu-id="8ef00-142">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="8ef00-142">DateTime the object was created.</span></span> <span data-ttu-id="8ef00-143">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8ef00-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ef00-144">説明</span><span class="sxs-lookup"><span data-stu-id="8ef00-144">description</span></span>|<span data-ttu-id="8ef00-145">String</span><span class="sxs-lookup"><span data-stu-id="8ef00-145">String</span></span>|<span data-ttu-id="8ef00-146">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="8ef00-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8ef00-147">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8ef00-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ef00-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ef00-148">lastModifiedDateTime</span></span>|<span data-ttu-id="8ef00-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ef00-149">DateTimeOffset</span></span>|<span data-ttu-id="8ef00-150">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="8ef00-150">DateTime the object was last modified.</span></span> <span data-ttu-id="8ef00-151">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8ef00-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ef00-152">displayName</span><span class="sxs-lookup"><span data-stu-id="8ef00-152">displayName</span></span>|<span data-ttu-id="8ef00-153">String</span><span class="sxs-lookup"><span data-stu-id="8ef00-153">String</span></span>|<span data-ttu-id="8ef00-154">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="8ef00-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8ef00-155">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8ef00-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ef00-156">version</span><span class="sxs-lookup"><span data-stu-id="8ef00-156">version</span></span>|<span data-ttu-id="8ef00-157">Int32</span><span class="sxs-lookup"><span data-stu-id="8ef00-157">Int32</span></span>|<span data-ttu-id="8ef00-158">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="8ef00-158">Version of the device configuration.</span></span> <span data-ttu-id="8ef00-159">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8ef00-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ef00-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="8ef00-160">passwordRequired</span></span>|<span data-ttu-id="8ef00-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ef00-161">Boolean</span></span>|<span data-ttu-id="8ef00-162">Windows Phone デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="8ef00-162">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="8ef00-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="8ef00-163">passwordBlockSimple</span></span>|<span data-ttu-id="8ef00-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ef00-164">Boolean</span></span>|<span data-ttu-id="8ef00-165">カレンダーの同期を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8ef00-165">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="8ef00-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8ef00-166">passwordMinimumLength</span></span>|<span data-ttu-id="8ef00-167">Int32</span><span class="sxs-lookup"><span data-stu-id="8ef00-167">Int32</span></span>|<span data-ttu-id="8ef00-168">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="8ef00-168">Minimum password length.</span></span> <span data-ttu-id="8ef00-169">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="8ef00-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="8ef00-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="8ef00-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="8ef00-171">Int32</span><span class="sxs-lookup"><span data-stu-id="8ef00-171">Int32</span></span>|<span data-ttu-id="8ef00-172">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="8ef00-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="8ef00-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8ef00-173">passwordRequiredType</span></span>|[<span data-ttu-id="8ef00-174">requiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="8ef00-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="8ef00-175">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="8ef00-175">The required password type.</span></span> <span data-ttu-id="8ef00-176">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="8ef00-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="8ef00-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8ef00-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8ef00-178">Int32</span><span class="sxs-lookup"><span data-stu-id="8ef00-178">Int32</span></span>|<span data-ttu-id="8ef00-179">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="8ef00-179">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="8ef00-180">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8ef00-180">passwordExpirationDays</span></span>|<span data-ttu-id="8ef00-181">Int32</span><span class="sxs-lookup"><span data-stu-id="8ef00-181">Int32</span></span>|<span data-ttu-id="8ef00-182">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="8ef00-182">Number of days before password expiration.</span></span> <span data-ttu-id="8ef00-183">有効な値は 1 から 255 までです</span><span class="sxs-lookup"><span data-stu-id="8ef00-183">Valid values 1 to 255</span></span>|
|<span data-ttu-id="8ef00-184">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="8ef00-184">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="8ef00-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8ef00-185">Int32</span></span>|<span data-ttu-id="8ef00-186">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="8ef00-186">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="8ef00-187">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="8ef00-187">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="8ef00-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ef00-188">Boolean</span></span>|<span data-ttu-id="8ef00-189">アイドル デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="8ef00-189">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="8ef00-190">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8ef00-190">osMinimumVersion</span></span>|<span data-ttu-id="8ef00-191">String</span><span class="sxs-lookup"><span data-stu-id="8ef00-191">String</span></span>|<span data-ttu-id="8ef00-192">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="8ef00-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="8ef00-193">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8ef00-193">osMaximumVersion</span></span>|<span data-ttu-id="8ef00-194">String</span><span class="sxs-lookup"><span data-stu-id="8ef00-194">String</span></span>|<span data-ttu-id="8ef00-195">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="8ef00-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="8ef00-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="8ef00-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="8ef00-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ef00-197">Boolean</span></span>|<span data-ttu-id="8ef00-198">デバイスが Windows デバイス正常性構成証明によって正常と報告される (早期起動マルウェア対策ドライバーが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="8ef00-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="8ef00-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="8ef00-199">bitLockerEnabled</span></span>|<span data-ttu-id="8ef00-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ef00-200">Boolean</span></span>|<span data-ttu-id="8ef00-201">デバイスが Windows デバイス正常性構成証明によって正常と報告される (BitLocker が有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="8ef00-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="8ef00-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="8ef00-202">secureBootEnabled</span></span>|<span data-ttu-id="8ef00-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ef00-203">Boolean</span></span>|<span data-ttu-id="8ef00-204">デバイスが Windows デバイス正常性構成証明によって正常と報告される (セキュア ブートが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="8ef00-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="8ef00-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="8ef00-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="8ef00-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ef00-206">Boolean</span></span>|<span data-ttu-id="8ef00-207">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="8ef00-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="8ef00-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="8ef00-208">storageRequireEncryption</span></span>|<span data-ttu-id="8ef00-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ef00-209">Boolean</span></span>|<span data-ttu-id="8ef00-210">Windows デバイス上での暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="8ef00-210">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="8ef00-211">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="8ef00-211">activeFirewallRequired</span></span>|<span data-ttu-id="8ef00-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ef00-212">Boolean</span></span>|<span data-ttu-id="8ef00-213">Windows デバイスでアクティブなファイアウォールが必要です。</span><span class="sxs-lookup"><span data-stu-id="8ef00-213">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="8ef00-214">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="8ef00-214">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="8ef00-215">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8ef00-215">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="8ef00-216">Windows デバイス上の有効なオペレーティングシステムのビルド範囲。</span><span class="sxs-lookup"><span data-stu-id="8ef00-216">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="8ef00-217">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="8ef00-217">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="8ef00-218">応答</span><span class="sxs-lookup"><span data-stu-id="8ef00-218">Response</span></span>
<span data-ttu-id="8ef00-219">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="8ef00-219">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ef00-220">例</span><span class="sxs-lookup"><span data-stu-id="8ef00-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ef00-221">要求</span><span class="sxs-lookup"><span data-stu-id="8ef00-221">Request</span></span>
<span data-ttu-id="8ef00-222">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8ef00-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1158

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="8ef00-223">応答</span><span class="sxs-lookup"><span data-stu-id="8ef00-223">Response</span></span>
<span data-ttu-id="8ef00-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8ef00-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1330

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "3d4237b0-37b0-3d42-b037-423db037423d",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ]
}
```





