---
title: Create windows10MobileCompliancePolicy
description: 新しい windows10MobileCompliancePolicy オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 782f81110dc5fe60fd9e8fa21249fd42be9dc4c5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155567"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="a4017-103">Create windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a4017-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="a4017-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4017-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4017-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4017-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4017-106">新しい [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a4017-106">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4017-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a4017-107">Prerequisites</span></span>
<span data-ttu-id="a4017-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a4017-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a4017-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a4017-110">Permission type</span></span>|<span data-ttu-id="a4017-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a4017-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4017-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a4017-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4017-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4017-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a4017-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a4017-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4017-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4017-115">Not supported.</span></span>|
|<span data-ttu-id="a4017-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a4017-116">Application</span></span>|<span data-ttu-id="a4017-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4017-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4017-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a4017-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="a4017-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4017-119">Request headers</span></span>
|<span data-ttu-id="a4017-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4017-120">Header</span></span>|<span data-ttu-id="a4017-121">値</span><span class="sxs-lookup"><span data-stu-id="a4017-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4017-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4017-122">Authorization</span></span>|<span data-ttu-id="a4017-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a4017-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4017-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a4017-124">Accept</span></span>|<span data-ttu-id="a4017-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a4017-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4017-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a4017-126">Request body</span></span>
<span data-ttu-id="a4017-127">要求本文で、windows10MobileCompliancePolicy オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a4017-127">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="a4017-128">次の表に、windows10MobileCompliancePolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a4017-128">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="a4017-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4017-129">Property</span></span>|<span data-ttu-id="a4017-130">型</span><span class="sxs-lookup"><span data-stu-id="a4017-130">Type</span></span>|<span data-ttu-id="a4017-131">説明</span><span class="sxs-lookup"><span data-stu-id="a4017-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4017-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a4017-132">roleScopeTagIds</span></span>|<span data-ttu-id="a4017-133">String collection</span><span class="sxs-lookup"><span data-stu-id="a4017-133">String collection</span></span>|<span data-ttu-id="a4017-134">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="a4017-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a4017-135">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4017-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a4017-136">id</span><span class="sxs-lookup"><span data-stu-id="a4017-136">id</span></span>|<span data-ttu-id="a4017-137">文字列</span><span class="sxs-lookup"><span data-stu-id="a4017-137">String</span></span>|<span data-ttu-id="a4017-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a4017-138">Key of the entity.</span></span> <span data-ttu-id="a4017-139">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4017-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a4017-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4017-140">createdDateTime</span></span>|<span data-ttu-id="a4017-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4017-141">DateTimeOffset</span></span>|<span data-ttu-id="a4017-142">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a4017-142">DateTime the object was created.</span></span> <span data-ttu-id="a4017-143">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4017-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a4017-144">説明</span><span class="sxs-lookup"><span data-stu-id="a4017-144">description</span></span>|<span data-ttu-id="a4017-145">文字列</span><span class="sxs-lookup"><span data-stu-id="a4017-145">String</span></span>|<span data-ttu-id="a4017-146">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="a4017-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a4017-147">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4017-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a4017-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4017-148">lastModifiedDateTime</span></span>|<span data-ttu-id="a4017-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4017-149">DateTimeOffset</span></span>|<span data-ttu-id="a4017-150">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a4017-150">DateTime the object was last modified.</span></span> <span data-ttu-id="a4017-151">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4017-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a4017-152">displayName</span><span class="sxs-lookup"><span data-stu-id="a4017-152">displayName</span></span>|<span data-ttu-id="a4017-153">String</span><span class="sxs-lookup"><span data-stu-id="a4017-153">String</span></span>|<span data-ttu-id="a4017-154">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="a4017-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a4017-155">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4017-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a4017-156">version</span><span class="sxs-lookup"><span data-stu-id="a4017-156">version</span></span>|<span data-ttu-id="a4017-157">Int32</span><span class="sxs-lookup"><span data-stu-id="a4017-157">Int32</span></span>|<span data-ttu-id="a4017-158">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a4017-158">Version of the device configuration.</span></span> <span data-ttu-id="a4017-159">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4017-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a4017-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="a4017-160">passwordRequired</span></span>|<span data-ttu-id="a4017-161">ブール値</span><span class="sxs-lookup"><span data-stu-id="a4017-161">Boolean</span></span>|<span data-ttu-id="a4017-162">Windows Phone デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="a4017-162">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="a4017-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="a4017-163">passwordBlockSimple</span></span>|<span data-ttu-id="a4017-164">ブール値</span><span class="sxs-lookup"><span data-stu-id="a4017-164">Boolean</span></span>|<span data-ttu-id="a4017-165">カレンダーの同期を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="a4017-165">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="a4017-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a4017-166">passwordMinimumLength</span></span>|<span data-ttu-id="a4017-167">Int32</span><span class="sxs-lookup"><span data-stu-id="a4017-167">Int32</span></span>|<span data-ttu-id="a4017-168">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="a4017-168">Minimum password length.</span></span> <span data-ttu-id="a4017-169">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="a4017-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a4017-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="a4017-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="a4017-171">Int32</span><span class="sxs-lookup"><span data-stu-id="a4017-171">Int32</span></span>|<span data-ttu-id="a4017-172">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="a4017-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="a4017-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a4017-173">passwordRequiredType</span></span>|[<span data-ttu-id="a4017-174">requiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="a4017-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="a4017-175">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="a4017-175">The required password type.</span></span> <span data-ttu-id="a4017-176">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="a4017-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="a4017-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a4017-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a4017-178">Int32</span><span class="sxs-lookup"><span data-stu-id="a4017-178">Int32</span></span>|<span data-ttu-id="a4017-179">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="a4017-179">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="a4017-180">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a4017-180">passwordExpirationDays</span></span>|<span data-ttu-id="a4017-181">Int32</span><span class="sxs-lookup"><span data-stu-id="a4017-181">Int32</span></span>|<span data-ttu-id="a4017-182">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="a4017-182">Number of days before password expiration.</span></span> <span data-ttu-id="a4017-183">有効な値は 1 から 255 までです</span><span class="sxs-lookup"><span data-stu-id="a4017-183">Valid values 1 to 255</span></span>|
|<span data-ttu-id="a4017-184">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="a4017-184">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="a4017-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a4017-185">Int32</span></span>|<span data-ttu-id="a4017-186">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="a4017-186">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="a4017-187">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="a4017-187">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="a4017-188">ブール値</span><span class="sxs-lookup"><span data-stu-id="a4017-188">Boolean</span></span>|<span data-ttu-id="a4017-189">アイドル デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="a4017-189">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="a4017-190">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="a4017-190">osMinimumVersion</span></span>|<span data-ttu-id="a4017-191">String</span><span class="sxs-lookup"><span data-stu-id="a4017-191">String</span></span>|<span data-ttu-id="a4017-192">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="a4017-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="a4017-193">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="a4017-193">osMaximumVersion</span></span>|<span data-ttu-id="a4017-194">String</span><span class="sxs-lookup"><span data-stu-id="a4017-194">String</span></span>|<span data-ttu-id="a4017-195">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="a4017-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="a4017-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="a4017-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="a4017-197">ブール値</span><span class="sxs-lookup"><span data-stu-id="a4017-197">Boolean</span></span>|<span data-ttu-id="a4017-198">デバイスが Windows デバイス正常性構成証明によって正常と報告される (早期起動マルウェア対策ドライバーが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="a4017-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="a4017-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="a4017-199">bitLockerEnabled</span></span>|<span data-ttu-id="a4017-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4017-200">Boolean</span></span>|<span data-ttu-id="a4017-201">デバイスが Windows デバイス正常性構成証明によって正常と報告される (BitLocker が有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="a4017-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="a4017-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="a4017-202">secureBootEnabled</span></span>|<span data-ttu-id="a4017-203">ブール値</span><span class="sxs-lookup"><span data-stu-id="a4017-203">Boolean</span></span>|<span data-ttu-id="a4017-204">デバイスが Windows デバイス正常性構成証明によって正常と報告される (セキュア ブートが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="a4017-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="a4017-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="a4017-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="a4017-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4017-206">Boolean</span></span>|<span data-ttu-id="a4017-207">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="a4017-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="a4017-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="a4017-208">storageRequireEncryption</span></span>|<span data-ttu-id="a4017-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4017-209">Boolean</span></span>|<span data-ttu-id="a4017-210">Windows デバイス上での暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="a4017-210">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="a4017-211">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="a4017-211">activeFirewallRequired</span></span>|<span data-ttu-id="a4017-212">ブール値</span><span class="sxs-lookup"><span data-stu-id="a4017-212">Boolean</span></span>|<span data-ttu-id="a4017-213">Windows デバイスでアクティブなファイアウォールが必要です。</span><span class="sxs-lookup"><span data-stu-id="a4017-213">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="a4017-214">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="a4017-214">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="a4017-215">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a4017-215">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="a4017-216">Windows デバイス上の有効なオペレーティングシステムのビルド範囲。</span><span class="sxs-lookup"><span data-stu-id="a4017-216">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="a4017-217">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a4017-217">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="a4017-218">応答</span><span class="sxs-lookup"><span data-stu-id="a4017-218">Response</span></span>
<span data-ttu-id="a4017-219">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a4017-219">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4017-220">例</span><span class="sxs-lookup"><span data-stu-id="a4017-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4017-221">要求</span><span class="sxs-lookup"><span data-stu-id="a4017-221">Request</span></span>
<span data-ttu-id="a4017-222">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a4017-222">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a4017-223">応答</span><span class="sxs-lookup"><span data-stu-id="a4017-223">Response</span></span>
<span data-ttu-id="a4017-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a4017-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




