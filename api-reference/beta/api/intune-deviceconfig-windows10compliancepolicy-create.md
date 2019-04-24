---
title: windows10CompliancePolicy の作成
description: 新しい windows10CompliancePolicy オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 64649c1028a0ed7c4beca8ceb41eb683c25c8a27
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32517877"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="dfb50-103">windows10CompliancePolicy の作成</span><span class="sxs-lookup"><span data-stu-id="dfb50-103">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="dfb50-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dfb50-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfb50-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dfb50-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfb50-106">新しい [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="dfb50-106">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dfb50-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="dfb50-107">Prerequisites</span></span>
<span data-ttu-id="dfb50-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dfb50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfb50-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dfb50-110">Permission type</span></span>|<span data-ttu-id="dfb50-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dfb50-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfb50-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dfb50-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dfb50-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfb50-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dfb50-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dfb50-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfb50-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dfb50-115">Not supported.</span></span>|
|<span data-ttu-id="dfb50-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dfb50-116">Application</span></span>|<span data-ttu-id="dfb50-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dfb50-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfb50-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dfb50-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="dfb50-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dfb50-119">Request headers</span></span>
|<span data-ttu-id="dfb50-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dfb50-120">Header</span></span>|<span data-ttu-id="dfb50-121">値</span><span class="sxs-lookup"><span data-stu-id="dfb50-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfb50-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfb50-122">Authorization</span></span>|<span data-ttu-id="dfb50-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="dfb50-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfb50-124">承諾</span><span class="sxs-lookup"><span data-stu-id="dfb50-124">Accept</span></span>|<span data-ttu-id="dfb50-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dfb50-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfb50-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="dfb50-126">Request body</span></span>
<span data-ttu-id="dfb50-127">要求本文で、windows10CompliancePolicy オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dfb50-127">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="dfb50-128">次の表に、windows10CompliancePolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="dfb50-128">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="dfb50-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfb50-129">Property</span></span>|<span data-ttu-id="dfb50-130">型</span><span class="sxs-lookup"><span data-stu-id="dfb50-130">Type</span></span>|<span data-ttu-id="dfb50-131">説明</span><span class="sxs-lookup"><span data-stu-id="dfb50-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfb50-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dfb50-132">roleScopeTagIds</span></span>|<span data-ttu-id="dfb50-133">String collection</span><span class="sxs-lookup"><span data-stu-id="dfb50-133">String collection</span></span>|<span data-ttu-id="dfb50-134">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="dfb50-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dfb50-135">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfb50-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dfb50-136">id</span><span class="sxs-lookup"><span data-stu-id="dfb50-136">id</span></span>|<span data-ttu-id="dfb50-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="dfb50-137">String</span></span>|<span data-ttu-id="dfb50-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="dfb50-138">Key of the entity.</span></span> <span data-ttu-id="dfb50-139">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfb50-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dfb50-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dfb50-140">createdDateTime</span></span>|<span data-ttu-id="dfb50-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfb50-141">DateTimeOffset</span></span>|<span data-ttu-id="dfb50-142">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="dfb50-142">DateTime the object was created.</span></span> <span data-ttu-id="dfb50-143">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfb50-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dfb50-144">説明</span><span class="sxs-lookup"><span data-stu-id="dfb50-144">description</span></span>|<span data-ttu-id="dfb50-145">String</span><span class="sxs-lookup"><span data-stu-id="dfb50-145">String</span></span>|<span data-ttu-id="dfb50-146">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="dfb50-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dfb50-147">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfb50-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dfb50-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dfb50-148">lastModifiedDateTime</span></span>|<span data-ttu-id="dfb50-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfb50-149">DateTimeOffset</span></span>|<span data-ttu-id="dfb50-150">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="dfb50-150">DateTime the object was last modified.</span></span> <span data-ttu-id="dfb50-151">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfb50-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dfb50-152">displayName</span><span class="sxs-lookup"><span data-stu-id="dfb50-152">displayName</span></span>|<span data-ttu-id="dfb50-153">String</span><span class="sxs-lookup"><span data-stu-id="dfb50-153">String</span></span>|<span data-ttu-id="dfb50-154">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="dfb50-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dfb50-155">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfb50-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dfb50-156">version</span><span class="sxs-lookup"><span data-stu-id="dfb50-156">version</span></span>|<span data-ttu-id="dfb50-157">Int32</span><span class="sxs-lookup"><span data-stu-id="dfb50-157">Int32</span></span>|<span data-ttu-id="dfb50-158">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="dfb50-158">Version of the device configuration.</span></span> <span data-ttu-id="dfb50-159">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfb50-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dfb50-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="dfb50-160">passwordRequired</span></span>|<span data-ttu-id="dfb50-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb50-161">Boolean</span></span>|<span data-ttu-id="dfb50-162">Windows デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="dfb50-162">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="dfb50-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="dfb50-163">passwordBlockSimple</span></span>|<span data-ttu-id="dfb50-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb50-164">Boolean</span></span>|<span data-ttu-id="dfb50-165">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dfb50-165">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="dfb50-166">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="dfb50-166">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="dfb50-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb50-167">Boolean</span></span>|<span data-ttu-id="dfb50-168">アイドル デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="dfb50-168">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="dfb50-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="dfb50-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="dfb50-170">Int32</span><span class="sxs-lookup"><span data-stu-id="dfb50-170">Int32</span></span>|<span data-ttu-id="dfb50-171">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="dfb50-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="dfb50-172">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="dfb50-172">passwordExpirationDays</span></span>|<span data-ttu-id="dfb50-173">Int32</span><span class="sxs-lookup"><span data-stu-id="dfb50-173">Int32</span></span>|<span data-ttu-id="dfb50-174">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="dfb50-174">The password expiration in days.</span></span>|
|<span data-ttu-id="dfb50-175">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="dfb50-175">passwordMinimumLength</span></span>|<span data-ttu-id="dfb50-176">Int32</span><span class="sxs-lookup"><span data-stu-id="dfb50-176">Int32</span></span>|<span data-ttu-id="dfb50-177">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="dfb50-177">The minimum password length.</span></span>|
|<span data-ttu-id="dfb50-178">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="dfb50-178">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="dfb50-179">Int32</span><span class="sxs-lookup"><span data-stu-id="dfb50-179">Int32</span></span>|<span data-ttu-id="dfb50-180">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="dfb50-180">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="dfb50-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="dfb50-181">passwordRequiredType</span></span>|[<span data-ttu-id="dfb50-182">requiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="dfb50-182">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="dfb50-183">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="dfb50-183">The required password type.</span></span> <span data-ttu-id="dfb50-184">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="dfb50-184">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="dfb50-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="dfb50-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="dfb50-186">Int32</span><span class="sxs-lookup"><span data-stu-id="dfb50-186">Int32</span></span>|<span data-ttu-id="dfb50-187">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="dfb50-187">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="dfb50-188">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="dfb50-188">requireHealthyDeviceReport</span></span>|<span data-ttu-id="dfb50-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb50-189">Boolean</span></span>|<span data-ttu-id="dfb50-190">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="dfb50-190">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="dfb50-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="dfb50-191">osMinimumVersion</span></span>|<span data-ttu-id="dfb50-192">String</span><span class="sxs-lookup"><span data-stu-id="dfb50-192">String</span></span>|<span data-ttu-id="dfb50-193">Windows 10 の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="dfb50-193">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="dfb50-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="dfb50-194">osMaximumVersion</span></span>|<span data-ttu-id="dfb50-195">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="dfb50-195">String</span></span>|<span data-ttu-id="dfb50-196">Windows 10 の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="dfb50-196">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="dfb50-197">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="dfb50-197">mobileOsMinimumVersion</span></span>|<span data-ttu-id="dfb50-198">String</span><span class="sxs-lookup"><span data-stu-id="dfb50-198">String</span></span>|<span data-ttu-id="dfb50-199">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="dfb50-199">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="dfb50-200">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="dfb50-200">mobileOsMaximumVersion</span></span>|<span data-ttu-id="dfb50-201">String</span><span class="sxs-lookup"><span data-stu-id="dfb50-201">String</span></span>|<span data-ttu-id="dfb50-202">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="dfb50-202">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="dfb50-203">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="dfb50-203">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="dfb50-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb50-204">Boolean</span></span>|<span data-ttu-id="dfb50-205">デバイスが Windows デバイス正常性構成証明によって正常と報告される (早期起動マルウェア対策ドライバーが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="dfb50-205">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="dfb50-206">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="dfb50-206">bitLockerEnabled</span></span>|<span data-ttu-id="dfb50-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb50-207">Boolean</span></span>|<span data-ttu-id="dfb50-208">デバイスが Windows デバイス正常性構成証明によって正常と報告される (BitLocker が有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="dfb50-208">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="dfb50-209">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="dfb50-209">secureBootEnabled</span></span>|<span data-ttu-id="dfb50-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb50-210">Boolean</span></span>|<span data-ttu-id="dfb50-211">デバイスが Windows デバイス正常性構成証明によって正常と報告される (セキュア ブートが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="dfb50-211">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="dfb50-212">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="dfb50-212">codeIntegrityEnabled</span></span>|<span data-ttu-id="dfb50-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb50-213">Boolean</span></span>|<span data-ttu-id="dfb50-214">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="dfb50-214">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="dfb50-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="dfb50-215">storageRequireEncryption</span></span>|<span data-ttu-id="dfb50-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb50-216">Boolean</span></span>|<span data-ttu-id="dfb50-217">Windows デバイス上での暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="dfb50-217">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="dfb50-218">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="dfb50-218">activeFirewallRequired</span></span>|<span data-ttu-id="dfb50-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb50-219">Boolean</span></span>|<span data-ttu-id="dfb50-220">Windows デバイスでアクティブなファイアウォールが必要です。</span><span class="sxs-lookup"><span data-stu-id="dfb50-220">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="dfb50-221">defenderenabled</span><span class="sxs-lookup"><span data-stu-id="dfb50-221">defenderEnabled</span></span>|<span data-ttu-id="dfb50-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb50-222">Boolean</span></span>|<span data-ttu-id="dfb50-223">windows デバイスで windows Defender マルウェア対策を必須にする。</span><span class="sxs-lookup"><span data-stu-id="dfb50-223">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="dfb50-224">defenderversion</span><span class="sxs-lookup"><span data-stu-id="dfb50-224">defenderVersion</span></span>|<span data-ttu-id="dfb50-225">String</span><span class="sxs-lookup"><span data-stu-id="dfb50-225">String</span></span>|<span data-ttu-id="dfb50-226">windows デバイスで windows Defender マルウェア対策の最小バージョンが必要です。</span><span class="sxs-lookup"><span data-stu-id="dfb50-226">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="dfb50-227">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="dfb50-227">signatureOutOfDate</span></span>|<span data-ttu-id="dfb50-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb50-228">Boolean</span></span>|<span data-ttu-id="dfb50-229">windows デバイスで windows Defender マルウェア対策の署名が最新の状態になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="dfb50-229">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="dfb50-230">rtpenabled</span><span class="sxs-lookup"><span data-stu-id="dfb50-230">rtpEnabled</span></span>|<span data-ttu-id="dfb50-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb50-231">Boolean</span></span>|<span data-ttu-id="dfb50-232">windows デバイスで windows Defender マルウェア対策のリアルタイム保護を必要とします。</span><span class="sxs-lookup"><span data-stu-id="dfb50-232">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="dfb50-233">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="dfb50-233">antivirusRequired</span></span>|<span data-ttu-id="dfb50-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb50-234">Boolean</span></span>|<span data-ttu-id="dfb50-235">windows Decurity Center に登録されているウイルス対策ソリューション (Symantec、Windows Defender など) を必要とします。</span><span class="sxs-lookup"><span data-stu-id="dfb50-235">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="dfb50-236">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="dfb50-236">antiSpywareRequired</span></span>|<span data-ttu-id="dfb50-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb50-237">Boolean</span></span>|<span data-ttu-id="dfb50-238">windows Decurity Center に登録されているスパイウェア対策ソリューションで、オンおよび監視する必要があります (Symantec、Windows Defender など)。</span><span class="sxs-lookup"><span data-stu-id="dfb50-238">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="dfb50-239">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="dfb50-239">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="dfb50-240">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="dfb50-240">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="dfb50-241">Windows デバイス上の有効なオペレーティングシステムのビルド範囲。</span><span class="sxs-lookup"><span data-stu-id="dfb50-241">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="dfb50-242">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="dfb50-242">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="dfb50-243">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="dfb50-243">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="dfb50-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb50-244">Boolean</span></span>|<span data-ttu-id="dfb50-245">デバイスの脅威保護が有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="dfb50-245">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="dfb50-246">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="dfb50-246">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="dfb50-247">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="dfb50-247">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="dfb50-248">デバイスの脅威保護で、コンプライアンス違反を報告するために最低限必要となるリスクレベル。</span><span class="sxs-lookup"><span data-stu-id="dfb50-248">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="dfb50-249">可能な値は `unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="dfb50-249">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="dfb50-250">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="dfb50-250">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="dfb50-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb50-251">Boolean</span></span>|<span data-ttu-id="dfb50-252">Intune コンプライアンスの状態を考慮に入れて SCCM コンプライアンスの状態を考慮する必要があります。</span><span class="sxs-lookup"><span data-stu-id="dfb50-252">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|



## <a name="response"></a><span data-ttu-id="dfb50-253">応答</span><span class="sxs-lookup"><span data-stu-id="dfb50-253">Response</span></span>
<span data-ttu-id="dfb50-254">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dfb50-254">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfb50-255">例</span><span class="sxs-lookup"><span data-stu-id="dfb50-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfb50-256">要求</span><span class="sxs-lookup"><span data-stu-id="dfb50-256">Request</span></span>
<span data-ttu-id="dfb50-257">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dfb50-257">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1666

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true
}
```

### <a name="response"></a><span data-ttu-id="dfb50-258">応答</span><span class="sxs-lookup"><span data-stu-id="dfb50-258">Response</span></span>
<span data-ttu-id="dfb50-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dfb50-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1838

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "2919ae62-ae62-2919-62ae-192962ae1929",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true
}
```





