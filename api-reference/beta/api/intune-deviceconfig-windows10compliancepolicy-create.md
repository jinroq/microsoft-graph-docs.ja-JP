---
title: windows10CompliancePolicy の作成
description: 新しい windows10CompliancePolicy オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 50d1230a6e1580008e501745f9c7918da5031187
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360915"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="41f94-103">windows10CompliancePolicy の作成</span><span class="sxs-lookup"><span data-stu-id="41f94-103">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="41f94-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="41f94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41f94-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41f94-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="41f94-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="41f94-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41f94-107">新しい [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="41f94-107">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="41f94-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="41f94-108">Prerequisites</span></span>
<span data-ttu-id="41f94-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41f94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41f94-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="41f94-111">Permission type</span></span>|<span data-ttu-id="41f94-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="41f94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41f94-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="41f94-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41f94-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41f94-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41f94-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="41f94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41f94-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41f94-116">Not supported.</span></span>|
|<span data-ttu-id="41f94-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="41f94-117">Application</span></span>|<span data-ttu-id="41f94-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41f94-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41f94-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="41f94-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="41f94-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41f94-120">Request headers</span></span>
|<span data-ttu-id="41f94-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41f94-121">Header</span></span>|<span data-ttu-id="41f94-122">値</span><span class="sxs-lookup"><span data-stu-id="41f94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41f94-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="41f94-123">Authorization</span></span>|<span data-ttu-id="41f94-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="41f94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41f94-125">Accept</span><span class="sxs-lookup"><span data-stu-id="41f94-125">Accept</span></span>|<span data-ttu-id="41f94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41f94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41f94-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="41f94-127">Request body</span></span>
<span data-ttu-id="41f94-128">要求本文で、windows10CompliancePolicy オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="41f94-128">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="41f94-129">次の表に、windows10CompliancePolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="41f94-129">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="41f94-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41f94-130">Property</span></span>|<span data-ttu-id="41f94-131">種類</span><span class="sxs-lookup"><span data-stu-id="41f94-131">Type</span></span>|<span data-ttu-id="41f94-132">説明</span><span class="sxs-lookup"><span data-stu-id="41f94-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41f94-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="41f94-133">roleScopeTagIds</span></span>|<span data-ttu-id="41f94-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="41f94-134">String collection</span></span>|<span data-ttu-id="41f94-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="41f94-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="41f94-136">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="41f94-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="41f94-137">id</span><span class="sxs-lookup"><span data-stu-id="41f94-137">id</span></span>|<span data-ttu-id="41f94-138">String</span><span class="sxs-lookup"><span data-stu-id="41f94-138">String</span></span>|<span data-ttu-id="41f94-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="41f94-139">Key of the entity.</span></span> <span data-ttu-id="41f94-140">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="41f94-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="41f94-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41f94-141">createdDateTime</span></span>|<span data-ttu-id="41f94-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41f94-142">DateTimeOffset</span></span>|<span data-ttu-id="41f94-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="41f94-143">DateTime the object was created.</span></span> <span data-ttu-id="41f94-144">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="41f94-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="41f94-145">説明</span><span class="sxs-lookup"><span data-stu-id="41f94-145">description</span></span>|<span data-ttu-id="41f94-146">String</span><span class="sxs-lookup"><span data-stu-id="41f94-146">String</span></span>|<span data-ttu-id="41f94-147">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="41f94-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="41f94-148">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="41f94-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="41f94-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41f94-149">lastModifiedDateTime</span></span>|<span data-ttu-id="41f94-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41f94-150">DateTimeOffset</span></span>|<span data-ttu-id="41f94-151">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="41f94-151">DateTime the object was last modified.</span></span> <span data-ttu-id="41f94-152">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="41f94-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="41f94-153">displayName</span><span class="sxs-lookup"><span data-stu-id="41f94-153">displayName</span></span>|<span data-ttu-id="41f94-154">String</span><span class="sxs-lookup"><span data-stu-id="41f94-154">String</span></span>|<span data-ttu-id="41f94-155">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="41f94-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="41f94-156">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="41f94-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="41f94-157">version</span><span class="sxs-lookup"><span data-stu-id="41f94-157">version</span></span>|<span data-ttu-id="41f94-158">Int32</span><span class="sxs-lookup"><span data-stu-id="41f94-158">Int32</span></span>|<span data-ttu-id="41f94-159">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="41f94-159">Version of the device configuration.</span></span> <span data-ttu-id="41f94-160">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="41f94-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="41f94-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="41f94-161">passwordRequired</span></span>|<span data-ttu-id="41f94-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="41f94-162">Boolean</span></span>|<span data-ttu-id="41f94-163">Windows デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="41f94-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="41f94-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="41f94-164">passwordBlockSimple</span></span>|<span data-ttu-id="41f94-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="41f94-165">Boolean</span></span>|<span data-ttu-id="41f94-166">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="41f94-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="41f94-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="41f94-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="41f94-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="41f94-168">Boolean</span></span>|<span data-ttu-id="41f94-169">アイドル デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="41f94-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="41f94-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="41f94-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="41f94-171">Int32</span><span class="sxs-lookup"><span data-stu-id="41f94-171">Int32</span></span>|<span data-ttu-id="41f94-172">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="41f94-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="41f94-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="41f94-173">passwordExpirationDays</span></span>|<span data-ttu-id="41f94-174">Int32</span><span class="sxs-lookup"><span data-stu-id="41f94-174">Int32</span></span>|<span data-ttu-id="41f94-175">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="41f94-175">The password expiration in days.</span></span>|
|<span data-ttu-id="41f94-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="41f94-176">passwordMinimumLength</span></span>|<span data-ttu-id="41f94-177">Int32</span><span class="sxs-lookup"><span data-stu-id="41f94-177">Int32</span></span>|<span data-ttu-id="41f94-178">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="41f94-178">The minimum password length.</span></span>|
|<span data-ttu-id="41f94-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="41f94-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="41f94-180">Int32</span><span class="sxs-lookup"><span data-stu-id="41f94-180">Int32</span></span>|<span data-ttu-id="41f94-181">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="41f94-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="41f94-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="41f94-182">passwordRequiredType</span></span>|[<span data-ttu-id="41f94-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="41f94-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="41f94-184">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="41f94-184">The required password type.</span></span> <span data-ttu-id="41f94-185">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="41f94-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="41f94-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="41f94-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="41f94-187">Int32</span><span class="sxs-lookup"><span data-stu-id="41f94-187">Int32</span></span>|<span data-ttu-id="41f94-188">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="41f94-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="41f94-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="41f94-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="41f94-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="41f94-190">Boolean</span></span>|<span data-ttu-id="41f94-191">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="41f94-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="41f94-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="41f94-192">osMinimumVersion</span></span>|<span data-ttu-id="41f94-193">String</span><span class="sxs-lookup"><span data-stu-id="41f94-193">String</span></span>|<span data-ttu-id="41f94-194">Windows 10 の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="41f94-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="41f94-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="41f94-195">osMaximumVersion</span></span>|<span data-ttu-id="41f94-196">String</span><span class="sxs-lookup"><span data-stu-id="41f94-196">String</span></span>|<span data-ttu-id="41f94-197">Windows 10 の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="41f94-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="41f94-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="41f94-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="41f94-199">String</span><span class="sxs-lookup"><span data-stu-id="41f94-199">String</span></span>|<span data-ttu-id="41f94-200">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="41f94-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="41f94-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="41f94-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="41f94-202">String</span><span class="sxs-lookup"><span data-stu-id="41f94-202">String</span></span>|<span data-ttu-id="41f94-203">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="41f94-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="41f94-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="41f94-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="41f94-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="41f94-205">Boolean</span></span>|<span data-ttu-id="41f94-206">デバイスが Windows デバイス正常性構成証明によって正常と報告される (早期起動マルウェア対策ドライバーが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="41f94-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="41f94-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="41f94-207">bitLockerEnabled</span></span>|<span data-ttu-id="41f94-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="41f94-208">Boolean</span></span>|<span data-ttu-id="41f94-209">デバイスが Windows デバイス正常性構成証明によって正常と報告される (BitLocker が有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="41f94-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="41f94-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="41f94-210">secureBootEnabled</span></span>|<span data-ttu-id="41f94-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="41f94-211">Boolean</span></span>|<span data-ttu-id="41f94-212">デバイスが Windows デバイス正常性構成証明によって正常と報告される (セキュア ブートが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="41f94-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="41f94-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="41f94-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="41f94-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="41f94-214">Boolean</span></span>|<span data-ttu-id="41f94-215">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="41f94-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="41f94-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="41f94-216">storageRequireEncryption</span></span>|<span data-ttu-id="41f94-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="41f94-217">Boolean</span></span>|<span data-ttu-id="41f94-218">Windows デバイス上での暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="41f94-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="41f94-219">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="41f94-219">activeFirewallRequired</span></span>|<span data-ttu-id="41f94-220">ブール型</span><span class="sxs-lookup"><span data-stu-id="41f94-220">Boolean</span></span>|<span data-ttu-id="41f94-221">Windows デバイス上のアクティブなファイアウォールが必要です。</span><span class="sxs-lookup"><span data-stu-id="41f94-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="41f94-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="41f94-222">defenderEnabled</span></span>|<span data-ttu-id="41f94-223">ブール型</span><span class="sxs-lookup"><span data-stu-id="41f94-223">Boolean</span></span>|<span data-ttu-id="41f94-224">Windows デバイスで Windows Defender のウイルス対策が必要です。</span><span class="sxs-lookup"><span data-stu-id="41f94-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="41f94-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="41f94-225">defenderVersion</span></span>|<span data-ttu-id="41f94-226">String</span><span class="sxs-lookup"><span data-stu-id="41f94-226">String</span></span>|<span data-ttu-id="41f94-227">Windows デバイスの最小バージョンの Windows Defender のウイルス対策が必要です。</span><span class="sxs-lookup"><span data-stu-id="41f94-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="41f94-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="41f94-228">signatureOutOfDate</span></span>|<span data-ttu-id="41f94-229">ブール型</span><span class="sxs-lookup"><span data-stu-id="41f94-229">Boolean</span></span>|<span data-ttu-id="41f94-230">Windows デバイスで最新のものに、Windows Defender のウイルス対策署名が必要です。</span><span class="sxs-lookup"><span data-stu-id="41f94-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="41f94-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="41f94-231">rtpEnabled</span></span>|<span data-ttu-id="41f94-232">ブール型</span><span class="sxs-lookup"><span data-stu-id="41f94-232">Boolean</span></span>|<span data-ttu-id="41f94-233">Windows デバイスでは、Windows Defender のウイルス対策のリアルタイム保護を必要とします。</span><span class="sxs-lookup"><span data-stu-id="41f94-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="41f94-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="41f94-234">antivirusRequired</span></span>|<span data-ttu-id="41f94-235">ブール型</span><span class="sxs-lookup"><span data-stu-id="41f94-235">Boolean</span></span>|<span data-ttu-id="41f94-236">上にある Windows セキュリティ センターに登録され、(例: シマンテック、Windows Defender) を監視するウイルス対策ソリューションが必要です。</span><span class="sxs-lookup"><span data-stu-id="41f94-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="41f94-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="41f94-237">antiSpywareRequired</span></span>|<span data-ttu-id="41f94-238">ブール型</span><span class="sxs-lookup"><span data-stu-id="41f94-238">Boolean</span></span>|<span data-ttu-id="41f94-239">任意のウイルス対策ソリューションに Windows セキュリティ センターに登録され、監視 (シマンテック、Windows Defender など) が必要です。</span><span class="sxs-lookup"><span data-stu-id="41f94-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="41f94-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="41f94-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="41f94-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="41f94-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="41f94-242">有効なオペレーティング システムは、Windows デバイス上の範囲を作成します。</span><span class="sxs-lookup"><span data-stu-id="41f94-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="41f94-243">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="41f94-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="41f94-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="41f94-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="41f94-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="41f94-245">Boolean</span></span>|<span data-ttu-id="41f94-246">デバイスの脅威保護が有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="41f94-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="41f94-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="41f94-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="41f94-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="41f94-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="41f94-249">法令遵守の不履行を報告する最小のリスク レベルの脅威のデバイスの保護を必要とします。</span><span class="sxs-lookup"><span data-stu-id="41f94-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="41f94-250">使用可能な値: `unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="41f94-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="41f94-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="41f94-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="41f94-252">ブール型</span><span class="sxs-lookup"><span data-stu-id="41f94-252">Boolean</span></span>|<span data-ttu-id="41f94-253">Intune 準拠状態の考慮事項に SCCM の準拠状態を考慮する必要があります。</span><span class="sxs-lookup"><span data-stu-id="41f94-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|



## <a name="response"></a><span data-ttu-id="41f94-254">応答</span><span class="sxs-lookup"><span data-stu-id="41f94-254">Response</span></span>
<span data-ttu-id="41f94-255">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="41f94-255">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41f94-256">例</span><span class="sxs-lookup"><span data-stu-id="41f94-256">Example</span></span>
### <a name="request"></a><span data-ttu-id="41f94-257">要求</span><span class="sxs-lookup"><span data-stu-id="41f94-257">Request</span></span>
<span data-ttu-id="41f94-258">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="41f94-258">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1730

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="41f94-259">応答</span><span class="sxs-lookup"><span data-stu-id="41f94-259">Response</span></span>
<span data-ttu-id="41f94-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="41f94-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




