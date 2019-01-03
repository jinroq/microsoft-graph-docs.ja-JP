---
title: windowsPhone81CompliancePolicy の更新
description: windowsPhone81CompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: b017d25570b3cd220fa150b1be49516c02e3467a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362343"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="6ba99-103">windowsPhone81CompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="6ba99-103">Update windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="6ba99-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6ba99-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ba99-105">[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6ba99-105">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6ba99-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6ba99-106">Prerequisites</span></span>
<span data-ttu-id="6ba99-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6ba99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ba99-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6ba99-109">Permission type</span></span>|<span data-ttu-id="6ba99-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6ba99-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ba99-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6ba99-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6ba99-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ba99-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ba99-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6ba99-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ba99-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ba99-114">Not supported.</span></span>|
|<span data-ttu-id="6ba99-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6ba99-115">Application</span></span>|<span data-ttu-id="6ba99-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ba99-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ba99-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6ba99-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="6ba99-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ba99-118">Request headers</span></span>
|<span data-ttu-id="6ba99-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ba99-119">Header</span></span>|<span data-ttu-id="6ba99-120">値</span><span class="sxs-lookup"><span data-stu-id="6ba99-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ba99-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ba99-121">Authorization</span></span>|<span data-ttu-id="6ba99-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6ba99-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ba99-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6ba99-123">Accept</span></span>|<span data-ttu-id="6ba99-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6ba99-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ba99-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6ba99-125">Request body</span></span>
<span data-ttu-id="6ba99-126">要求本文で、[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6ba99-126">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="6ba99-127">次の表に、[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6ba99-127">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="6ba99-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ba99-128">Property</span></span>|<span data-ttu-id="6ba99-129">種類</span><span class="sxs-lookup"><span data-stu-id="6ba99-129">Type</span></span>|<span data-ttu-id="6ba99-130">説明</span><span class="sxs-lookup"><span data-stu-id="6ba99-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ba99-131">ID</span><span class="sxs-lookup"><span data-stu-id="6ba99-131">id</span></span>|<span data-ttu-id="6ba99-132">String</span><span class="sxs-lookup"><span data-stu-id="6ba99-132">String</span></span>|<span data-ttu-id="6ba99-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6ba99-133">Key of the entity.</span></span> <span data-ttu-id="6ba99-134">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ba99-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6ba99-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6ba99-135">createdDateTime</span></span>|<span data-ttu-id="6ba99-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ba99-136">DateTimeOffset</span></span>|<span data-ttu-id="6ba99-137">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6ba99-137">DateTime the object was created.</span></span> <span data-ttu-id="6ba99-138">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ba99-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6ba99-139">説明</span><span class="sxs-lookup"><span data-stu-id="6ba99-139">description</span></span>|<span data-ttu-id="6ba99-140">String</span><span class="sxs-lookup"><span data-stu-id="6ba99-140">String</span></span>|<span data-ttu-id="6ba99-141">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="6ba99-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6ba99-142">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ba99-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6ba99-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ba99-143">lastModifiedDateTime</span></span>|<span data-ttu-id="6ba99-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ba99-144">DateTimeOffset</span></span>|<span data-ttu-id="6ba99-145">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6ba99-145">DateTime the object was last modified.</span></span> <span data-ttu-id="6ba99-146">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ba99-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6ba99-147">displayName</span><span class="sxs-lookup"><span data-stu-id="6ba99-147">displayName</span></span>|<span data-ttu-id="6ba99-148">String</span><span class="sxs-lookup"><span data-stu-id="6ba99-148">String</span></span>|<span data-ttu-id="6ba99-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="6ba99-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6ba99-150">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ba99-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6ba99-151">version</span><span class="sxs-lookup"><span data-stu-id="6ba99-151">version</span></span>|<span data-ttu-id="6ba99-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6ba99-152">Int32</span></span>|<span data-ttu-id="6ba99-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="6ba99-153">Version of the device configuration.</span></span> <span data-ttu-id="6ba99-154">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ba99-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6ba99-155">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6ba99-155">passwordBlockSimple</span></span>|<span data-ttu-id="6ba99-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ba99-156">Boolean</span></span>|<span data-ttu-id="6ba99-157">カレンダーの同期を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6ba99-157">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="6ba99-158">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6ba99-158">passwordExpirationDays</span></span>|<span data-ttu-id="6ba99-159">Int32</span><span class="sxs-lookup"><span data-stu-id="6ba99-159">Int32</span></span>|<span data-ttu-id="6ba99-160">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="6ba99-160">Number of days before the password expires.</span></span>|
|<span data-ttu-id="6ba99-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6ba99-161">passwordMinimumLength</span></span>|<span data-ttu-id="6ba99-162">Int32</span><span class="sxs-lookup"><span data-stu-id="6ba99-162">Int32</span></span>|<span data-ttu-id="6ba99-163">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="6ba99-163">Minimum length of passwords.</span></span>|
|<span data-ttu-id="6ba99-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6ba99-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6ba99-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6ba99-165">Int32</span></span>|<span data-ttu-id="6ba99-166">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="6ba99-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="6ba99-167">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6ba99-167">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="6ba99-168">Int32</span><span class="sxs-lookup"><span data-stu-id="6ba99-168">Int32</span></span>|<span data-ttu-id="6ba99-169">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="6ba99-169">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="6ba99-170">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6ba99-170">passwordRequiredType</span></span>|[<span data-ttu-id="6ba99-171">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6ba99-171">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6ba99-172">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="6ba99-172">The required password type.</span></span> <span data-ttu-id="6ba99-173">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="6ba99-173">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6ba99-174">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6ba99-174">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6ba99-175">Int32</span><span class="sxs-lookup"><span data-stu-id="6ba99-175">Int32</span></span>|<span data-ttu-id="6ba99-176">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="6ba99-176">Number of previous passwords to block.</span></span> <span data-ttu-id="6ba99-177">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="6ba99-177">Valid values 0 to 24</span></span>|
|<span data-ttu-id="6ba99-178">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6ba99-178">passwordRequired</span></span>|<span data-ttu-id="6ba99-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ba99-179">Boolean</span></span>|<span data-ttu-id="6ba99-180">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6ba99-180">Whether or not to require a password.</span></span>|
|<span data-ttu-id="6ba99-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6ba99-181">osMinimumVersion</span></span>|<span data-ttu-id="6ba99-182">String</span><span class="sxs-lookup"><span data-stu-id="6ba99-182">String</span></span>|<span data-ttu-id="6ba99-183">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="6ba99-183">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="6ba99-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6ba99-184">osMaximumVersion</span></span>|<span data-ttu-id="6ba99-185">String</span><span class="sxs-lookup"><span data-stu-id="6ba99-185">String</span></span>|<span data-ttu-id="6ba99-186">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="6ba99-186">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="6ba99-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="6ba99-187">storageRequireEncryption</span></span>|<span data-ttu-id="6ba99-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ba99-188">Boolean</span></span>|<span data-ttu-id="6ba99-189">Windows Phone デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="6ba99-189">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="6ba99-190">応答</span><span class="sxs-lookup"><span data-stu-id="6ba99-190">Response</span></span>
<span data-ttu-id="6ba99-191">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6ba99-191">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ba99-192">例</span><span class="sxs-lookup"><span data-stu-id="6ba99-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="6ba99-193">要求</span><span class="sxs-lookup"><span data-stu-id="6ba99-193">Request</span></span>
<span data-ttu-id="6ba99-194">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6ba99-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 607

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="6ba99-195">応答</span><span class="sxs-lookup"><span data-stu-id="6ba99-195">Response</span></span>
<span data-ttu-id="6ba99-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6ba99-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 779

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```


