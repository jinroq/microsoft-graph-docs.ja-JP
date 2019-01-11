---
title: windows10MobileCompliancePolicy の更新
description: windows10MobileCompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3956af618a5d6ed52e5385a0d09b4326ac9ef367
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849449"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="c3b44-103">windows10MobileCompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="c3b44-103">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="c3b44-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c3b44-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3b44-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3b44-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3b44-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3b44-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3b44-107">[windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c3b44-107">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c3b44-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c3b44-108">Prerequisites</span></span>
<span data-ttu-id="c3b44-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3b44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3b44-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3b44-111">Permission type</span></span>|<span data-ttu-id="c3b44-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3b44-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3b44-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3b44-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3b44-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3b44-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c3b44-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3b44-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3b44-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3b44-116">Not supported.</span></span>|
|<span data-ttu-id="c3b44-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3b44-117">Application</span></span>|<span data-ttu-id="c3b44-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3b44-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3b44-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3b44-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="c3b44-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3b44-120">Request headers</span></span>
|<span data-ttu-id="c3b44-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3b44-121">Header</span></span>|<span data-ttu-id="c3b44-122">値</span><span class="sxs-lookup"><span data-stu-id="c3b44-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3b44-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3b44-123">Authorization</span></span>|<span data-ttu-id="c3b44-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c3b44-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3b44-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c3b44-125">Accept</span></span>|<span data-ttu-id="c3b44-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3b44-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3b44-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3b44-127">Request body</span></span>
<span data-ttu-id="c3b44-128">要求本文で、[windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c3b44-128">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="c3b44-129">次の表に、[windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c3b44-129">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="c3b44-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3b44-130">Property</span></span>|<span data-ttu-id="c3b44-131">種類</span><span class="sxs-lookup"><span data-stu-id="c3b44-131">Type</span></span>|<span data-ttu-id="c3b44-132">説明</span><span class="sxs-lookup"><span data-stu-id="c3b44-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3b44-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c3b44-133">roleScopeTagIds</span></span>|<span data-ttu-id="c3b44-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c3b44-134">String collection</span></span>|<span data-ttu-id="c3b44-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="c3b44-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c3b44-136">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3b44-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c3b44-137">id</span><span class="sxs-lookup"><span data-stu-id="c3b44-137">id</span></span>|<span data-ttu-id="c3b44-138">String</span><span class="sxs-lookup"><span data-stu-id="c3b44-138">String</span></span>|<span data-ttu-id="c3b44-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c3b44-139">Key of the entity.</span></span> <span data-ttu-id="c3b44-140">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3b44-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c3b44-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3b44-141">createdDateTime</span></span>|<span data-ttu-id="c3b44-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3b44-142">DateTimeOffset</span></span>|<span data-ttu-id="c3b44-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c3b44-143">DateTime the object was created.</span></span> <span data-ttu-id="c3b44-144">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3b44-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c3b44-145">説明</span><span class="sxs-lookup"><span data-stu-id="c3b44-145">description</span></span>|<span data-ttu-id="c3b44-146">String</span><span class="sxs-lookup"><span data-stu-id="c3b44-146">String</span></span>|<span data-ttu-id="c3b44-147">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="c3b44-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c3b44-148">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3b44-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c3b44-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3b44-149">lastModifiedDateTime</span></span>|<span data-ttu-id="c3b44-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3b44-150">DateTimeOffset</span></span>|<span data-ttu-id="c3b44-151">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c3b44-151">DateTime the object was last modified.</span></span> <span data-ttu-id="c3b44-152">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3b44-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c3b44-153">displayName</span><span class="sxs-lookup"><span data-stu-id="c3b44-153">displayName</span></span>|<span data-ttu-id="c3b44-154">String</span><span class="sxs-lookup"><span data-stu-id="c3b44-154">String</span></span>|<span data-ttu-id="c3b44-155">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="c3b44-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c3b44-156">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3b44-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c3b44-157">version</span><span class="sxs-lookup"><span data-stu-id="c3b44-157">version</span></span>|<span data-ttu-id="c3b44-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c3b44-158">Int32</span></span>|<span data-ttu-id="c3b44-159">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="c3b44-159">Version of the device configuration.</span></span> <span data-ttu-id="c3b44-160">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3b44-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c3b44-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c3b44-161">passwordRequired</span></span>|<span data-ttu-id="c3b44-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3b44-162">Boolean</span></span>|<span data-ttu-id="c3b44-163">Windows Phone デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="c3b44-163">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="c3b44-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c3b44-164">passwordBlockSimple</span></span>|<span data-ttu-id="c3b44-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3b44-165">Boolean</span></span>|<span data-ttu-id="c3b44-166">カレンダーの同期を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c3b44-166">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="c3b44-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c3b44-167">passwordMinimumLength</span></span>|<span data-ttu-id="c3b44-168">Int32</span><span class="sxs-lookup"><span data-stu-id="c3b44-168">Int32</span></span>|<span data-ttu-id="c3b44-169">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="c3b44-169">Minimum password length.</span></span> <span data-ttu-id="c3b44-170">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="c3b44-170">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c3b44-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c3b44-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="c3b44-172">Int32</span><span class="sxs-lookup"><span data-stu-id="c3b44-172">Int32</span></span>|<span data-ttu-id="c3b44-173">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="c3b44-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="c3b44-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c3b44-174">passwordRequiredType</span></span>|[<span data-ttu-id="c3b44-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c3b44-175">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c3b44-176">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="c3b44-176">The required password type.</span></span> <span data-ttu-id="c3b44-177">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="c3b44-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c3b44-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c3b44-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c3b44-179">Int32</span><span class="sxs-lookup"><span data-stu-id="c3b44-179">Int32</span></span>|<span data-ttu-id="c3b44-180">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="c3b44-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="c3b44-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c3b44-181">passwordExpirationDays</span></span>|<span data-ttu-id="c3b44-182">Int32</span><span class="sxs-lookup"><span data-stu-id="c3b44-182">Int32</span></span>|<span data-ttu-id="c3b44-183">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="c3b44-183">Number of days before password expiration.</span></span> <span data-ttu-id="c3b44-184">有効な値は 1 から 255 までです</span><span class="sxs-lookup"><span data-stu-id="c3b44-184">Valid values 1 to 255</span></span>|
|<span data-ttu-id="c3b44-185">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c3b44-185">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c3b44-186">Int32</span><span class="sxs-lookup"><span data-stu-id="c3b44-186">Int32</span></span>|<span data-ttu-id="c3b44-187">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="c3b44-187">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="c3b44-188">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="c3b44-188">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="c3b44-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3b44-189">Boolean</span></span>|<span data-ttu-id="c3b44-190">アイドル デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="c3b44-190">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="c3b44-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c3b44-191">osMinimumVersion</span></span>|<span data-ttu-id="c3b44-192">String</span><span class="sxs-lookup"><span data-stu-id="c3b44-192">String</span></span>|<span data-ttu-id="c3b44-193">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="c3b44-193">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="c3b44-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c3b44-194">osMaximumVersion</span></span>|<span data-ttu-id="c3b44-195">String</span><span class="sxs-lookup"><span data-stu-id="c3b44-195">String</span></span>|<span data-ttu-id="c3b44-196">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="c3b44-196">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="c3b44-197">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="c3b44-197">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="c3b44-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3b44-198">Boolean</span></span>|<span data-ttu-id="c3b44-199">デバイスが Windows デバイス正常性構成証明によって正常と報告される (早期起動マルウェア対策ドライバーが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="c3b44-199">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="c3b44-200">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="c3b44-200">bitLockerEnabled</span></span>|<span data-ttu-id="c3b44-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3b44-201">Boolean</span></span>|<span data-ttu-id="c3b44-202">デバイスが Windows デバイス正常性構成証明によって正常と報告される (BitLocker が有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="c3b44-202">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="c3b44-203">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="c3b44-203">secureBootEnabled</span></span>|<span data-ttu-id="c3b44-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3b44-204">Boolean</span></span>|<span data-ttu-id="c3b44-205">デバイスが Windows デバイス正常性構成証明によって正常と報告される (セキュア ブートが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="c3b44-205">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="c3b44-206">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="c3b44-206">codeIntegrityEnabled</span></span>|<span data-ttu-id="c3b44-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3b44-207">Boolean</span></span>|<span data-ttu-id="c3b44-208">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="c3b44-208">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="c3b44-209">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="c3b44-209">storageRequireEncryption</span></span>|<span data-ttu-id="c3b44-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3b44-210">Boolean</span></span>|<span data-ttu-id="c3b44-211">Windows デバイス上での暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="c3b44-211">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="c3b44-212">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="c3b44-212">activeFirewallRequired</span></span>|<span data-ttu-id="c3b44-213">ブール型</span><span class="sxs-lookup"><span data-stu-id="c3b44-213">Boolean</span></span>|<span data-ttu-id="c3b44-214">Windows デバイス上のアクティブなファイアウォールが必要です。</span><span class="sxs-lookup"><span data-stu-id="c3b44-214">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="c3b44-215">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="c3b44-215">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="c3b44-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c3b44-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="c3b44-217">有効なオペレーティング システムは、Windows デバイス上の範囲を作成します。</span><span class="sxs-lookup"><span data-stu-id="c3b44-217">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="c3b44-218">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="c3b44-218">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c3b44-219">応答</span><span class="sxs-lookup"><span data-stu-id="c3b44-219">Response</span></span>
<span data-ttu-id="c3b44-220">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="c3b44-220">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3b44-221">例</span><span class="sxs-lookup"><span data-stu-id="c3b44-221">Example</span></span>
### <a name="request"></a><span data-ttu-id="c3b44-222">要求</span><span class="sxs-lookup"><span data-stu-id="c3b44-222">Request</span></span>
<span data-ttu-id="c3b44-223">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c3b44-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1152

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="c3b44-224">応答</span><span class="sxs-lookup"><span data-stu-id="c3b44-224">Response</span></span>
<span data-ttu-id="c3b44-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c3b44-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





