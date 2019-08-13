---
title: windows81CompliancePolicy の作成
description: 新しい windows81CompliancePolicy オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0c6644d4d648c05d9deae69191e13ba9e583927e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36344855"
---
# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="7cef3-103">windows81CompliancePolicy の作成</span><span class="sxs-lookup"><span data-stu-id="7cef3-103">Create windows81CompliancePolicy</span></span>

> <span data-ttu-id="7cef3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cef3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7cef3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7cef3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cef3-106">新しい [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7cef3-106">Create a new [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7cef3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7cef3-107">Prerequisites</span></span>
<span data-ttu-id="7cef3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7cef3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cef3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7cef3-110">Permission type</span></span>|<span data-ttu-id="7cef3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7cef3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cef3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7cef3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7cef3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cef3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7cef3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7cef3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cef3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cef3-115">Not supported.</span></span>|
|<span data-ttu-id="7cef3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7cef3-116">Application</span></span>|<span data-ttu-id="7cef3-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cef3-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cef3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7cef3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="7cef3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7cef3-119">Request headers</span></span>
|<span data-ttu-id="7cef3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7cef3-120">Header</span></span>|<span data-ttu-id="7cef3-121">値</span><span class="sxs-lookup"><span data-stu-id="7cef3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cef3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cef3-122">Authorization</span></span>|<span data-ttu-id="7cef3-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7cef3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cef3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7cef3-124">Accept</span></span>|<span data-ttu-id="7cef3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7cef3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cef3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7cef3-126">Request body</span></span>
<span data-ttu-id="7cef3-127">要求本文で、windows81CompliancePolicy オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="7cef3-127">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="7cef3-128">次の表に、windows81CompliancePolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7cef3-128">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="7cef3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7cef3-129">Property</span></span>|<span data-ttu-id="7cef3-130">型</span><span class="sxs-lookup"><span data-stu-id="7cef3-130">Type</span></span>|<span data-ttu-id="7cef3-131">説明</span><span class="sxs-lookup"><span data-stu-id="7cef3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cef3-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7cef3-132">roleScopeTagIds</span></span>|<span data-ttu-id="7cef3-133">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="7cef3-133">String collection</span></span>|<span data-ttu-id="7cef3-134">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="7cef3-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7cef3-135">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7cef3-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7cef3-136">id</span><span class="sxs-lookup"><span data-stu-id="7cef3-136">id</span></span>|<span data-ttu-id="7cef3-137">文字列</span><span class="sxs-lookup"><span data-stu-id="7cef3-137">String</span></span>|<span data-ttu-id="7cef3-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7cef3-138">Key of the entity.</span></span> <span data-ttu-id="7cef3-139">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7cef3-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7cef3-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7cef3-140">createdDateTime</span></span>|<span data-ttu-id="7cef3-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cef3-141">DateTimeOffset</span></span>|<span data-ttu-id="7cef3-142">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7cef3-142">DateTime the object was created.</span></span> <span data-ttu-id="7cef3-143">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7cef3-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7cef3-144">description</span><span class="sxs-lookup"><span data-stu-id="7cef3-144">description</span></span>|<span data-ttu-id="7cef3-145">String</span><span class="sxs-lookup"><span data-stu-id="7cef3-145">String</span></span>|<span data-ttu-id="7cef3-146">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="7cef3-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7cef3-147">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7cef3-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7cef3-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7cef3-148">lastModifiedDateTime</span></span>|<span data-ttu-id="7cef3-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cef3-149">DateTimeOffset</span></span>|<span data-ttu-id="7cef3-150">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="7cef3-150">DateTime the object was last modified.</span></span> <span data-ttu-id="7cef3-151">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7cef3-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7cef3-152">displayName</span><span class="sxs-lookup"><span data-stu-id="7cef3-152">displayName</span></span>|<span data-ttu-id="7cef3-153">String</span><span class="sxs-lookup"><span data-stu-id="7cef3-153">String</span></span>|<span data-ttu-id="7cef3-154">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="7cef3-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7cef3-155">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7cef3-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7cef3-156">version</span><span class="sxs-lookup"><span data-stu-id="7cef3-156">version</span></span>|<span data-ttu-id="7cef3-157">Int32</span><span class="sxs-lookup"><span data-stu-id="7cef3-157">Int32</span></span>|<span data-ttu-id="7cef3-158">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7cef3-158">Version of the device configuration.</span></span> <span data-ttu-id="7cef3-159">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7cef3-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7cef3-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="7cef3-160">passwordRequired</span></span>|<span data-ttu-id="7cef3-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="7cef3-161">Boolean</span></span>|<span data-ttu-id="7cef3-162">Windows デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="7cef3-162">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="7cef3-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="7cef3-163">passwordBlockSimple</span></span>|<span data-ttu-id="7cef3-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="7cef3-164">Boolean</span></span>|<span data-ttu-id="7cef3-165">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7cef3-165">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="7cef3-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7cef3-166">passwordExpirationDays</span></span>|<span data-ttu-id="7cef3-167">Int32</span><span class="sxs-lookup"><span data-stu-id="7cef3-167">Int32</span></span>|<span data-ttu-id="7cef3-168">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="7cef3-168">Password expiration in days.</span></span>|
|<span data-ttu-id="7cef3-169">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7cef3-169">passwordMinimumLength</span></span>|<span data-ttu-id="7cef3-170">Int32</span><span class="sxs-lookup"><span data-stu-id="7cef3-170">Int32</span></span>|<span data-ttu-id="7cef3-171">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="7cef3-171">The minimum password length.</span></span>|
|<span data-ttu-id="7cef3-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="7cef3-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="7cef3-173">Int32</span><span class="sxs-lookup"><span data-stu-id="7cef3-173">Int32</span></span>|<span data-ttu-id="7cef3-174">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="7cef3-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="7cef3-175">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="7cef3-175">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="7cef3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="7cef3-176">Int32</span></span>|<span data-ttu-id="7cef3-177">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="7cef3-177">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="7cef3-178">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7cef3-178">passwordRequiredType</span></span>|[<span data-ttu-id="7cef3-179">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7cef3-179">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="7cef3-180">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="7cef3-180">The required password type.</span></span> <span data-ttu-id="7cef3-181">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="7cef3-181">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="7cef3-182">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7cef3-182">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7cef3-183">Int32</span><span class="sxs-lookup"><span data-stu-id="7cef3-183">Int32</span></span>|<span data-ttu-id="7cef3-184">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="7cef3-184">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="7cef3-185">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="7cef3-185">Valid values 0 to 24</span></span>|
|<span data-ttu-id="7cef3-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7cef3-186">osMinimumVersion</span></span>|<span data-ttu-id="7cef3-187">String</span><span class="sxs-lookup"><span data-stu-id="7cef3-187">String</span></span>|<span data-ttu-id="7cef3-188">Windows 8.1 の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="7cef3-188">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="7cef3-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7cef3-189">osMaximumVersion</span></span>|<span data-ttu-id="7cef3-190">String</span><span class="sxs-lookup"><span data-stu-id="7cef3-190">String</span></span>|<span data-ttu-id="7cef3-191">Windows 8.1 の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="7cef3-191">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="7cef3-192">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="7cef3-192">storageRequireEncryption</span></span>|<span data-ttu-id="7cef3-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="7cef3-193">Boolean</span></span>|<span data-ttu-id="7cef3-194">Windows 8.1 のデバイスでの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7cef3-194">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="7cef3-195">応答</span><span class="sxs-lookup"><span data-stu-id="7cef3-195">Response</span></span>
<span data-ttu-id="7cef3-196">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7cef3-196">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cef3-197">例</span><span class="sxs-lookup"><span data-stu-id="7cef3-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="7cef3-198">要求</span><span class="sxs-lookup"><span data-stu-id="7cef3-198">Request</span></span>
<span data-ttu-id="7cef3-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7cef3-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 664

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="7cef3-200">応答</span><span class="sxs-lookup"><span data-stu-id="7cef3-200">Response</span></span>
<span data-ttu-id="7cef3-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7cef3-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






