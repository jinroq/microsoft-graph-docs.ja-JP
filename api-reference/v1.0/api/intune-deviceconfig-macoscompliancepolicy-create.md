---
title: macOSCompliancePolicy の作成
description: 新しい macOSCompliancePolicy オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 615d60cc91d4ca463331b6352d29734640d6f5fc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302234"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="dd0cc-103">macOSCompliancePolicy の作成</span><span class="sxs-lookup"><span data-stu-id="dd0cc-103">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="dd0cc-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd0cc-105">新しい [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-105">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dd0cc-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="dd0cc-106">Prerequisites</span></span>
<span data-ttu-id="dd0cc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd0cc-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dd0cc-109">Permission type</span></span>|<span data-ttu-id="dd0cc-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dd0cc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd0cc-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dd0cc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dd0cc-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd0cc-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd0cc-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dd0cc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd0cc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-114">Not supported.</span></span>|
|<span data-ttu-id="dd0cc-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dd0cc-115">Application</span></span>|<span data-ttu-id="dd0cc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd0cc-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dd0cc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="dd0cc-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dd0cc-118">Request headers</span></span>
|<span data-ttu-id="dd0cc-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dd0cc-119">Header</span></span>|<span data-ttu-id="dd0cc-120">値</span><span class="sxs-lookup"><span data-stu-id="dd0cc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd0cc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd0cc-121">Authorization</span></span>|<span data-ttu-id="dd0cc-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd0cc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="dd0cc-123">Accept</span></span>|<span data-ttu-id="dd0cc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dd0cc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd0cc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="dd0cc-125">Request body</span></span>
<span data-ttu-id="dd0cc-126">要求本文で、macOSCompliancePolicy オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-126">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="dd0cc-127">次の表に、macOSCompliancePolicy 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-127">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="dd0cc-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dd0cc-128">Property</span></span>|<span data-ttu-id="dd0cc-129">種類</span><span class="sxs-lookup"><span data-stu-id="dd0cc-129">Type</span></span>|<span data-ttu-id="dd0cc-130">説明</span><span class="sxs-lookup"><span data-stu-id="dd0cc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd0cc-131">ID</span><span class="sxs-lookup"><span data-stu-id="dd0cc-131">id</span></span>|<span data-ttu-id="dd0cc-132">String</span><span class="sxs-lookup"><span data-stu-id="dd0cc-132">String</span></span>|<span data-ttu-id="dd0cc-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-133">Key of the entity.</span></span> <span data-ttu-id="dd0cc-134">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd0cc-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dd0cc-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd0cc-135">createdDateTime</span></span>|<span data-ttu-id="dd0cc-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd0cc-136">DateTimeOffset</span></span>|<span data-ttu-id="dd0cc-137">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-137">DateTime the object was created.</span></span> <span data-ttu-id="dd0cc-138">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd0cc-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dd0cc-139">説明</span><span class="sxs-lookup"><span data-stu-id="dd0cc-139">description</span></span>|<span data-ttu-id="dd0cc-140">String</span><span class="sxs-lookup"><span data-stu-id="dd0cc-140">String</span></span>|<span data-ttu-id="dd0cc-141">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dd0cc-142">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd0cc-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dd0cc-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd0cc-143">lastModifiedDateTime</span></span>|<span data-ttu-id="dd0cc-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd0cc-144">DateTimeOffset</span></span>|<span data-ttu-id="dd0cc-145">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-145">DateTime the object was last modified.</span></span> <span data-ttu-id="dd0cc-146">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd0cc-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dd0cc-147">displayName</span><span class="sxs-lookup"><span data-stu-id="dd0cc-147">displayName</span></span>|<span data-ttu-id="dd0cc-148">String</span><span class="sxs-lookup"><span data-stu-id="dd0cc-148">String</span></span>|<span data-ttu-id="dd0cc-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dd0cc-150">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd0cc-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dd0cc-151">version</span><span class="sxs-lookup"><span data-stu-id="dd0cc-151">version</span></span>|<span data-ttu-id="dd0cc-152">Int32</span><span class="sxs-lookup"><span data-stu-id="dd0cc-152">Int32</span></span>|<span data-ttu-id="dd0cc-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-153">Version of the device configuration.</span></span> <span data-ttu-id="dd0cc-154">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dd0cc-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dd0cc-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="dd0cc-155">passwordRequired</span></span>|<span data-ttu-id="dd0cc-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd0cc-156">Boolean</span></span>|<span data-ttu-id="dd0cc-157">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-157">Whether or not to require a password.</span></span>|
|<span data-ttu-id="dd0cc-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="dd0cc-158">passwordBlockSimple</span></span>|<span data-ttu-id="dd0cc-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd0cc-159">Boolean</span></span>|<span data-ttu-id="dd0cc-160">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-160">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="dd0cc-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="dd0cc-161">passwordExpirationDays</span></span>|<span data-ttu-id="dd0cc-162">Int32</span><span class="sxs-lookup"><span data-stu-id="dd0cc-162">Int32</span></span>|<span data-ttu-id="dd0cc-163">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-163">Number of days before the password expires.</span></span> <span data-ttu-id="dd0cc-164">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="dd0cc-164">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="dd0cc-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="dd0cc-165">passwordMinimumLength</span></span>|<span data-ttu-id="dd0cc-166">Int32</span><span class="sxs-lookup"><span data-stu-id="dd0cc-166">Int32</span></span>|<span data-ttu-id="dd0cc-167">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-167">Minimum length of password.</span></span> <span data-ttu-id="dd0cc-168">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="dd0cc-168">Valid values 4 to 14</span></span>|
|<span data-ttu-id="dd0cc-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="dd0cc-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="dd0cc-170">Int32</span><span class="sxs-lookup"><span data-stu-id="dd0cc-170">Int32</span></span>|<span data-ttu-id="dd0cc-171">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="dd0cc-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="dd0cc-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="dd0cc-173">Int32</span><span class="sxs-lookup"><span data-stu-id="dd0cc-173">Int32</span></span>|<span data-ttu-id="dd0cc-174">禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-174">Number of previous passwords to block.</span></span> <span data-ttu-id="dd0cc-175">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="dd0cc-175">Valid values 1 to 24</span></span>|
|<span data-ttu-id="dd0cc-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="dd0cc-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="dd0cc-177">Int32</span><span class="sxs-lookup"><span data-stu-id="dd0cc-177">Int32</span></span>|<span data-ttu-id="dd0cc-178">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="dd0cc-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="dd0cc-179">passwordRequiredType</span></span>|[<span data-ttu-id="dd0cc-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="dd0cc-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="dd0cc-181">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-181">The required password type.</span></span> <span data-ttu-id="dd0cc-182">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="dd0cc-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="dd0cc-183">osMinimumVersion</span></span>|<span data-ttu-id="dd0cc-184">String</span><span class="sxs-lookup"><span data-stu-id="dd0cc-184">String</span></span>|<span data-ttu-id="dd0cc-185">最低限必要な iOS のバージョン。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="dd0cc-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="dd0cc-186">osMaximumVersion</span></span>|<span data-ttu-id="dd0cc-187">String</span><span class="sxs-lookup"><span data-stu-id="dd0cc-187">String</span></span>|<span data-ttu-id="dd0cc-188">最大の iOS バージョン。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="dd0cc-189">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="dd0cc-189">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="dd0cc-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd0cc-190">Boolean</span></span>|<span data-ttu-id="dd0cc-191">デバイスでシステム整合性の保護が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-191">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="dd0cc-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="dd0cc-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="dd0cc-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd0cc-193">Boolean</span></span>|<span data-ttu-id="dd0cc-194">デバイスへの脅威に対する保護が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="dd0cc-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="dd0cc-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="dd0cc-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="dd0cc-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="dd0cc-197">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="dd0cc-198">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="dd0cc-199">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="dd0cc-199">storageRequireEncryption</span></span>|<span data-ttu-id="dd0cc-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd0cc-200">Boolean</span></span>|<span data-ttu-id="dd0cc-201">Mac OS デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-201">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="dd0cc-202">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="dd0cc-202">firewallEnabled</span></span>|<span data-ttu-id="dd0cc-203">ブール型</span><span class="sxs-lookup"><span data-stu-id="dd0cc-203">Boolean</span></span>|<span data-ttu-id="dd0cc-204">かどうか、か、これらのファイアウォールは有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-204">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="dd0cc-205">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="dd0cc-205">firewallBlockAllIncoming</span></span>|<span data-ttu-id="dd0cc-206">ブール型</span><span class="sxs-lookup"><span data-stu-id="dd0cc-206">Boolean</span></span>|<span data-ttu-id="dd0cc-207">「すべての着信接続をブロックする] オプションに対応します。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-207">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="dd0cc-208">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="dd0cc-208">firewallEnableStealthMode</span></span>|<span data-ttu-id="dd0cc-209">ブール型</span><span class="sxs-lookup"><span data-stu-id="dd0cc-209">Boolean</span></span>|<span data-ttu-id="dd0cc-210">「有効にするステルス モード」に対応</span><span class="sxs-lookup"><span data-stu-id="dd0cc-210">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="dd0cc-211">応答</span><span class="sxs-lookup"><span data-stu-id="dd0cc-211">Response</span></span>
<span data-ttu-id="dd0cc-212">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-212">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd0cc-213">例</span><span class="sxs-lookup"><span data-stu-id="dd0cc-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd0cc-214">要求</span><span class="sxs-lookup"><span data-stu-id="dd0cc-214">Request</span></span>
<span data-ttu-id="dd0cc-215">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 849

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="dd0cc-216">応答</span><span class="sxs-lookup"><span data-stu-id="dd0cc-216">Response</span></span>
<span data-ttu-id="dd0cc-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dd0cc-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1021

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```


