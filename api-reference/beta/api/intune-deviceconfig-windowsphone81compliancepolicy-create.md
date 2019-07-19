---
title: windowsPhone81CompliancePolicy の作成
description: 新しい windowsPhone81CompliancePolicy オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 44ae3c154d11215cbc1e0d741fd04f43d4090ca1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961764"
---
# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="6cc34-103">windowsPhone81CompliancePolicy の作成</span><span class="sxs-lookup"><span data-stu-id="6cc34-103">Create windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="6cc34-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cc34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cc34-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6cc34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cc34-106">新しい [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6cc34-106">Create a new [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cc34-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6cc34-107">Prerequisites</span></span>
<span data-ttu-id="6cc34-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6cc34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cc34-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6cc34-110">Permission type</span></span>|<span data-ttu-id="6cc34-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6cc34-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cc34-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6cc34-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6cc34-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cc34-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6cc34-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6cc34-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cc34-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cc34-115">Not supported.</span></span>|
|<span data-ttu-id="6cc34-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6cc34-116">Application</span></span>|<span data-ttu-id="6cc34-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cc34-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cc34-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6cc34-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="6cc34-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6cc34-119">Request headers</span></span>
|<span data-ttu-id="6cc34-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6cc34-120">Header</span></span>|<span data-ttu-id="6cc34-121">値</span><span class="sxs-lookup"><span data-stu-id="6cc34-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cc34-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cc34-122">Authorization</span></span>|<span data-ttu-id="6cc34-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6cc34-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cc34-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6cc34-124">Accept</span></span>|<span data-ttu-id="6cc34-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6cc34-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cc34-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6cc34-126">Request body</span></span>
<span data-ttu-id="6cc34-127">要求本文で、windowsPhone81CompliancePolicy オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6cc34-127">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="6cc34-128">次の表に、windowsPhone81CompliancePolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6cc34-128">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="6cc34-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6cc34-129">Property</span></span>|<span data-ttu-id="6cc34-130">型</span><span class="sxs-lookup"><span data-stu-id="6cc34-130">Type</span></span>|<span data-ttu-id="6cc34-131">説明</span><span class="sxs-lookup"><span data-stu-id="6cc34-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cc34-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6cc34-132">roleScopeTagIds</span></span>|<span data-ttu-id="6cc34-133">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="6cc34-133">String collection</span></span>|<span data-ttu-id="6cc34-134">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="6cc34-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6cc34-135">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cc34-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6cc34-136">id</span><span class="sxs-lookup"><span data-stu-id="6cc34-136">id</span></span>|<span data-ttu-id="6cc34-137">文字列</span><span class="sxs-lookup"><span data-stu-id="6cc34-137">String</span></span>|<span data-ttu-id="6cc34-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6cc34-138">Key of the entity.</span></span> <span data-ttu-id="6cc34-139">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cc34-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6cc34-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6cc34-140">createdDateTime</span></span>|<span data-ttu-id="6cc34-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cc34-141">DateTimeOffset</span></span>|<span data-ttu-id="6cc34-142">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6cc34-142">DateTime the object was created.</span></span> <span data-ttu-id="6cc34-143">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cc34-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6cc34-144">description</span><span class="sxs-lookup"><span data-stu-id="6cc34-144">description</span></span>|<span data-ttu-id="6cc34-145">String</span><span class="sxs-lookup"><span data-stu-id="6cc34-145">String</span></span>|<span data-ttu-id="6cc34-146">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="6cc34-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6cc34-147">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cc34-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6cc34-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6cc34-148">lastModifiedDateTime</span></span>|<span data-ttu-id="6cc34-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cc34-149">DateTimeOffset</span></span>|<span data-ttu-id="6cc34-150">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="6cc34-150">DateTime the object was last modified.</span></span> <span data-ttu-id="6cc34-151">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cc34-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6cc34-152">displayName</span><span class="sxs-lookup"><span data-stu-id="6cc34-152">displayName</span></span>|<span data-ttu-id="6cc34-153">String</span><span class="sxs-lookup"><span data-stu-id="6cc34-153">String</span></span>|<span data-ttu-id="6cc34-154">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="6cc34-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6cc34-155">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cc34-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6cc34-156">version</span><span class="sxs-lookup"><span data-stu-id="6cc34-156">version</span></span>|<span data-ttu-id="6cc34-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6cc34-157">Int32</span></span>|<span data-ttu-id="6cc34-158">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="6cc34-158">Version of the device configuration.</span></span> <span data-ttu-id="6cc34-159">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cc34-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6cc34-160">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6cc34-160">passwordBlockSimple</span></span>|<span data-ttu-id="6cc34-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cc34-161">Boolean</span></span>|<span data-ttu-id="6cc34-162">カレンダーの同期を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6cc34-162">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="6cc34-163">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6cc34-163">passwordExpirationDays</span></span>|<span data-ttu-id="6cc34-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6cc34-164">Int32</span></span>|<span data-ttu-id="6cc34-165">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="6cc34-165">Number of days before the password expires.</span></span>|
|<span data-ttu-id="6cc34-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6cc34-166">passwordMinimumLength</span></span>|<span data-ttu-id="6cc34-167">Int32</span><span class="sxs-lookup"><span data-stu-id="6cc34-167">Int32</span></span>|<span data-ttu-id="6cc34-168">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="6cc34-168">Minimum length of passwords.</span></span>|
|<span data-ttu-id="6cc34-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6cc34-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6cc34-170">Int32</span><span class="sxs-lookup"><span data-stu-id="6cc34-170">Int32</span></span>|<span data-ttu-id="6cc34-171">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="6cc34-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="6cc34-172">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6cc34-172">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="6cc34-173">Int32</span><span class="sxs-lookup"><span data-stu-id="6cc34-173">Int32</span></span>|<span data-ttu-id="6cc34-174">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="6cc34-174">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="6cc34-175">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6cc34-175">passwordRequiredType</span></span>|[<span data-ttu-id="6cc34-176">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6cc34-176">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6cc34-177">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="6cc34-177">The required password type.</span></span> <span data-ttu-id="6cc34-178">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="6cc34-178">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6cc34-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6cc34-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6cc34-180">Int32</span><span class="sxs-lookup"><span data-stu-id="6cc34-180">Int32</span></span>|<span data-ttu-id="6cc34-181">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="6cc34-181">Number of previous passwords to block.</span></span> <span data-ttu-id="6cc34-182">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="6cc34-182">Valid values 0 to 24</span></span>|
|<span data-ttu-id="6cc34-183">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6cc34-183">passwordRequired</span></span>|<span data-ttu-id="6cc34-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cc34-184">Boolean</span></span>|<span data-ttu-id="6cc34-185">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6cc34-185">Whether or not to require a password.</span></span>|
|<span data-ttu-id="6cc34-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6cc34-186">osMinimumVersion</span></span>|<span data-ttu-id="6cc34-187">String</span><span class="sxs-lookup"><span data-stu-id="6cc34-187">String</span></span>|<span data-ttu-id="6cc34-188">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="6cc34-188">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="6cc34-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6cc34-189">osMaximumVersion</span></span>|<span data-ttu-id="6cc34-190">String</span><span class="sxs-lookup"><span data-stu-id="6cc34-190">String</span></span>|<span data-ttu-id="6cc34-191">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="6cc34-191">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="6cc34-192">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="6cc34-192">storageRequireEncryption</span></span>|<span data-ttu-id="6cc34-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cc34-193">Boolean</span></span>|<span data-ttu-id="6cc34-194">Windows Phone デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="6cc34-194">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="6cc34-195">応答</span><span class="sxs-lookup"><span data-stu-id="6cc34-195">Response</span></span>
<span data-ttu-id="6cc34-196">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6cc34-196">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cc34-197">例</span><span class="sxs-lookup"><span data-stu-id="6cc34-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cc34-198">要求</span><span class="sxs-lookup"><span data-stu-id="6cc34-198">Request</span></span>
<span data-ttu-id="6cc34-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6cc34-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="6cc34-200">応答</span><span class="sxs-lookup"><span data-stu-id="6cc34-200">Response</span></span>
<span data-ttu-id="6cc34-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6cc34-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





