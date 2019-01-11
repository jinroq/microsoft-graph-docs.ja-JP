---
title: Create iosCompliancePolicy
description: 新しい iosCompliancePolicy オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: df69e8512a1f8e900f1e3751d5943f4ea8e6a215
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834462"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="11de0-103">Create iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="11de0-103">Create iosCompliancePolicy</span></span>

> <span data-ttu-id="11de0-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="11de0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11de0-105">新しい [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="11de0-105">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="11de0-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="11de0-106">Prerequisites</span></span>
<span data-ttu-id="11de0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11de0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11de0-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="11de0-109">Permission type</span></span>|<span data-ttu-id="11de0-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="11de0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11de0-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="11de0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="11de0-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11de0-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="11de0-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="11de0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11de0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11de0-114">Not supported.</span></span>|
|<span data-ttu-id="11de0-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="11de0-115">Application</span></span>|<span data-ttu-id="11de0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11de0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11de0-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="11de0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="11de0-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11de0-118">Request headers</span></span>
|<span data-ttu-id="11de0-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11de0-119">Header</span></span>|<span data-ttu-id="11de0-120">値</span><span class="sxs-lookup"><span data-stu-id="11de0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11de0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="11de0-121">Authorization</span></span>|<span data-ttu-id="11de0-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="11de0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11de0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="11de0-123">Accept</span></span>|<span data-ttu-id="11de0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="11de0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11de0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="11de0-125">Request body</span></span>
<span data-ttu-id="11de0-126">要求本文で、iosCompliancePolicy オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="11de0-126">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="11de0-127">次の表に、iosCompliancePolicy 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="11de0-127">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="11de0-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="11de0-128">Property</span></span>|<span data-ttu-id="11de0-129">種類</span><span class="sxs-lookup"><span data-stu-id="11de0-129">Type</span></span>|<span data-ttu-id="11de0-130">説明</span><span class="sxs-lookup"><span data-stu-id="11de0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11de0-131">ID</span><span class="sxs-lookup"><span data-stu-id="11de0-131">id</span></span>|<span data-ttu-id="11de0-132">String</span><span class="sxs-lookup"><span data-stu-id="11de0-132">String</span></span>|<span data-ttu-id="11de0-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="11de0-133">Key of the entity.</span></span> <span data-ttu-id="11de0-134">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11de0-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="11de0-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11de0-135">createdDateTime</span></span>|<span data-ttu-id="11de0-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11de0-136">DateTimeOffset</span></span>|<span data-ttu-id="11de0-137">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="11de0-137">DateTime the object was created.</span></span> <span data-ttu-id="11de0-138">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11de0-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="11de0-139">説明</span><span class="sxs-lookup"><span data-stu-id="11de0-139">description</span></span>|<span data-ttu-id="11de0-140">String</span><span class="sxs-lookup"><span data-stu-id="11de0-140">String</span></span>|<span data-ttu-id="11de0-141">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="11de0-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="11de0-142">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11de0-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="11de0-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11de0-143">lastModifiedDateTime</span></span>|<span data-ttu-id="11de0-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11de0-144">DateTimeOffset</span></span>|<span data-ttu-id="11de0-145">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="11de0-145">DateTime the object was last modified.</span></span> <span data-ttu-id="11de0-146">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11de0-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="11de0-147">displayName</span><span class="sxs-lookup"><span data-stu-id="11de0-147">displayName</span></span>|<span data-ttu-id="11de0-148">String</span><span class="sxs-lookup"><span data-stu-id="11de0-148">String</span></span>|<span data-ttu-id="11de0-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="11de0-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="11de0-150">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11de0-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="11de0-151">version</span><span class="sxs-lookup"><span data-stu-id="11de0-151">version</span></span>|<span data-ttu-id="11de0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="11de0-152">Int32</span></span>|<span data-ttu-id="11de0-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="11de0-153">Version of the device configuration.</span></span> <span data-ttu-id="11de0-154">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="11de0-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="11de0-155">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="11de0-155">passcodeBlockSimple</span></span>|<span data-ttu-id="11de0-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="11de0-156">Boolean</span></span>|<span data-ttu-id="11de0-157">単純なパスコードを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="11de0-157">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="11de0-158">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="11de0-158">passcodeExpirationDays</span></span>|<span data-ttu-id="11de0-159">Int32</span><span class="sxs-lookup"><span data-stu-id="11de0-159">Int32</span></span>|<span data-ttu-id="11de0-160">パスコードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="11de0-160">Number of days before the passcode expires.</span></span> <span data-ttu-id="11de0-161">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="11de0-161">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="11de0-162">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="11de0-162">passcodeMinimumLength</span></span>|<span data-ttu-id="11de0-163">Int32</span><span class="sxs-lookup"><span data-stu-id="11de0-163">Int32</span></span>|<span data-ttu-id="11de0-164">パスコードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="11de0-164">Minimum length of passcode.</span></span> <span data-ttu-id="11de0-165">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="11de0-165">Valid values 4 to 14</span></span>|
|<span data-ttu-id="11de0-166">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="11de0-166">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="11de0-167">Int32</span><span class="sxs-lookup"><span data-stu-id="11de0-167">Int32</span></span>|<span data-ttu-id="11de0-168">パスコードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="11de0-168">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="11de0-169">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="11de0-169">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="11de0-170">Int32</span><span class="sxs-lookup"><span data-stu-id="11de0-170">Int32</span></span>|<span data-ttu-id="11de0-171">ブロックする、以前のパスコードの数。</span><span class="sxs-lookup"><span data-stu-id="11de0-171">Number of previous passcodes to block.</span></span> <span data-ttu-id="11de0-172">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="11de0-172">Valid values 1 to 24</span></span>|
|<span data-ttu-id="11de0-173">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="11de0-173">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="11de0-174">Int32</span><span class="sxs-lookup"><span data-stu-id="11de0-174">Int32</span></span>|<span data-ttu-id="11de0-175">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="11de0-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="11de0-176">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="11de0-176">passcodeRequiredType</span></span>|[<span data-ttu-id="11de0-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="11de0-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="11de0-178">要求されるパスコードの種類。</span><span class="sxs-lookup"><span data-stu-id="11de0-178">The required passcode type.</span></span> <span data-ttu-id="11de0-179">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="11de0-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="11de0-180">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="11de0-180">passcodeRequired</span></span>|<span data-ttu-id="11de0-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="11de0-181">Boolean</span></span>|<span data-ttu-id="11de0-182">パスコードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="11de0-182">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="11de0-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="11de0-183">osMinimumVersion</span></span>|<span data-ttu-id="11de0-184">String</span><span class="sxs-lookup"><span data-stu-id="11de0-184">String</span></span>|<span data-ttu-id="11de0-185">最低限必要な iOS のバージョン。</span><span class="sxs-lookup"><span data-stu-id="11de0-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="11de0-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="11de0-186">osMaximumVersion</span></span>|<span data-ttu-id="11de0-187">String</span><span class="sxs-lookup"><span data-stu-id="11de0-187">String</span></span>|<span data-ttu-id="11de0-188">iOS の最高バージョン。</span><span class="sxs-lookup"><span data-stu-id="11de0-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="11de0-189">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="11de0-189">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="11de0-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="11de0-190">Boolean</span></span>|<span data-ttu-id="11de0-191">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="11de0-191">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="11de0-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="11de0-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="11de0-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="11de0-193">Boolean</span></span>|<span data-ttu-id="11de0-194">デバイスへの脅威に対する保護が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="11de0-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="11de0-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="11de0-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="11de0-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="11de0-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="11de0-197">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="11de0-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="11de0-198">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="11de0-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="11de0-199">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="11de0-199">managedEmailProfileRequired</span></span>|<span data-ttu-id="11de0-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="11de0-200">Boolean</span></span>|<span data-ttu-id="11de0-201">管理された電子メール プロファイルを必要とするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="11de0-201">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="11de0-202">応答</span><span class="sxs-lookup"><span data-stu-id="11de0-202">Response</span></span>
<span data-ttu-id="11de0-203">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="11de0-203">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11de0-204">例</span><span class="sxs-lookup"><span data-stu-id="11de0-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="11de0-205">要求</span><span class="sxs-lookup"><span data-stu-id="11de0-205">Request</span></span>
<span data-ttu-id="11de0-206">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="11de0-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 745

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```

### <a name="response"></a><span data-ttu-id="11de0-207">応答</span><span class="sxs-lookup"><span data-stu-id="11de0-207">Response</span></span>
<span data-ttu-id="11de0-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="11de0-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 917

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "id": "4f501351-1351-4f50-5113-504f5113504f",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```



