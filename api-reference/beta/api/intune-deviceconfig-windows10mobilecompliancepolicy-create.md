---
title: Create windows10MobileCompliancePolicy
description: 新しい windows10MobileCompliancePolicy オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c252ece92661c2b57c8d8c7ea6c1b714a9bb9594
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797558"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="a2b2a-103">Create windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a2b2a-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="a2b2a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2b2a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2b2a-106">新しい [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-106">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2b2a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a2b2a-107">Prerequisites</span></span>
<span data-ttu-id="a2b2a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2b2a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a2b2a-110">Permission type</span></span>|<span data-ttu-id="a2b2a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a2b2a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2b2a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a2b2a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2b2a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2b2a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2b2a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2b2a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2b2a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-115">Not supported.</span></span>|
|<span data-ttu-id="a2b2a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a2b2a-116">Application</span></span>|<span data-ttu-id="a2b2a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2b2a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2b2a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="a2b2a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2b2a-119">Request headers</span></span>
|<span data-ttu-id="a2b2a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2b2a-120">Header</span></span>|<span data-ttu-id="a2b2a-121">値</span><span class="sxs-lookup"><span data-stu-id="a2b2a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2b2a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2b2a-122">Authorization</span></span>|<span data-ttu-id="a2b2a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2b2a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a2b2a-124">Accept</span></span>|<span data-ttu-id="a2b2a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a2b2a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2b2a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a2b2a-126">Request body</span></span>
<span data-ttu-id="a2b2a-127">要求本文で、windows10MobileCompliancePolicy オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-127">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="a2b2a-128">次の表に、windows10MobileCompliancePolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-128">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="a2b2a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2b2a-129">Property</span></span>|<span data-ttu-id="a2b2a-130">型</span><span class="sxs-lookup"><span data-stu-id="a2b2a-130">Type</span></span>|<span data-ttu-id="a2b2a-131">説明</span><span class="sxs-lookup"><span data-stu-id="a2b2a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2b2a-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a2b2a-132">roleScopeTagIds</span></span>|<span data-ttu-id="a2b2a-133">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a2b2a-133">String collection</span></span>|<span data-ttu-id="a2b2a-134">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a2b2a-135">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a2b2a-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2b2a-136">id</span><span class="sxs-lookup"><span data-stu-id="a2b2a-136">id</span></span>|<span data-ttu-id="a2b2a-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a2b2a-137">String</span></span>|<span data-ttu-id="a2b2a-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-138">Key of the entity.</span></span> <span data-ttu-id="a2b2a-139">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a2b2a-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2b2a-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2b2a-140">createdDateTime</span></span>|<span data-ttu-id="a2b2a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2b2a-141">DateTimeOffset</span></span>|<span data-ttu-id="a2b2a-142">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-142">DateTime the object was created.</span></span> <span data-ttu-id="a2b2a-143">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a2b2a-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2b2a-144">説明</span><span class="sxs-lookup"><span data-stu-id="a2b2a-144">description</span></span>|<span data-ttu-id="a2b2a-145">String</span><span class="sxs-lookup"><span data-stu-id="a2b2a-145">String</span></span>|<span data-ttu-id="a2b2a-146">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a2b2a-147">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a2b2a-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2b2a-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2b2a-148">lastModifiedDateTime</span></span>|<span data-ttu-id="a2b2a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2b2a-149">DateTimeOffset</span></span>|<span data-ttu-id="a2b2a-150">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-150">DateTime the object was last modified.</span></span> <span data-ttu-id="a2b2a-151">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a2b2a-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2b2a-152">displayName</span><span class="sxs-lookup"><span data-stu-id="a2b2a-152">displayName</span></span>|<span data-ttu-id="a2b2a-153">String</span><span class="sxs-lookup"><span data-stu-id="a2b2a-153">String</span></span>|<span data-ttu-id="a2b2a-154">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a2b2a-155">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a2b2a-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2b2a-156">version</span><span class="sxs-lookup"><span data-stu-id="a2b2a-156">version</span></span>|<span data-ttu-id="a2b2a-157">Int32</span><span class="sxs-lookup"><span data-stu-id="a2b2a-157">Int32</span></span>|<span data-ttu-id="a2b2a-158">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-158">Version of the device configuration.</span></span> <span data-ttu-id="a2b2a-159">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a2b2a-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2b2a-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="a2b2a-160">passwordRequired</span></span>|<span data-ttu-id="a2b2a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2b2a-161">Boolean</span></span>|<span data-ttu-id="a2b2a-162">Windows Phone デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-162">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="a2b2a-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="a2b2a-163">passwordBlockSimple</span></span>|<span data-ttu-id="a2b2a-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2b2a-164">Boolean</span></span>|<span data-ttu-id="a2b2a-165">カレンダーの同期を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-165">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="a2b2a-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a2b2a-166">passwordMinimumLength</span></span>|<span data-ttu-id="a2b2a-167">Int32</span><span class="sxs-lookup"><span data-stu-id="a2b2a-167">Int32</span></span>|<span data-ttu-id="a2b2a-168">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-168">Minimum password length.</span></span> <span data-ttu-id="a2b2a-169">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="a2b2a-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a2b2a-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="a2b2a-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="a2b2a-171">Int32</span><span class="sxs-lookup"><span data-stu-id="a2b2a-171">Int32</span></span>|<span data-ttu-id="a2b2a-172">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="a2b2a-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a2b2a-173">passwordRequiredType</span></span>|[<span data-ttu-id="a2b2a-174">requiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="a2b2a-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="a2b2a-175">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-175">The required password type.</span></span> <span data-ttu-id="a2b2a-176">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="a2b2a-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a2b2a-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a2b2a-178">Int32</span><span class="sxs-lookup"><span data-stu-id="a2b2a-178">Int32</span></span>|<span data-ttu-id="a2b2a-179">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-179">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="a2b2a-180">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a2b2a-180">passwordExpirationDays</span></span>|<span data-ttu-id="a2b2a-181">Int32</span><span class="sxs-lookup"><span data-stu-id="a2b2a-181">Int32</span></span>|<span data-ttu-id="a2b2a-182">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-182">Number of days before password expiration.</span></span> <span data-ttu-id="a2b2a-183">有効な値は 1 から 255 までです</span><span class="sxs-lookup"><span data-stu-id="a2b2a-183">Valid values 1 to 255</span></span>|
|<span data-ttu-id="a2b2a-184">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="a2b2a-184">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="a2b2a-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a2b2a-185">Int32</span></span>|<span data-ttu-id="a2b2a-186">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-186">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="a2b2a-187">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="a2b2a-187">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="a2b2a-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2b2a-188">Boolean</span></span>|<span data-ttu-id="a2b2a-189">アイドル デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-189">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="a2b2a-190">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="a2b2a-190">osMinimumVersion</span></span>|<span data-ttu-id="a2b2a-191">文字列</span><span class="sxs-lookup"><span data-stu-id="a2b2a-191">String</span></span>|<span data-ttu-id="a2b2a-192">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="a2b2a-193">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="a2b2a-193">osMaximumVersion</span></span>|<span data-ttu-id="a2b2a-194">String</span><span class="sxs-lookup"><span data-stu-id="a2b2a-194">String</span></span>|<span data-ttu-id="a2b2a-195">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="a2b2a-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="a2b2a-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="a2b2a-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2b2a-197">Boolean</span></span>|<span data-ttu-id="a2b2a-198">デバイスが Windows デバイス正常性構成証明によって正常と報告される (早期起動マルウェア対策ドライバーが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="a2b2a-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="a2b2a-199">bitLockerEnabled</span></span>|<span data-ttu-id="a2b2a-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2b2a-200">Boolean</span></span>|<span data-ttu-id="a2b2a-201">デバイスが Windows デバイス正常性構成証明によって正常と報告される (BitLocker が有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="a2b2a-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="a2b2a-202">secureBootEnabled</span></span>|<span data-ttu-id="a2b2a-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2b2a-203">Boolean</span></span>|<span data-ttu-id="a2b2a-204">デバイスが Windows デバイス正常性構成証明によって正常と報告される (セキュア ブートが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="a2b2a-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="a2b2a-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="a2b2a-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2b2a-206">Boolean</span></span>|<span data-ttu-id="a2b2a-207">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="a2b2a-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="a2b2a-208">storageRequireEncryption</span></span>|<span data-ttu-id="a2b2a-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2b2a-209">Boolean</span></span>|<span data-ttu-id="a2b2a-210">Windows デバイス上での暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-210">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="a2b2a-211">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="a2b2a-211">activeFirewallRequired</span></span>|<span data-ttu-id="a2b2a-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2b2a-212">Boolean</span></span>|<span data-ttu-id="a2b2a-213">Windows デバイスでアクティブなファイアウォールが必要です。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-213">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="a2b2a-214">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="a2b2a-214">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="a2b2a-215">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a2b2a-215">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="a2b2a-216">Windows デバイス上の有効なオペレーティングシステムのビルド範囲。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-216">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="a2b2a-217">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-217">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="a2b2a-218">応答</span><span class="sxs-lookup"><span data-stu-id="a2b2a-218">Response</span></span>
<span data-ttu-id="a2b2a-219">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-219">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2b2a-220">例</span><span class="sxs-lookup"><span data-stu-id="a2b2a-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2b2a-221">要求</span><span class="sxs-lookup"><span data-stu-id="a2b2a-221">Request</span></span>
<span data-ttu-id="a2b2a-222">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="a2b2a-223">応答</span><span class="sxs-lookup"><span data-stu-id="a2b2a-223">Response</span></span>
<span data-ttu-id="a2b2a-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a2b2a-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





