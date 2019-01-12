---
title: windowsPhone81CompliancePolicy の更新
description: windowsPhone81CompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6357ed5b20689dd5059d63869cf5b35e745bdf4d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938406"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="18f82-103">windowsPhone81CompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="18f82-103">Update windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="18f82-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="18f82-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18f82-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18f82-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18f82-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="18f82-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18f82-107">[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="18f82-107">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="18f82-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="18f82-108">Prerequisites</span></span>
<span data-ttu-id="18f82-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18f82-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18f82-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18f82-111">Permission type</span></span>|<span data-ttu-id="18f82-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="18f82-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18f82-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18f82-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18f82-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18f82-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="18f82-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18f82-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18f82-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18f82-116">Not supported.</span></span>|
|<span data-ttu-id="18f82-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18f82-117">Application</span></span>|<span data-ttu-id="18f82-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18f82-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18f82-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18f82-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="18f82-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18f82-120">Request headers</span></span>
|<span data-ttu-id="18f82-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18f82-121">Header</span></span>|<span data-ttu-id="18f82-122">値</span><span class="sxs-lookup"><span data-stu-id="18f82-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18f82-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18f82-123">Authorization</span></span>|<span data-ttu-id="18f82-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="18f82-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18f82-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18f82-125">Accept</span></span>|<span data-ttu-id="18f82-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18f82-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18f82-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="18f82-127">Request body</span></span>
<span data-ttu-id="18f82-128">要求本文で、[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="18f82-128">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="18f82-129">次の表に、[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="18f82-129">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="18f82-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18f82-130">Property</span></span>|<span data-ttu-id="18f82-131">型</span><span class="sxs-lookup"><span data-stu-id="18f82-131">Type</span></span>|<span data-ttu-id="18f82-132">説明</span><span class="sxs-lookup"><span data-stu-id="18f82-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18f82-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="18f82-133">roleScopeTagIds</span></span>|<span data-ttu-id="18f82-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="18f82-134">String collection</span></span>|<span data-ttu-id="18f82-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="18f82-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="18f82-136">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18f82-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="18f82-137">id</span><span class="sxs-lookup"><span data-stu-id="18f82-137">id</span></span>|<span data-ttu-id="18f82-138">String</span><span class="sxs-lookup"><span data-stu-id="18f82-138">String</span></span>|<span data-ttu-id="18f82-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="18f82-139">Key of the entity.</span></span> <span data-ttu-id="18f82-140">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18f82-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="18f82-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18f82-141">createdDateTime</span></span>|<span data-ttu-id="18f82-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18f82-142">DateTimeOffset</span></span>|<span data-ttu-id="18f82-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="18f82-143">DateTime the object was created.</span></span> <span data-ttu-id="18f82-144">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18f82-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="18f82-145">説明</span><span class="sxs-lookup"><span data-stu-id="18f82-145">description</span></span>|<span data-ttu-id="18f82-146">String</span><span class="sxs-lookup"><span data-stu-id="18f82-146">String</span></span>|<span data-ttu-id="18f82-147">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="18f82-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="18f82-148">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18f82-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="18f82-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18f82-149">lastModifiedDateTime</span></span>|<span data-ttu-id="18f82-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18f82-150">DateTimeOffset</span></span>|<span data-ttu-id="18f82-151">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="18f82-151">DateTime the object was last modified.</span></span> <span data-ttu-id="18f82-152">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18f82-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="18f82-153">displayName</span><span class="sxs-lookup"><span data-stu-id="18f82-153">displayName</span></span>|<span data-ttu-id="18f82-154">String</span><span class="sxs-lookup"><span data-stu-id="18f82-154">String</span></span>|<span data-ttu-id="18f82-155">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="18f82-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="18f82-156">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18f82-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="18f82-157">version</span><span class="sxs-lookup"><span data-stu-id="18f82-157">version</span></span>|<span data-ttu-id="18f82-158">Int32</span><span class="sxs-lookup"><span data-stu-id="18f82-158">Int32</span></span>|<span data-ttu-id="18f82-159">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="18f82-159">Version of the device configuration.</span></span> <span data-ttu-id="18f82-160">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="18f82-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="18f82-161">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="18f82-161">passwordBlockSimple</span></span>|<span data-ttu-id="18f82-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="18f82-162">Boolean</span></span>|<span data-ttu-id="18f82-163">カレンダーの同期を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="18f82-163">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="18f82-164">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="18f82-164">passwordExpirationDays</span></span>|<span data-ttu-id="18f82-165">Int32</span><span class="sxs-lookup"><span data-stu-id="18f82-165">Int32</span></span>|<span data-ttu-id="18f82-166">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="18f82-166">Number of days before the password expires.</span></span>|
|<span data-ttu-id="18f82-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="18f82-167">passwordMinimumLength</span></span>|<span data-ttu-id="18f82-168">Int32</span><span class="sxs-lookup"><span data-stu-id="18f82-168">Int32</span></span>|<span data-ttu-id="18f82-169">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="18f82-169">Minimum length of passwords.</span></span>|
|<span data-ttu-id="18f82-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="18f82-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="18f82-171">Int32</span><span class="sxs-lookup"><span data-stu-id="18f82-171">Int32</span></span>|<span data-ttu-id="18f82-172">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="18f82-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="18f82-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="18f82-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="18f82-174">Int32</span><span class="sxs-lookup"><span data-stu-id="18f82-174">Int32</span></span>|<span data-ttu-id="18f82-175">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="18f82-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="18f82-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="18f82-176">passwordRequiredType</span></span>|[<span data-ttu-id="18f82-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="18f82-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="18f82-178">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="18f82-178">The required password type.</span></span> <span data-ttu-id="18f82-179">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="18f82-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="18f82-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="18f82-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="18f82-181">Int32</span><span class="sxs-lookup"><span data-stu-id="18f82-181">Int32</span></span>|<span data-ttu-id="18f82-182">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="18f82-182">Number of previous passwords to block.</span></span> <span data-ttu-id="18f82-183">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="18f82-183">Valid values 0 to 24</span></span>|
|<span data-ttu-id="18f82-184">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="18f82-184">passwordRequired</span></span>|<span data-ttu-id="18f82-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="18f82-185">Boolean</span></span>|<span data-ttu-id="18f82-186">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="18f82-186">Whether or not to require a password.</span></span>|
|<span data-ttu-id="18f82-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="18f82-187">osMinimumVersion</span></span>|<span data-ttu-id="18f82-188">String</span><span class="sxs-lookup"><span data-stu-id="18f82-188">String</span></span>|<span data-ttu-id="18f82-189">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="18f82-189">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="18f82-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="18f82-190">osMaximumVersion</span></span>|<span data-ttu-id="18f82-191">String</span><span class="sxs-lookup"><span data-stu-id="18f82-191">String</span></span>|<span data-ttu-id="18f82-192">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="18f82-192">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="18f82-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="18f82-193">storageRequireEncryption</span></span>|<span data-ttu-id="18f82-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="18f82-194">Boolean</span></span>|<span data-ttu-id="18f82-195">Windows Phone デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="18f82-195">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="18f82-196">応答</span><span class="sxs-lookup"><span data-stu-id="18f82-196">Response</span></span>
<span data-ttu-id="18f82-197">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="18f82-197">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18f82-198">例</span><span class="sxs-lookup"><span data-stu-id="18f82-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="18f82-199">要求</span><span class="sxs-lookup"><span data-stu-id="18f82-199">Request</span></span>
<span data-ttu-id="18f82-200">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="18f82-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="18f82-201">応答</span><span class="sxs-lookup"><span data-stu-id="18f82-201">Response</span></span>
<span data-ttu-id="18f82-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="18f82-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 841

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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





