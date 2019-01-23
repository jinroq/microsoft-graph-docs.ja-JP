---
title: windows10CompliancePolicy の作成
description: 新しい windows10CompliancePolicy オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2eba67635ea4e596dd9bf1881b5b5c0d7b9743df
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422741"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="cf2b3-103">windows10CompliancePolicy の作成</span><span class="sxs-lookup"><span data-stu-id="cf2b3-103">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="cf2b3-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cf2b3-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf2b3-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf2b3-107">新しい [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-107">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf2b3-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="cf2b3-108">Prerequisites</span></span>
<span data-ttu-id="cf2b3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cf2b3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cf2b3-111">Permission type</span></span>|<span data-ttu-id="cf2b3-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cf2b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf2b3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cf2b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf2b3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf2b3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf2b3-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cf2b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf2b3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-116">Not supported.</span></span>|
|<span data-ttu-id="cf2b3-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cf2b3-117">Application</span></span>|<span data-ttu-id="cf2b3-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf2b3-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cf2b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="cf2b3-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf2b3-120">Request headers</span></span>
|<span data-ttu-id="cf2b3-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf2b3-121">Header</span></span>|<span data-ttu-id="cf2b3-122">値</span><span class="sxs-lookup"><span data-stu-id="cf2b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf2b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf2b3-123">Authorization</span></span>|<span data-ttu-id="cf2b3-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf2b3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf2b3-125">Accept</span></span>|<span data-ttu-id="cf2b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf2b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf2b3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="cf2b3-127">Request body</span></span>
<span data-ttu-id="cf2b3-128">要求本文で、windows10CompliancePolicy オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-128">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="cf2b3-129">次の表に、windows10CompliancePolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-129">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="cf2b3-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf2b3-130">Property</span></span>|<span data-ttu-id="cf2b3-131">型</span><span class="sxs-lookup"><span data-stu-id="cf2b3-131">Type</span></span>|<span data-ttu-id="cf2b3-132">説明</span><span class="sxs-lookup"><span data-stu-id="cf2b3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf2b3-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cf2b3-133">roleScopeTagIds</span></span>|<span data-ttu-id="cf2b3-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="cf2b3-134">String collection</span></span>|<span data-ttu-id="cf2b3-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cf2b3-136">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cf2b3-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cf2b3-137">id</span><span class="sxs-lookup"><span data-stu-id="cf2b3-137">id</span></span>|<span data-ttu-id="cf2b3-138">String</span><span class="sxs-lookup"><span data-stu-id="cf2b3-138">String</span></span>|<span data-ttu-id="cf2b3-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-139">Key of the entity.</span></span> <span data-ttu-id="cf2b3-140">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cf2b3-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cf2b3-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf2b3-141">createdDateTime</span></span>|<span data-ttu-id="cf2b3-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf2b3-142">DateTimeOffset</span></span>|<span data-ttu-id="cf2b3-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-143">DateTime the object was created.</span></span> <span data-ttu-id="cf2b3-144">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cf2b3-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cf2b3-145">説明</span><span class="sxs-lookup"><span data-stu-id="cf2b3-145">description</span></span>|<span data-ttu-id="cf2b3-146">String</span><span class="sxs-lookup"><span data-stu-id="cf2b3-146">String</span></span>|<span data-ttu-id="cf2b3-147">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cf2b3-148">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cf2b3-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cf2b3-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf2b3-149">lastModifiedDateTime</span></span>|<span data-ttu-id="cf2b3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf2b3-150">DateTimeOffset</span></span>|<span data-ttu-id="cf2b3-151">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-151">DateTime the object was last modified.</span></span> <span data-ttu-id="cf2b3-152">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cf2b3-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cf2b3-153">displayName</span><span class="sxs-lookup"><span data-stu-id="cf2b3-153">displayName</span></span>|<span data-ttu-id="cf2b3-154">String</span><span class="sxs-lookup"><span data-stu-id="cf2b3-154">String</span></span>|<span data-ttu-id="cf2b3-155">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cf2b3-156">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cf2b3-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cf2b3-157">version</span><span class="sxs-lookup"><span data-stu-id="cf2b3-157">version</span></span>|<span data-ttu-id="cf2b3-158">Int32</span><span class="sxs-lookup"><span data-stu-id="cf2b3-158">Int32</span></span>|<span data-ttu-id="cf2b3-159">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-159">Version of the device configuration.</span></span> <span data-ttu-id="cf2b3-160">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cf2b3-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cf2b3-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="cf2b3-161">passwordRequired</span></span>|<span data-ttu-id="cf2b3-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf2b3-162">Boolean</span></span>|<span data-ttu-id="cf2b3-163">Windows デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="cf2b3-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="cf2b3-164">passwordBlockSimple</span></span>|<span data-ttu-id="cf2b3-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf2b3-165">Boolean</span></span>|<span data-ttu-id="cf2b3-166">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="cf2b3-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="cf2b3-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="cf2b3-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf2b3-168">Boolean</span></span>|<span data-ttu-id="cf2b3-169">アイドル デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="cf2b3-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="cf2b3-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="cf2b3-171">Int32</span><span class="sxs-lookup"><span data-stu-id="cf2b3-171">Int32</span></span>|<span data-ttu-id="cf2b3-172">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="cf2b3-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="cf2b3-173">passwordExpirationDays</span></span>|<span data-ttu-id="cf2b3-174">Int32</span><span class="sxs-lookup"><span data-stu-id="cf2b3-174">Int32</span></span>|<span data-ttu-id="cf2b3-175">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-175">The password expiration in days.</span></span>|
|<span data-ttu-id="cf2b3-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="cf2b3-176">passwordMinimumLength</span></span>|<span data-ttu-id="cf2b3-177">Int32</span><span class="sxs-lookup"><span data-stu-id="cf2b3-177">Int32</span></span>|<span data-ttu-id="cf2b3-178">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-178">The minimum password length.</span></span>|
|<span data-ttu-id="cf2b3-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="cf2b3-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="cf2b3-180">Int32</span><span class="sxs-lookup"><span data-stu-id="cf2b3-180">Int32</span></span>|<span data-ttu-id="cf2b3-181">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="cf2b3-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="cf2b3-182">passwordRequiredType</span></span>|[<span data-ttu-id="cf2b3-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="cf2b3-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="cf2b3-184">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-184">The required password type.</span></span> <span data-ttu-id="cf2b3-185">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="cf2b3-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="cf2b3-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="cf2b3-187">Int32</span><span class="sxs-lookup"><span data-stu-id="cf2b3-187">Int32</span></span>|<span data-ttu-id="cf2b3-188">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="cf2b3-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="cf2b3-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="cf2b3-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf2b3-190">Boolean</span></span>|<span data-ttu-id="cf2b3-191">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="cf2b3-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="cf2b3-192">osMinimumVersion</span></span>|<span data-ttu-id="cf2b3-193">String</span><span class="sxs-lookup"><span data-stu-id="cf2b3-193">String</span></span>|<span data-ttu-id="cf2b3-194">Windows 10 の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="cf2b3-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="cf2b3-195">osMaximumVersion</span></span>|<span data-ttu-id="cf2b3-196">String</span><span class="sxs-lookup"><span data-stu-id="cf2b3-196">String</span></span>|<span data-ttu-id="cf2b3-197">Windows 10 の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="cf2b3-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="cf2b3-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="cf2b3-199">String</span><span class="sxs-lookup"><span data-stu-id="cf2b3-199">String</span></span>|<span data-ttu-id="cf2b3-200">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="cf2b3-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="cf2b3-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="cf2b3-202">String</span><span class="sxs-lookup"><span data-stu-id="cf2b3-202">String</span></span>|<span data-ttu-id="cf2b3-203">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="cf2b3-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="cf2b3-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="cf2b3-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf2b3-205">Boolean</span></span>|<span data-ttu-id="cf2b3-206">デバイスが Windows デバイス正常性構成証明によって正常と報告される (早期起動マルウェア対策ドライバーが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="cf2b3-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="cf2b3-207">bitLockerEnabled</span></span>|<span data-ttu-id="cf2b3-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf2b3-208">Boolean</span></span>|<span data-ttu-id="cf2b3-209">デバイスが Windows デバイス正常性構成証明によって正常と報告される (BitLocker が有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="cf2b3-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="cf2b3-210">secureBootEnabled</span></span>|<span data-ttu-id="cf2b3-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf2b3-211">Boolean</span></span>|<span data-ttu-id="cf2b3-212">デバイスが Windows デバイス正常性構成証明によって正常と報告される (セキュア ブートが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="cf2b3-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="cf2b3-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="cf2b3-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf2b3-214">Boolean</span></span>|<span data-ttu-id="cf2b3-215">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="cf2b3-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="cf2b3-216">storageRequireEncryption</span></span>|<span data-ttu-id="cf2b3-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf2b3-217">Boolean</span></span>|<span data-ttu-id="cf2b3-218">Windows デバイス上での暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="cf2b3-219">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="cf2b3-219">activeFirewallRequired</span></span>|<span data-ttu-id="cf2b3-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf2b3-220">Boolean</span></span>|<span data-ttu-id="cf2b3-221">Windows デバイス上のアクティブなファイアウォールが必要です。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="cf2b3-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="cf2b3-222">defenderEnabled</span></span>|<span data-ttu-id="cf2b3-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf2b3-223">Boolean</span></span>|<span data-ttu-id="cf2b3-224">Windows デバイスで Windows Defender のウイルス対策が必要です。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="cf2b3-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="cf2b3-225">defenderVersion</span></span>|<span data-ttu-id="cf2b3-226">String</span><span class="sxs-lookup"><span data-stu-id="cf2b3-226">String</span></span>|<span data-ttu-id="cf2b3-227">Windows デバイスの最小バージョンの Windows Defender のウイルス対策が必要です。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="cf2b3-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="cf2b3-228">signatureOutOfDate</span></span>|<span data-ttu-id="cf2b3-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf2b3-229">Boolean</span></span>|<span data-ttu-id="cf2b3-230">Windows デバイスで最新のものに、Windows Defender のウイルス対策署名が必要です。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="cf2b3-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="cf2b3-231">rtpEnabled</span></span>|<span data-ttu-id="cf2b3-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf2b3-232">Boolean</span></span>|<span data-ttu-id="cf2b3-233">Windows デバイスでは、Windows Defender のウイルス対策のリアルタイム保護を必要とします。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="cf2b3-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="cf2b3-234">antivirusRequired</span></span>|<span data-ttu-id="cf2b3-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf2b3-235">Boolean</span></span>|<span data-ttu-id="cf2b3-236">上にある Windows セキュリティ センターに登録され、(例: シマンテック、Windows Defender) を監視するウイルス対策ソリューションが必要です。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="cf2b3-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="cf2b3-237">antiSpywareRequired</span></span>|<span data-ttu-id="cf2b3-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf2b3-238">Boolean</span></span>|<span data-ttu-id="cf2b3-239">任意のウイルス対策ソリューションに Windows セキュリティ センターに登録され、監視 (シマンテック、Windows Defender など) が必要です。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="cf2b3-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="cf2b3-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="cf2b3-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cf2b3-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="cf2b3-242">有効なオペレーティング システムは、Windows デバイス上の範囲を作成します。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="cf2b3-243">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="cf2b3-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="cf2b3-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="cf2b3-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf2b3-245">Boolean</span></span>|<span data-ttu-id="cf2b3-246">デバイスの脅威保護が有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="cf2b3-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="cf2b3-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="cf2b3-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="cf2b3-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="cf2b3-249">法令遵守の不履行を報告する最小のリスク レベルの脅威のデバイスの保護を必要とします。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="cf2b3-250">使用可能な値: `unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="cf2b3-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="cf2b3-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="cf2b3-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf2b3-252">Boolean</span></span>|<span data-ttu-id="cf2b3-253">Intune 準拠状態の考慮事項に SCCM の準拠状態を考慮する必要があります。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|



## <a name="response"></a><span data-ttu-id="cf2b3-254">応答</span><span class="sxs-lookup"><span data-stu-id="cf2b3-254">Response</span></span>
<span data-ttu-id="cf2b3-255">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-255">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf2b3-256">例</span><span class="sxs-lookup"><span data-stu-id="cf2b3-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf2b3-257">要求</span><span class="sxs-lookup"><span data-stu-id="cf2b3-257">Request</span></span>
<span data-ttu-id="cf2b3-258">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-258">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cf2b3-259">応答</span><span class="sxs-lookup"><span data-stu-id="cf2b3-259">Response</span></span>
<span data-ttu-id="cf2b3-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cf2b3-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




