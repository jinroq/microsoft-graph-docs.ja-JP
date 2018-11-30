---
title: windows81CompliancePolicy の更新
description: windows81CompliancePolicy オブジェクトのプロパティを更新します。
ms.openlocfilehash: 238d1f063e5c41f7f7622ef56bff69db29559631
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071284"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="9a96c-103">windows81CompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="9a96c-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="9a96c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9a96c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a96c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a96c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9a96c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9a96c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9a96c-107">[windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9a96c-107">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9a96c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9a96c-108">Prerequisites</span></span>
<span data-ttu-id="9a96c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a96c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a96c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9a96c-111">Permission type</span></span>|<span data-ttu-id="9a96c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9a96c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a96c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9a96c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a96c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a96c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a96c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a96c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a96c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a96c-116">Not supported.</span></span>|
|<span data-ttu-id="9a96c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a96c-117">Application</span></span>|<span data-ttu-id="9a96c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a96c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a96c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a96c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="9a96c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a96c-120">Request headers</span></span>
|<span data-ttu-id="9a96c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a96c-121">Header</span></span>|<span data-ttu-id="9a96c-122">値</span><span class="sxs-lookup"><span data-stu-id="9a96c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a96c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a96c-123">Authorization</span></span>|<span data-ttu-id="9a96c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9a96c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a96c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9a96c-125">Accept</span></span>|<span data-ttu-id="9a96c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a96c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a96c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9a96c-127">Request body</span></span>
<span data-ttu-id="9a96c-128">要求本文で、[windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="9a96c-128">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="9a96c-129">次の表に、[windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9a96c-129">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="9a96c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a96c-130">Property</span></span>|<span data-ttu-id="9a96c-131">型</span><span class="sxs-lookup"><span data-stu-id="9a96c-131">Type</span></span>|<span data-ttu-id="9a96c-132">説明</span><span class="sxs-lookup"><span data-stu-id="9a96c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a96c-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9a96c-133">roleScopeTagIds</span></span>|<span data-ttu-id="9a96c-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9a96c-134">String collection</span></span>|<span data-ttu-id="9a96c-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="9a96c-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9a96c-136">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a96c-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a96c-137">id</span><span class="sxs-lookup"><span data-stu-id="9a96c-137">id</span></span>|<span data-ttu-id="9a96c-138">String</span><span class="sxs-lookup"><span data-stu-id="9a96c-138">String</span></span>|<span data-ttu-id="9a96c-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9a96c-139">Key of the entity.</span></span> <span data-ttu-id="9a96c-140">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a96c-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a96c-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a96c-141">createdDateTime</span></span>|<span data-ttu-id="9a96c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a96c-142">DateTimeOffset</span></span>|<span data-ttu-id="9a96c-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9a96c-143">DateTime the object was created.</span></span> <span data-ttu-id="9a96c-144">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a96c-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a96c-145">説明</span><span class="sxs-lookup"><span data-stu-id="9a96c-145">description</span></span>|<span data-ttu-id="9a96c-146">String</span><span class="sxs-lookup"><span data-stu-id="9a96c-146">String</span></span>|<span data-ttu-id="9a96c-147">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="9a96c-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9a96c-148">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a96c-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a96c-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a96c-149">lastModifiedDateTime</span></span>|<span data-ttu-id="9a96c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a96c-150">DateTimeOffset</span></span>|<span data-ttu-id="9a96c-151">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9a96c-151">DateTime the object was last modified.</span></span> <span data-ttu-id="9a96c-152">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a96c-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a96c-153">displayName</span><span class="sxs-lookup"><span data-stu-id="9a96c-153">displayName</span></span>|<span data-ttu-id="9a96c-154">String</span><span class="sxs-lookup"><span data-stu-id="9a96c-154">String</span></span>|<span data-ttu-id="9a96c-155">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="9a96c-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9a96c-156">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a96c-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a96c-157">version</span><span class="sxs-lookup"><span data-stu-id="9a96c-157">version</span></span>|<span data-ttu-id="9a96c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="9a96c-158">Int32</span></span>|<span data-ttu-id="9a96c-159">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9a96c-159">Version of the device configuration.</span></span> <span data-ttu-id="9a96c-160">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9a96c-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a96c-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="9a96c-161">passwordRequired</span></span>|<span data-ttu-id="9a96c-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a96c-162">Boolean</span></span>|<span data-ttu-id="9a96c-163">Windows デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="9a96c-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="9a96c-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="9a96c-164">passwordBlockSimple</span></span>|<span data-ttu-id="9a96c-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a96c-165">Boolean</span></span>|<span data-ttu-id="9a96c-166">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9a96c-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="9a96c-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9a96c-167">passwordExpirationDays</span></span>|<span data-ttu-id="9a96c-168">Int32</span><span class="sxs-lookup"><span data-stu-id="9a96c-168">Int32</span></span>|<span data-ttu-id="9a96c-169">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="9a96c-169">Password expiration in days.</span></span>|
|<span data-ttu-id="9a96c-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9a96c-170">passwordMinimumLength</span></span>|<span data-ttu-id="9a96c-171">Int32</span><span class="sxs-lookup"><span data-stu-id="9a96c-171">Int32</span></span>|<span data-ttu-id="9a96c-172">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="9a96c-172">The minimum password length.</span></span>|
|<span data-ttu-id="9a96c-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="9a96c-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="9a96c-174">Int32</span><span class="sxs-lookup"><span data-stu-id="9a96c-174">Int32</span></span>|<span data-ttu-id="9a96c-175">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="9a96c-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="9a96c-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="9a96c-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="9a96c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9a96c-177">Int32</span></span>|<span data-ttu-id="9a96c-178">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="9a96c-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="9a96c-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9a96c-179">passwordRequiredType</span></span>|[<span data-ttu-id="9a96c-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9a96c-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="9a96c-181">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="9a96c-181">The required password type.</span></span> <span data-ttu-id="9a96c-182">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="9a96c-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="9a96c-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="9a96c-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="9a96c-184">Int32</span><span class="sxs-lookup"><span data-stu-id="9a96c-184">Int32</span></span>|<span data-ttu-id="9a96c-185">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="9a96c-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="9a96c-186">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="9a96c-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="9a96c-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="9a96c-187">osMinimumVersion</span></span>|<span data-ttu-id="9a96c-188">String</span><span class="sxs-lookup"><span data-stu-id="9a96c-188">String</span></span>|<span data-ttu-id="9a96c-189">Windows 8.1 の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="9a96c-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="9a96c-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="9a96c-190">osMaximumVersion</span></span>|<span data-ttu-id="9a96c-191">String</span><span class="sxs-lookup"><span data-stu-id="9a96c-191">String</span></span>|<span data-ttu-id="9a96c-192">Windows 8.1 の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="9a96c-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="9a96c-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="9a96c-193">storageRequireEncryption</span></span>|<span data-ttu-id="9a96c-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a96c-194">Boolean</span></span>|<span data-ttu-id="9a96c-195">Windows 8.1 のデバイスでの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9a96c-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="9a96c-196">応答</span><span class="sxs-lookup"><span data-stu-id="9a96c-196">Response</span></span>
<span data-ttu-id="9a96c-197">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="9a96c-197">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a96c-198">例</span><span class="sxs-lookup"><span data-stu-id="9a96c-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="9a96c-199">要求</span><span class="sxs-lookup"><span data-stu-id="9a96c-199">Request</span></span>
<span data-ttu-id="9a96c-200">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9a96c-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 664

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
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="9a96c-201">応答</span><span class="sxs-lookup"><span data-stu-id="9a96c-201">Response</span></span>
<span data-ttu-id="9a96c-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9a96c-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 836

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
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
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```





