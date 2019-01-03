---
title: windowsPhone81CompliancePolicy の作成
description: 新しい windowsPhone81CompliancePolicy オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 689421dcc1a38d43fe6ebeef667df7d89312df9b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302395"
---
# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="6eea1-103">windowsPhone81CompliancePolicy の作成</span><span class="sxs-lookup"><span data-stu-id="6eea1-103">Create windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="6eea1-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6eea1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6eea1-105">新しい [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6eea1-105">Create a new [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6eea1-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6eea1-106">Prerequisites</span></span>
<span data-ttu-id="6eea1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6eea1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6eea1-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6eea1-109">Permission type</span></span>|<span data-ttu-id="6eea1-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6eea1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6eea1-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6eea1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6eea1-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6eea1-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6eea1-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6eea1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6eea1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6eea1-114">Not supported.</span></span>|
|<span data-ttu-id="6eea1-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6eea1-115">Application</span></span>|<span data-ttu-id="6eea1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6eea1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6eea1-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6eea1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="6eea1-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6eea1-118">Request headers</span></span>
|<span data-ttu-id="6eea1-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6eea1-119">Header</span></span>|<span data-ttu-id="6eea1-120">値</span><span class="sxs-lookup"><span data-stu-id="6eea1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6eea1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6eea1-121">Authorization</span></span>|<span data-ttu-id="6eea1-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6eea1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6eea1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6eea1-123">Accept</span></span>|<span data-ttu-id="6eea1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6eea1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6eea1-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6eea1-125">Request body</span></span>
<span data-ttu-id="6eea1-126">要求本文で、windowsPhone81CompliancePolicy オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6eea1-126">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="6eea1-127">次の表に、windowsPhone81CompliancePolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6eea1-127">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="6eea1-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6eea1-128">Property</span></span>|<span data-ttu-id="6eea1-129">種類</span><span class="sxs-lookup"><span data-stu-id="6eea1-129">Type</span></span>|<span data-ttu-id="6eea1-130">説明</span><span class="sxs-lookup"><span data-stu-id="6eea1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6eea1-131">ID</span><span class="sxs-lookup"><span data-stu-id="6eea1-131">id</span></span>|<span data-ttu-id="6eea1-132">String</span><span class="sxs-lookup"><span data-stu-id="6eea1-132">String</span></span>|<span data-ttu-id="6eea1-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6eea1-133">Key of the entity.</span></span> <span data-ttu-id="6eea1-134">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6eea1-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6eea1-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6eea1-135">createdDateTime</span></span>|<span data-ttu-id="6eea1-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6eea1-136">DateTimeOffset</span></span>|<span data-ttu-id="6eea1-137">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6eea1-137">DateTime the object was created.</span></span> <span data-ttu-id="6eea1-138">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6eea1-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6eea1-139">説明</span><span class="sxs-lookup"><span data-stu-id="6eea1-139">description</span></span>|<span data-ttu-id="6eea1-140">String</span><span class="sxs-lookup"><span data-stu-id="6eea1-140">String</span></span>|<span data-ttu-id="6eea1-141">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="6eea1-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6eea1-142">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6eea1-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6eea1-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6eea1-143">lastModifiedDateTime</span></span>|<span data-ttu-id="6eea1-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6eea1-144">DateTimeOffset</span></span>|<span data-ttu-id="6eea1-145">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6eea1-145">DateTime the object was last modified.</span></span> <span data-ttu-id="6eea1-146">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6eea1-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6eea1-147">displayName</span><span class="sxs-lookup"><span data-stu-id="6eea1-147">displayName</span></span>|<span data-ttu-id="6eea1-148">String</span><span class="sxs-lookup"><span data-stu-id="6eea1-148">String</span></span>|<span data-ttu-id="6eea1-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="6eea1-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6eea1-150">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6eea1-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6eea1-151">version</span><span class="sxs-lookup"><span data-stu-id="6eea1-151">version</span></span>|<span data-ttu-id="6eea1-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6eea1-152">Int32</span></span>|<span data-ttu-id="6eea1-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="6eea1-153">Version of the device configuration.</span></span> <span data-ttu-id="6eea1-154">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6eea1-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6eea1-155">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6eea1-155">passwordBlockSimple</span></span>|<span data-ttu-id="6eea1-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="6eea1-156">Boolean</span></span>|<span data-ttu-id="6eea1-157">カレンダーの同期を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6eea1-157">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="6eea1-158">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6eea1-158">passwordExpirationDays</span></span>|<span data-ttu-id="6eea1-159">Int32</span><span class="sxs-lookup"><span data-stu-id="6eea1-159">Int32</span></span>|<span data-ttu-id="6eea1-160">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="6eea1-160">Number of days before the password expires.</span></span>|
|<span data-ttu-id="6eea1-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6eea1-161">passwordMinimumLength</span></span>|<span data-ttu-id="6eea1-162">Int32</span><span class="sxs-lookup"><span data-stu-id="6eea1-162">Int32</span></span>|<span data-ttu-id="6eea1-163">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="6eea1-163">Minimum length of passwords.</span></span>|
|<span data-ttu-id="6eea1-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6eea1-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6eea1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6eea1-165">Int32</span></span>|<span data-ttu-id="6eea1-166">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="6eea1-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="6eea1-167">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6eea1-167">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="6eea1-168">Int32</span><span class="sxs-lookup"><span data-stu-id="6eea1-168">Int32</span></span>|<span data-ttu-id="6eea1-169">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="6eea1-169">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="6eea1-170">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6eea1-170">passwordRequiredType</span></span>|[<span data-ttu-id="6eea1-171">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6eea1-171">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6eea1-172">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="6eea1-172">The required password type.</span></span> <span data-ttu-id="6eea1-173">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="6eea1-173">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6eea1-174">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6eea1-174">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6eea1-175">Int32</span><span class="sxs-lookup"><span data-stu-id="6eea1-175">Int32</span></span>|<span data-ttu-id="6eea1-176">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="6eea1-176">Number of previous passwords to block.</span></span> <span data-ttu-id="6eea1-177">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="6eea1-177">Valid values 0 to 24</span></span>|
|<span data-ttu-id="6eea1-178">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6eea1-178">passwordRequired</span></span>|<span data-ttu-id="6eea1-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="6eea1-179">Boolean</span></span>|<span data-ttu-id="6eea1-180">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6eea1-180">Whether or not to require a password.</span></span>|
|<span data-ttu-id="6eea1-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6eea1-181">osMinimumVersion</span></span>|<span data-ttu-id="6eea1-182">String</span><span class="sxs-lookup"><span data-stu-id="6eea1-182">String</span></span>|<span data-ttu-id="6eea1-183">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="6eea1-183">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="6eea1-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6eea1-184">osMaximumVersion</span></span>|<span data-ttu-id="6eea1-185">String</span><span class="sxs-lookup"><span data-stu-id="6eea1-185">String</span></span>|<span data-ttu-id="6eea1-186">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="6eea1-186">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="6eea1-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="6eea1-187">storageRequireEncryption</span></span>|<span data-ttu-id="6eea1-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="6eea1-188">Boolean</span></span>|<span data-ttu-id="6eea1-189">Windows Phone デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="6eea1-189">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="6eea1-190">応答</span><span class="sxs-lookup"><span data-stu-id="6eea1-190">Response</span></span>
<span data-ttu-id="6eea1-191">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6eea1-191">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6eea1-192">例</span><span class="sxs-lookup"><span data-stu-id="6eea1-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="6eea1-193">要求</span><span class="sxs-lookup"><span data-stu-id="6eea1-193">Request</span></span>
<span data-ttu-id="6eea1-194">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6eea1-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="6eea1-195">応答</span><span class="sxs-lookup"><span data-stu-id="6eea1-195">Response</span></span>
<span data-ttu-id="6eea1-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6eea1-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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


