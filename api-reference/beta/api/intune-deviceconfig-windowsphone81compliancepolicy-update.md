---
title: windowsPhone81CompliancePolicy の更新
description: windowsPhone81CompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 804fdb19f5f9ba17afb3b8880f7b3ed602cdf197
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32513280"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="609bb-103">windowsPhone81CompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="609bb-103">Update windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="609bb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="609bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="609bb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="609bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="609bb-106">[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="609bb-106">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="609bb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="609bb-107">Prerequisites</span></span>
<span data-ttu-id="609bb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="609bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="609bb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="609bb-110">Permission type</span></span>|<span data-ttu-id="609bb-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="609bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="609bb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="609bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="609bb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="609bb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="609bb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="609bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="609bb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="609bb-115">Not supported.</span></span>|
|<span data-ttu-id="609bb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="609bb-116">Application</span></span>|<span data-ttu-id="609bb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="609bb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="609bb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="609bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="609bb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="609bb-119">Request headers</span></span>
|<span data-ttu-id="609bb-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="609bb-120">Header</span></span>|<span data-ttu-id="609bb-121">値</span><span class="sxs-lookup"><span data-stu-id="609bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="609bb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="609bb-122">Authorization</span></span>|<span data-ttu-id="609bb-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="609bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="609bb-124">承諾</span><span class="sxs-lookup"><span data-stu-id="609bb-124">Accept</span></span>|<span data-ttu-id="609bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="609bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="609bb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="609bb-126">Request body</span></span>
<span data-ttu-id="609bb-127">要求本文で、[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="609bb-127">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="609bb-128">次の表に、[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="609bb-128">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="609bb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="609bb-129">Property</span></span>|<span data-ttu-id="609bb-130">型</span><span class="sxs-lookup"><span data-stu-id="609bb-130">Type</span></span>|<span data-ttu-id="609bb-131">説明</span><span class="sxs-lookup"><span data-stu-id="609bb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="609bb-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="609bb-132">roleScopeTagIds</span></span>|<span data-ttu-id="609bb-133">String collection</span><span class="sxs-lookup"><span data-stu-id="609bb-133">String collection</span></span>|<span data-ttu-id="609bb-134">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="609bb-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="609bb-135">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="609bb-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="609bb-136">id</span><span class="sxs-lookup"><span data-stu-id="609bb-136">id</span></span>|<span data-ttu-id="609bb-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="609bb-137">String</span></span>|<span data-ttu-id="609bb-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="609bb-138">Key of the entity.</span></span> <span data-ttu-id="609bb-139">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="609bb-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="609bb-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="609bb-140">createdDateTime</span></span>|<span data-ttu-id="609bb-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="609bb-141">DateTimeOffset</span></span>|<span data-ttu-id="609bb-142">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="609bb-142">DateTime the object was created.</span></span> <span data-ttu-id="609bb-143">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="609bb-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="609bb-144">説明</span><span class="sxs-lookup"><span data-stu-id="609bb-144">description</span></span>|<span data-ttu-id="609bb-145">String</span><span class="sxs-lookup"><span data-stu-id="609bb-145">String</span></span>|<span data-ttu-id="609bb-146">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="609bb-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="609bb-147">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="609bb-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="609bb-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="609bb-148">lastModifiedDateTime</span></span>|<span data-ttu-id="609bb-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="609bb-149">DateTimeOffset</span></span>|<span data-ttu-id="609bb-150">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="609bb-150">DateTime the object was last modified.</span></span> <span data-ttu-id="609bb-151">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="609bb-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="609bb-152">displayName</span><span class="sxs-lookup"><span data-stu-id="609bb-152">displayName</span></span>|<span data-ttu-id="609bb-153">String</span><span class="sxs-lookup"><span data-stu-id="609bb-153">String</span></span>|<span data-ttu-id="609bb-154">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="609bb-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="609bb-155">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="609bb-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="609bb-156">version</span><span class="sxs-lookup"><span data-stu-id="609bb-156">version</span></span>|<span data-ttu-id="609bb-157">Int32</span><span class="sxs-lookup"><span data-stu-id="609bb-157">Int32</span></span>|<span data-ttu-id="609bb-158">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="609bb-158">Version of the device configuration.</span></span> <span data-ttu-id="609bb-159">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="609bb-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="609bb-160">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="609bb-160">passwordBlockSimple</span></span>|<span data-ttu-id="609bb-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="609bb-161">Boolean</span></span>|<span data-ttu-id="609bb-162">カレンダーの同期を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="609bb-162">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="609bb-163">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="609bb-163">passwordExpirationDays</span></span>|<span data-ttu-id="609bb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="609bb-164">Int32</span></span>|<span data-ttu-id="609bb-165">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="609bb-165">Number of days before the password expires.</span></span>|
|<span data-ttu-id="609bb-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="609bb-166">passwordMinimumLength</span></span>|<span data-ttu-id="609bb-167">Int32</span><span class="sxs-lookup"><span data-stu-id="609bb-167">Int32</span></span>|<span data-ttu-id="609bb-168">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="609bb-168">Minimum length of passwords.</span></span>|
|<span data-ttu-id="609bb-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="609bb-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="609bb-170">Int32</span><span class="sxs-lookup"><span data-stu-id="609bb-170">Int32</span></span>|<span data-ttu-id="609bb-171">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="609bb-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="609bb-172">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="609bb-172">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="609bb-173">Int32</span><span class="sxs-lookup"><span data-stu-id="609bb-173">Int32</span></span>|<span data-ttu-id="609bb-174">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="609bb-174">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="609bb-175">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="609bb-175">passwordRequiredType</span></span>|[<span data-ttu-id="609bb-176">requiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="609bb-176">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="609bb-177">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="609bb-177">The required password type.</span></span> <span data-ttu-id="609bb-178">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="609bb-178">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="609bb-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="609bb-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="609bb-180">Int32</span><span class="sxs-lookup"><span data-stu-id="609bb-180">Int32</span></span>|<span data-ttu-id="609bb-181">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="609bb-181">Number of previous passwords to block.</span></span> <span data-ttu-id="609bb-182">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="609bb-182">Valid values 0 to 24</span></span>|
|<span data-ttu-id="609bb-183">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="609bb-183">passwordRequired</span></span>|<span data-ttu-id="609bb-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="609bb-184">Boolean</span></span>|<span data-ttu-id="609bb-185">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="609bb-185">Whether or not to require a password.</span></span>|
|<span data-ttu-id="609bb-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="609bb-186">osMinimumVersion</span></span>|<span data-ttu-id="609bb-187">String</span><span class="sxs-lookup"><span data-stu-id="609bb-187">String</span></span>|<span data-ttu-id="609bb-188">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="609bb-188">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="609bb-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="609bb-189">osMaximumVersion</span></span>|<span data-ttu-id="609bb-190">String</span><span class="sxs-lookup"><span data-stu-id="609bb-190">String</span></span>|<span data-ttu-id="609bb-191">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="609bb-191">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="609bb-192">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="609bb-192">storageRequireEncryption</span></span>|<span data-ttu-id="609bb-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="609bb-193">Boolean</span></span>|<span data-ttu-id="609bb-194">Windows Phone デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="609bb-194">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="609bb-195">応答</span><span class="sxs-lookup"><span data-stu-id="609bb-195">Response</span></span>
<span data-ttu-id="609bb-196">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="609bb-196">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="609bb-197">例</span><span class="sxs-lookup"><span data-stu-id="609bb-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="609bb-198">要求</span><span class="sxs-lookup"><span data-stu-id="609bb-198">Request</span></span>
<span data-ttu-id="609bb-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="609bb-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 669

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="609bb-200">応答</span><span class="sxs-lookup"><span data-stu-id="609bb-200">Response</span></span>
<span data-ttu-id="609bb-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="609bb-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





