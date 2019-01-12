---
title: windows81CompliancePolicy の更新
description: windows81CompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ecdd69fa115e4352b2470df263df83f889f8c36a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979363"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="ef9c0-103">windows81CompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="ef9c0-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="ef9c0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef9c0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef9c0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef9c0-107">[windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-107">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ef9c0-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ef9c0-108">Prerequisites</span></span>
<span data-ttu-id="ef9c0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef9c0-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ef9c0-111">Permission type</span></span>|<span data-ttu-id="ef9c0-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ef9c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef9c0-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ef9c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef9c0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef9c0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef9c0-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ef9c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef9c0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-116">Not supported.</span></span>|
|<span data-ttu-id="ef9c0-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ef9c0-117">Application</span></span>|<span data-ttu-id="ef9c0-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef9c0-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ef9c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="ef9c0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ef9c0-120">Request headers</span></span>
|<span data-ttu-id="ef9c0-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ef9c0-121">Header</span></span>|<span data-ttu-id="ef9c0-122">値</span><span class="sxs-lookup"><span data-stu-id="ef9c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef9c0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef9c0-123">Authorization</span></span>|<span data-ttu-id="ef9c0-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef9c0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ef9c0-125">Accept</span></span>|<span data-ttu-id="ef9c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef9c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef9c0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ef9c0-127">Request body</span></span>
<span data-ttu-id="ef9c0-128">要求本文で、[windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-128">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="ef9c0-129">次の表に、[windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-129">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="ef9c0-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef9c0-130">Property</span></span>|<span data-ttu-id="ef9c0-131">型</span><span class="sxs-lookup"><span data-stu-id="ef9c0-131">Type</span></span>|<span data-ttu-id="ef9c0-132">説明</span><span class="sxs-lookup"><span data-stu-id="ef9c0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef9c0-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ef9c0-133">roleScopeTagIds</span></span>|<span data-ttu-id="ef9c0-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ef9c0-134">String collection</span></span>|<span data-ttu-id="ef9c0-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ef9c0-136">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef9c0-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef9c0-137">id</span><span class="sxs-lookup"><span data-stu-id="ef9c0-137">id</span></span>|<span data-ttu-id="ef9c0-138">String</span><span class="sxs-lookup"><span data-stu-id="ef9c0-138">String</span></span>|<span data-ttu-id="ef9c0-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-139">Key of the entity.</span></span> <span data-ttu-id="ef9c0-140">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef9c0-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef9c0-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef9c0-141">createdDateTime</span></span>|<span data-ttu-id="ef9c0-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef9c0-142">DateTimeOffset</span></span>|<span data-ttu-id="ef9c0-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-143">DateTime the object was created.</span></span> <span data-ttu-id="ef9c0-144">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef9c0-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef9c0-145">説明</span><span class="sxs-lookup"><span data-stu-id="ef9c0-145">description</span></span>|<span data-ttu-id="ef9c0-146">String</span><span class="sxs-lookup"><span data-stu-id="ef9c0-146">String</span></span>|<span data-ttu-id="ef9c0-147">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ef9c0-148">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef9c0-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef9c0-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef9c0-149">lastModifiedDateTime</span></span>|<span data-ttu-id="ef9c0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef9c0-150">DateTimeOffset</span></span>|<span data-ttu-id="ef9c0-151">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-151">DateTime the object was last modified.</span></span> <span data-ttu-id="ef9c0-152">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef9c0-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef9c0-153">displayName</span><span class="sxs-lookup"><span data-stu-id="ef9c0-153">displayName</span></span>|<span data-ttu-id="ef9c0-154">String</span><span class="sxs-lookup"><span data-stu-id="ef9c0-154">String</span></span>|<span data-ttu-id="ef9c0-155">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ef9c0-156">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef9c0-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef9c0-157">version</span><span class="sxs-lookup"><span data-stu-id="ef9c0-157">version</span></span>|<span data-ttu-id="ef9c0-158">Int32</span><span class="sxs-lookup"><span data-stu-id="ef9c0-158">Int32</span></span>|<span data-ttu-id="ef9c0-159">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-159">Version of the device configuration.</span></span> <span data-ttu-id="ef9c0-160">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef9c0-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef9c0-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="ef9c0-161">passwordRequired</span></span>|<span data-ttu-id="ef9c0-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef9c0-162">Boolean</span></span>|<span data-ttu-id="ef9c0-163">Windows デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="ef9c0-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="ef9c0-164">passwordBlockSimple</span></span>|<span data-ttu-id="ef9c0-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef9c0-165">Boolean</span></span>|<span data-ttu-id="ef9c0-166">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="ef9c0-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ef9c0-167">passwordExpirationDays</span></span>|<span data-ttu-id="ef9c0-168">Int32</span><span class="sxs-lookup"><span data-stu-id="ef9c0-168">Int32</span></span>|<span data-ttu-id="ef9c0-169">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-169">Password expiration in days.</span></span>|
|<span data-ttu-id="ef9c0-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ef9c0-170">passwordMinimumLength</span></span>|<span data-ttu-id="ef9c0-171">Int32</span><span class="sxs-lookup"><span data-stu-id="ef9c0-171">Int32</span></span>|<span data-ttu-id="ef9c0-172">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-172">The minimum password length.</span></span>|
|<span data-ttu-id="ef9c0-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ef9c0-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ef9c0-174">Int32</span><span class="sxs-lookup"><span data-stu-id="ef9c0-174">Int32</span></span>|<span data-ttu-id="ef9c0-175">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="ef9c0-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ef9c0-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="ef9c0-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ef9c0-177">Int32</span></span>|<span data-ttu-id="ef9c0-178">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="ef9c0-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ef9c0-179">passwordRequiredType</span></span>|[<span data-ttu-id="ef9c0-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ef9c0-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="ef9c0-181">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-181">The required password type.</span></span> <span data-ttu-id="ef9c0-182">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ef9c0-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="ef9c0-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="ef9c0-184">Int32</span><span class="sxs-lookup"><span data-stu-id="ef9c0-184">Int32</span></span>|<span data-ttu-id="ef9c0-185">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="ef9c0-186">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="ef9c0-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="ef9c0-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ef9c0-187">osMinimumVersion</span></span>|<span data-ttu-id="ef9c0-188">String</span><span class="sxs-lookup"><span data-stu-id="ef9c0-188">String</span></span>|<span data-ttu-id="ef9c0-189">Windows 8.1 の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="ef9c0-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ef9c0-190">osMaximumVersion</span></span>|<span data-ttu-id="ef9c0-191">String</span><span class="sxs-lookup"><span data-stu-id="ef9c0-191">String</span></span>|<span data-ttu-id="ef9c0-192">Windows 8.1 の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="ef9c0-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="ef9c0-193">storageRequireEncryption</span></span>|<span data-ttu-id="ef9c0-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef9c0-194">Boolean</span></span>|<span data-ttu-id="ef9c0-195">Windows 8.1 のデバイスでの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="ef9c0-196">応答</span><span class="sxs-lookup"><span data-stu-id="ef9c0-196">Response</span></span>
<span data-ttu-id="ef9c0-197">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-197">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef9c0-198">例</span><span class="sxs-lookup"><span data-stu-id="ef9c0-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="ef9c0-199">要求</span><span class="sxs-lookup"><span data-stu-id="ef9c0-199">Request</span></span>
<span data-ttu-id="ef9c0-200">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ef9c0-201">応答</span><span class="sxs-lookup"><span data-stu-id="ef9c0-201">Response</span></span>
<span data-ttu-id="ef9c0-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ef9c0-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





