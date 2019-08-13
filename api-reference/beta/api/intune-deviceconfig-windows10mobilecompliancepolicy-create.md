---
title: Create windows10MobileCompliancePolicy
description: 新しい windows10MobileCompliancePolicy オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 37e8ae87869e6cd76e80a589c80b3f63e849dda1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345156"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="6cabd-103">Create windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="6cabd-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="6cabd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cabd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cabd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6cabd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cabd-106">新しい [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6cabd-106">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cabd-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6cabd-107">Prerequisites</span></span>
<span data-ttu-id="6cabd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6cabd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cabd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6cabd-110">Permission type</span></span>|<span data-ttu-id="6cabd-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6cabd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cabd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6cabd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6cabd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cabd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6cabd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6cabd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cabd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cabd-115">Not supported.</span></span>|
|<span data-ttu-id="6cabd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6cabd-116">Application</span></span>|<span data-ttu-id="6cabd-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cabd-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cabd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6cabd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="6cabd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6cabd-119">Request headers</span></span>
|<span data-ttu-id="6cabd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6cabd-120">Header</span></span>|<span data-ttu-id="6cabd-121">値</span><span class="sxs-lookup"><span data-stu-id="6cabd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cabd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cabd-122">Authorization</span></span>|<span data-ttu-id="6cabd-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6cabd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cabd-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6cabd-124">Accept</span></span>|<span data-ttu-id="6cabd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6cabd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cabd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6cabd-126">Request body</span></span>
<span data-ttu-id="6cabd-127">要求本文で、windows10MobileCompliancePolicy オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6cabd-127">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="6cabd-128">次の表に、windows10MobileCompliancePolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6cabd-128">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="6cabd-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6cabd-129">Property</span></span>|<span data-ttu-id="6cabd-130">型</span><span class="sxs-lookup"><span data-stu-id="6cabd-130">Type</span></span>|<span data-ttu-id="6cabd-131">説明</span><span class="sxs-lookup"><span data-stu-id="6cabd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cabd-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6cabd-132">roleScopeTagIds</span></span>|<span data-ttu-id="6cabd-133">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="6cabd-133">String collection</span></span>|<span data-ttu-id="6cabd-134">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="6cabd-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6cabd-135">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cabd-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6cabd-136">id</span><span class="sxs-lookup"><span data-stu-id="6cabd-136">id</span></span>|<span data-ttu-id="6cabd-137">文字列</span><span class="sxs-lookup"><span data-stu-id="6cabd-137">String</span></span>|<span data-ttu-id="6cabd-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6cabd-138">Key of the entity.</span></span> <span data-ttu-id="6cabd-139">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cabd-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6cabd-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6cabd-140">createdDateTime</span></span>|<span data-ttu-id="6cabd-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cabd-141">DateTimeOffset</span></span>|<span data-ttu-id="6cabd-142">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6cabd-142">DateTime the object was created.</span></span> <span data-ttu-id="6cabd-143">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cabd-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6cabd-144">description</span><span class="sxs-lookup"><span data-stu-id="6cabd-144">description</span></span>|<span data-ttu-id="6cabd-145">String</span><span class="sxs-lookup"><span data-stu-id="6cabd-145">String</span></span>|<span data-ttu-id="6cabd-146">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="6cabd-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6cabd-147">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cabd-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6cabd-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6cabd-148">lastModifiedDateTime</span></span>|<span data-ttu-id="6cabd-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cabd-149">DateTimeOffset</span></span>|<span data-ttu-id="6cabd-150">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="6cabd-150">DateTime the object was last modified.</span></span> <span data-ttu-id="6cabd-151">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cabd-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6cabd-152">displayName</span><span class="sxs-lookup"><span data-stu-id="6cabd-152">displayName</span></span>|<span data-ttu-id="6cabd-153">String</span><span class="sxs-lookup"><span data-stu-id="6cabd-153">String</span></span>|<span data-ttu-id="6cabd-154">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="6cabd-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6cabd-155">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cabd-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6cabd-156">version</span><span class="sxs-lookup"><span data-stu-id="6cabd-156">version</span></span>|<span data-ttu-id="6cabd-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6cabd-157">Int32</span></span>|<span data-ttu-id="6cabd-158">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="6cabd-158">Version of the device configuration.</span></span> <span data-ttu-id="6cabd-159">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cabd-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6cabd-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6cabd-160">passwordRequired</span></span>|<span data-ttu-id="6cabd-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cabd-161">Boolean</span></span>|<span data-ttu-id="6cabd-162">Windows Phone デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="6cabd-162">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="6cabd-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6cabd-163">passwordBlockSimple</span></span>|<span data-ttu-id="6cabd-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cabd-164">Boolean</span></span>|<span data-ttu-id="6cabd-165">カレンダーの同期を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6cabd-165">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="6cabd-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6cabd-166">passwordMinimumLength</span></span>|<span data-ttu-id="6cabd-167">Int32</span><span class="sxs-lookup"><span data-stu-id="6cabd-167">Int32</span></span>|<span data-ttu-id="6cabd-168">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="6cabd-168">Minimum password length.</span></span> <span data-ttu-id="6cabd-169">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="6cabd-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="6cabd-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6cabd-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="6cabd-171">Int32</span><span class="sxs-lookup"><span data-stu-id="6cabd-171">Int32</span></span>|<span data-ttu-id="6cabd-172">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="6cabd-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="6cabd-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6cabd-173">passwordRequiredType</span></span>|[<span data-ttu-id="6cabd-174">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6cabd-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6cabd-175">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="6cabd-175">The required password type.</span></span> <span data-ttu-id="6cabd-176">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="6cabd-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6cabd-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6cabd-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6cabd-178">Int32</span><span class="sxs-lookup"><span data-stu-id="6cabd-178">Int32</span></span>|<span data-ttu-id="6cabd-179">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="6cabd-179">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="6cabd-180">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6cabd-180">passwordExpirationDays</span></span>|<span data-ttu-id="6cabd-181">Int32</span><span class="sxs-lookup"><span data-stu-id="6cabd-181">Int32</span></span>|<span data-ttu-id="6cabd-182">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="6cabd-182">Number of days before password expiration.</span></span> <span data-ttu-id="6cabd-183">有効な値は 1 から 255 までです</span><span class="sxs-lookup"><span data-stu-id="6cabd-183">Valid values 1 to 255</span></span>|
|<span data-ttu-id="6cabd-184">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6cabd-184">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6cabd-185">Int32</span><span class="sxs-lookup"><span data-stu-id="6cabd-185">Int32</span></span>|<span data-ttu-id="6cabd-186">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="6cabd-186">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="6cabd-187">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="6cabd-187">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="6cabd-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cabd-188">Boolean</span></span>|<span data-ttu-id="6cabd-189">アイドル デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="6cabd-189">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="6cabd-190">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6cabd-190">osMinimumVersion</span></span>|<span data-ttu-id="6cabd-191">String</span><span class="sxs-lookup"><span data-stu-id="6cabd-191">String</span></span>|<span data-ttu-id="6cabd-192">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="6cabd-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="6cabd-193">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6cabd-193">osMaximumVersion</span></span>|<span data-ttu-id="6cabd-194">String</span><span class="sxs-lookup"><span data-stu-id="6cabd-194">String</span></span>|<span data-ttu-id="6cabd-195">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="6cabd-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="6cabd-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="6cabd-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="6cabd-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cabd-197">Boolean</span></span>|<span data-ttu-id="6cabd-198">デバイスが Windows デバイス正常性構成証明によって正常と報告される (早期起動マルウェア対策ドライバーが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="6cabd-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="6cabd-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="6cabd-199">bitLockerEnabled</span></span>|<span data-ttu-id="6cabd-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cabd-200">Boolean</span></span>|<span data-ttu-id="6cabd-201">デバイスが Windows デバイス正常性構成証明によって正常と報告される (BitLocker が有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="6cabd-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="6cabd-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="6cabd-202">secureBootEnabled</span></span>|<span data-ttu-id="6cabd-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cabd-203">Boolean</span></span>|<span data-ttu-id="6cabd-204">デバイスが Windows デバイス正常性構成証明によって正常と報告される (セキュア ブートが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="6cabd-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="6cabd-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="6cabd-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="6cabd-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cabd-206">Boolean</span></span>|<span data-ttu-id="6cabd-207">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="6cabd-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="6cabd-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="6cabd-208">storageRequireEncryption</span></span>|<span data-ttu-id="6cabd-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cabd-209">Boolean</span></span>|<span data-ttu-id="6cabd-210">Windows デバイス上での暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="6cabd-210">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="6cabd-211">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="6cabd-211">activeFirewallRequired</span></span>|<span data-ttu-id="6cabd-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cabd-212">Boolean</span></span>|<span data-ttu-id="6cabd-213">Windows デバイスでアクティブなファイアウォールが必要です。</span><span class="sxs-lookup"><span data-stu-id="6cabd-213">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="6cabd-214">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="6cabd-214">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="6cabd-215">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6cabd-215">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="6cabd-216">Windows デバイス上の有効なオペレーティングシステムのビルド範囲。</span><span class="sxs-lookup"><span data-stu-id="6cabd-216">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="6cabd-217">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="6cabd-217">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="6cabd-218">応答</span><span class="sxs-lookup"><span data-stu-id="6cabd-218">Response</span></span>
<span data-ttu-id="6cabd-219">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6cabd-219">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cabd-220">例</span><span class="sxs-lookup"><span data-stu-id="6cabd-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cabd-221">要求</span><span class="sxs-lookup"><span data-stu-id="6cabd-221">Request</span></span>
<span data-ttu-id="6cabd-222">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6cabd-222">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6cabd-223">応答</span><span class="sxs-lookup"><span data-stu-id="6cabd-223">Response</span></span>
<span data-ttu-id="6cabd-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6cabd-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






