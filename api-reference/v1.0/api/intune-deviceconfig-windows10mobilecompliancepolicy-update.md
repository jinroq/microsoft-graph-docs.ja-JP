---
title: windows10MobileCompliancePolicy の更新
description: windows10MobileCompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cb78108dc5e97a195f5dddf8b486aef2457df049
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881167"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="c3bbf-103">windows10MobileCompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="c3bbf-103">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="c3bbf-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3bbf-105">[windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-105">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c3bbf-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="c3bbf-106">Prerequisites</span></span>
<span data-ttu-id="c3bbf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3bbf-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3bbf-109">Permission type</span></span>|<span data-ttu-id="c3bbf-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3bbf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3bbf-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3bbf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c3bbf-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3bbf-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c3bbf-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3bbf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3bbf-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-114">Not supported.</span></span>|
|<span data-ttu-id="c3bbf-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3bbf-115">Application</span></span>|<span data-ttu-id="c3bbf-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3bbf-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3bbf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="c3bbf-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3bbf-118">Request headers</span></span>
|<span data-ttu-id="c3bbf-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3bbf-119">Header</span></span>|<span data-ttu-id="c3bbf-120">値</span><span class="sxs-lookup"><span data-stu-id="c3bbf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3bbf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3bbf-121">Authorization</span></span>|<span data-ttu-id="c3bbf-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3bbf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c3bbf-123">Accept</span></span>|<span data-ttu-id="c3bbf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c3bbf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3bbf-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3bbf-125">Request body</span></span>
<span data-ttu-id="c3bbf-126">要求本文で、[windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-126">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="c3bbf-127">次の表に、[windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-127">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="c3bbf-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3bbf-128">Property</span></span>|<span data-ttu-id="c3bbf-129">種類</span><span class="sxs-lookup"><span data-stu-id="c3bbf-129">Type</span></span>|<span data-ttu-id="c3bbf-130">説明</span><span class="sxs-lookup"><span data-stu-id="c3bbf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3bbf-131">ID</span><span class="sxs-lookup"><span data-stu-id="c3bbf-131">id</span></span>|<span data-ttu-id="c3bbf-132">String</span><span class="sxs-lookup"><span data-stu-id="c3bbf-132">String</span></span>|<span data-ttu-id="c3bbf-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-133">Key of the entity.</span></span> <span data-ttu-id="c3bbf-134">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3bbf-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c3bbf-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3bbf-135">createdDateTime</span></span>|<span data-ttu-id="c3bbf-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3bbf-136">DateTimeOffset</span></span>|<span data-ttu-id="c3bbf-137">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-137">DateTime the object was created.</span></span> <span data-ttu-id="c3bbf-138">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3bbf-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c3bbf-139">説明</span><span class="sxs-lookup"><span data-stu-id="c3bbf-139">description</span></span>|<span data-ttu-id="c3bbf-140">String</span><span class="sxs-lookup"><span data-stu-id="c3bbf-140">String</span></span>|<span data-ttu-id="c3bbf-141">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c3bbf-142">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3bbf-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c3bbf-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3bbf-143">lastModifiedDateTime</span></span>|<span data-ttu-id="c3bbf-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3bbf-144">DateTimeOffset</span></span>|<span data-ttu-id="c3bbf-145">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-145">DateTime the object was last modified.</span></span> <span data-ttu-id="c3bbf-146">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3bbf-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c3bbf-147">displayName</span><span class="sxs-lookup"><span data-stu-id="c3bbf-147">displayName</span></span>|<span data-ttu-id="c3bbf-148">String</span><span class="sxs-lookup"><span data-stu-id="c3bbf-148">String</span></span>|<span data-ttu-id="c3bbf-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c3bbf-150">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3bbf-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c3bbf-151">version</span><span class="sxs-lookup"><span data-stu-id="c3bbf-151">version</span></span>|<span data-ttu-id="c3bbf-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bbf-152">Int32</span></span>|<span data-ttu-id="c3bbf-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-153">Version of the device configuration.</span></span> <span data-ttu-id="c3bbf-154">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3bbf-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c3bbf-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c3bbf-155">passwordRequired</span></span>|<span data-ttu-id="c3bbf-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3bbf-156">Boolean</span></span>|<span data-ttu-id="c3bbf-157">Windows Phone デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-157">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="c3bbf-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c3bbf-158">passwordBlockSimple</span></span>|<span data-ttu-id="c3bbf-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3bbf-159">Boolean</span></span>|<span data-ttu-id="c3bbf-160">カレンダーの同期を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-160">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="c3bbf-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c3bbf-161">passwordMinimumLength</span></span>|<span data-ttu-id="c3bbf-162">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bbf-162">Int32</span></span>|<span data-ttu-id="c3bbf-163">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-163">Minimum password length.</span></span> <span data-ttu-id="c3bbf-164">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="c3bbf-164">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c3bbf-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c3bbf-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="c3bbf-166">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bbf-166">Int32</span></span>|<span data-ttu-id="c3bbf-167">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="c3bbf-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c3bbf-168">passwordRequiredType</span></span>|[<span data-ttu-id="c3bbf-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c3bbf-169">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c3bbf-170">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-170">The required password type.</span></span> <span data-ttu-id="c3bbf-171">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c3bbf-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c3bbf-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c3bbf-173">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bbf-173">Int32</span></span>|<span data-ttu-id="c3bbf-174">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-174">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="c3bbf-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c3bbf-175">passwordExpirationDays</span></span>|<span data-ttu-id="c3bbf-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bbf-176">Int32</span></span>|<span data-ttu-id="c3bbf-177">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-177">Number of days before password expiration.</span></span> <span data-ttu-id="c3bbf-178">有効な値は 1 から 255 までです</span><span class="sxs-lookup"><span data-stu-id="c3bbf-178">Valid values 1 to 255</span></span>|
|<span data-ttu-id="c3bbf-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c3bbf-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c3bbf-180">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bbf-180">Int32</span></span>|<span data-ttu-id="c3bbf-181">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-181">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="c3bbf-182">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="c3bbf-182">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="c3bbf-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3bbf-183">Boolean</span></span>|<span data-ttu-id="c3bbf-184">アイドル デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-184">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="c3bbf-185">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c3bbf-185">osMinimumVersion</span></span>|<span data-ttu-id="c3bbf-186">String</span><span class="sxs-lookup"><span data-stu-id="c3bbf-186">String</span></span>|<span data-ttu-id="c3bbf-187">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-187">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="c3bbf-188">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c3bbf-188">osMaximumVersion</span></span>|<span data-ttu-id="c3bbf-189">String</span><span class="sxs-lookup"><span data-stu-id="c3bbf-189">String</span></span>|<span data-ttu-id="c3bbf-190">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-190">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="c3bbf-191">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="c3bbf-191">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="c3bbf-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3bbf-192">Boolean</span></span>|<span data-ttu-id="c3bbf-193">デバイスが Windows デバイス正常性構成証明によって正常と報告される (早期起動マルウェア対策ドライバーが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-193">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="c3bbf-194">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="c3bbf-194">bitLockerEnabled</span></span>|<span data-ttu-id="c3bbf-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3bbf-195">Boolean</span></span>|<span data-ttu-id="c3bbf-196">デバイスが Windows デバイス正常性構成証明によって正常と報告される (BitLocker が有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-196">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="c3bbf-197">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="c3bbf-197">secureBootEnabled</span></span>|<span data-ttu-id="c3bbf-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3bbf-198">Boolean</span></span>|<span data-ttu-id="c3bbf-199">デバイスが Windows デバイス正常性構成証明によって正常と報告される (セキュア ブートが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-199">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="c3bbf-200">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="c3bbf-200">codeIntegrityEnabled</span></span>|<span data-ttu-id="c3bbf-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3bbf-201">Boolean</span></span>|<span data-ttu-id="c3bbf-202">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-202">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="c3bbf-203">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="c3bbf-203">storageRequireEncryption</span></span>|<span data-ttu-id="c3bbf-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3bbf-204">Boolean</span></span>|<span data-ttu-id="c3bbf-205">Windows デバイス上での暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-205">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="c3bbf-206">応答</span><span class="sxs-lookup"><span data-stu-id="c3bbf-206">Response</span></span>
<span data-ttu-id="c3bbf-207">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-207">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3bbf-208">例</span><span class="sxs-lookup"><span data-stu-id="c3bbf-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="c3bbf-209">要求</span><span class="sxs-lookup"><span data-stu-id="c3bbf-209">Request</span></span>
<span data-ttu-id="c3bbf-210">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 792

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
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
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="c3bbf-211">応答</span><span class="sxs-lookup"><span data-stu-id="c3bbf-211">Response</span></span>
<span data-ttu-id="c3bbf-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c3bbf-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 964

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
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
  "storageRequireEncryption": true
}
```



