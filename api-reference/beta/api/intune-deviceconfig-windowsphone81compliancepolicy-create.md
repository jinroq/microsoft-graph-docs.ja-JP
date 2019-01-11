---
title: windowsPhone81CompliancePolicy の作成
description: 新しい windowsPhone81CompliancePolicy オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6ba95411610b8cc71917e344ad9d1d41b402be16
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812034"
---
# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="34746-103">windowsPhone81CompliancePolicy の作成</span><span class="sxs-lookup"><span data-stu-id="34746-103">Create windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="34746-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="34746-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34746-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34746-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34746-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="34746-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34746-107">新しい [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="34746-107">Create a new [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="34746-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="34746-108">Prerequisites</span></span>
<span data-ttu-id="34746-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34746-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34746-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="34746-111">Permission type</span></span>|<span data-ttu-id="34746-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="34746-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34746-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="34746-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34746-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34746-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34746-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="34746-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34746-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34746-116">Not supported.</span></span>|
|<span data-ttu-id="34746-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="34746-117">Application</span></span>|<span data-ttu-id="34746-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34746-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34746-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="34746-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="34746-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="34746-120">Request headers</span></span>
|<span data-ttu-id="34746-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="34746-121">Header</span></span>|<span data-ttu-id="34746-122">値</span><span class="sxs-lookup"><span data-stu-id="34746-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34746-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="34746-123">Authorization</span></span>|<span data-ttu-id="34746-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="34746-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34746-125">Accept</span><span class="sxs-lookup"><span data-stu-id="34746-125">Accept</span></span>|<span data-ttu-id="34746-126">application/json</span><span class="sxs-lookup"><span data-stu-id="34746-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34746-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="34746-127">Request body</span></span>
<span data-ttu-id="34746-128">要求本文で、windowsPhone81CompliancePolicy オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="34746-128">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="34746-129">次の表に、windowsPhone81CompliancePolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="34746-129">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="34746-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34746-130">Property</span></span>|<span data-ttu-id="34746-131">種類</span><span class="sxs-lookup"><span data-stu-id="34746-131">Type</span></span>|<span data-ttu-id="34746-132">説明</span><span class="sxs-lookup"><span data-stu-id="34746-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34746-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="34746-133">roleScopeTagIds</span></span>|<span data-ttu-id="34746-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="34746-134">String collection</span></span>|<span data-ttu-id="34746-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="34746-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="34746-136">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="34746-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34746-137">id</span><span class="sxs-lookup"><span data-stu-id="34746-137">id</span></span>|<span data-ttu-id="34746-138">String</span><span class="sxs-lookup"><span data-stu-id="34746-138">String</span></span>|<span data-ttu-id="34746-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="34746-139">Key of the entity.</span></span> <span data-ttu-id="34746-140">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="34746-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34746-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34746-141">createdDateTime</span></span>|<span data-ttu-id="34746-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34746-142">DateTimeOffset</span></span>|<span data-ttu-id="34746-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="34746-143">DateTime the object was created.</span></span> <span data-ttu-id="34746-144">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="34746-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34746-145">説明</span><span class="sxs-lookup"><span data-stu-id="34746-145">description</span></span>|<span data-ttu-id="34746-146">String</span><span class="sxs-lookup"><span data-stu-id="34746-146">String</span></span>|<span data-ttu-id="34746-147">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="34746-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="34746-148">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="34746-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34746-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34746-149">lastModifiedDateTime</span></span>|<span data-ttu-id="34746-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34746-150">DateTimeOffset</span></span>|<span data-ttu-id="34746-151">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="34746-151">DateTime the object was last modified.</span></span> <span data-ttu-id="34746-152">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="34746-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34746-153">displayName</span><span class="sxs-lookup"><span data-stu-id="34746-153">displayName</span></span>|<span data-ttu-id="34746-154">String</span><span class="sxs-lookup"><span data-stu-id="34746-154">String</span></span>|<span data-ttu-id="34746-155">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="34746-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="34746-156">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="34746-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34746-157">version</span><span class="sxs-lookup"><span data-stu-id="34746-157">version</span></span>|<span data-ttu-id="34746-158">Int32</span><span class="sxs-lookup"><span data-stu-id="34746-158">Int32</span></span>|<span data-ttu-id="34746-159">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="34746-159">Version of the device configuration.</span></span> <span data-ttu-id="34746-160">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="34746-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34746-161">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="34746-161">passwordBlockSimple</span></span>|<span data-ttu-id="34746-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="34746-162">Boolean</span></span>|<span data-ttu-id="34746-163">カレンダーの同期を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="34746-163">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="34746-164">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="34746-164">passwordExpirationDays</span></span>|<span data-ttu-id="34746-165">Int32</span><span class="sxs-lookup"><span data-stu-id="34746-165">Int32</span></span>|<span data-ttu-id="34746-166">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="34746-166">Number of days before the password expires.</span></span>|
|<span data-ttu-id="34746-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="34746-167">passwordMinimumLength</span></span>|<span data-ttu-id="34746-168">Int32</span><span class="sxs-lookup"><span data-stu-id="34746-168">Int32</span></span>|<span data-ttu-id="34746-169">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="34746-169">Minimum length of passwords.</span></span>|
|<span data-ttu-id="34746-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="34746-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="34746-171">Int32</span><span class="sxs-lookup"><span data-stu-id="34746-171">Int32</span></span>|<span data-ttu-id="34746-172">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="34746-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="34746-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="34746-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="34746-174">Int32</span><span class="sxs-lookup"><span data-stu-id="34746-174">Int32</span></span>|<span data-ttu-id="34746-175">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="34746-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="34746-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="34746-176">passwordRequiredType</span></span>|[<span data-ttu-id="34746-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="34746-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="34746-178">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="34746-178">The required password type.</span></span> <span data-ttu-id="34746-179">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="34746-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="34746-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="34746-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="34746-181">Int32</span><span class="sxs-lookup"><span data-stu-id="34746-181">Int32</span></span>|<span data-ttu-id="34746-182">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="34746-182">Number of previous passwords to block.</span></span> <span data-ttu-id="34746-183">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="34746-183">Valid values 0 to 24</span></span>|
|<span data-ttu-id="34746-184">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="34746-184">passwordRequired</span></span>|<span data-ttu-id="34746-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="34746-185">Boolean</span></span>|<span data-ttu-id="34746-186">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="34746-186">Whether or not to require a password.</span></span>|
|<span data-ttu-id="34746-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="34746-187">osMinimumVersion</span></span>|<span data-ttu-id="34746-188">String</span><span class="sxs-lookup"><span data-stu-id="34746-188">String</span></span>|<span data-ttu-id="34746-189">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="34746-189">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="34746-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="34746-190">osMaximumVersion</span></span>|<span data-ttu-id="34746-191">String</span><span class="sxs-lookup"><span data-stu-id="34746-191">String</span></span>|<span data-ttu-id="34746-192">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="34746-192">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="34746-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="34746-193">storageRequireEncryption</span></span>|<span data-ttu-id="34746-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="34746-194">Boolean</span></span>|<span data-ttu-id="34746-195">Windows Phone デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="34746-195">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="34746-196">応答</span><span class="sxs-lookup"><span data-stu-id="34746-196">Response</span></span>
<span data-ttu-id="34746-197">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="34746-197">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34746-198">例</span><span class="sxs-lookup"><span data-stu-id="34746-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="34746-199">要求</span><span class="sxs-lookup"><span data-stu-id="34746-199">Request</span></span>
<span data-ttu-id="34746-200">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="34746-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 733

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="34746-201">応答</span><span class="sxs-lookup"><span data-stu-id="34746-201">Response</span></span>
<span data-ttu-id="34746-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="34746-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





