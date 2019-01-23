---
title: windowsPhone81CompliancePolicy の作成
description: 新しい windowsPhone81CompliancePolicy オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a2d45f30b50906dc1e1a5dd2ac954fe151a6b59a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393082"
---
# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="13bdc-103">windowsPhone81CompliancePolicy の作成</span><span class="sxs-lookup"><span data-stu-id="13bdc-103">Create windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="13bdc-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="13bdc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="13bdc-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13bdc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13bdc-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="13bdc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13bdc-107">新しい [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="13bdc-107">Create a new [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13bdc-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="13bdc-108">Prerequisites</span></span>
<span data-ttu-id="13bdc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13bdc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="13bdc-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="13bdc-111">Permission type</span></span>|<span data-ttu-id="13bdc-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="13bdc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13bdc-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="13bdc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13bdc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13bdc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="13bdc-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="13bdc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13bdc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13bdc-116">Not supported.</span></span>|
|<span data-ttu-id="13bdc-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="13bdc-117">Application</span></span>|<span data-ttu-id="13bdc-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13bdc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13bdc-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="13bdc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="13bdc-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13bdc-120">Request headers</span></span>
|<span data-ttu-id="13bdc-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13bdc-121">Header</span></span>|<span data-ttu-id="13bdc-122">値</span><span class="sxs-lookup"><span data-stu-id="13bdc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13bdc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="13bdc-123">Authorization</span></span>|<span data-ttu-id="13bdc-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="13bdc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13bdc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="13bdc-125">Accept</span></span>|<span data-ttu-id="13bdc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13bdc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13bdc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="13bdc-127">Request body</span></span>
<span data-ttu-id="13bdc-128">要求本文で、windowsPhone81CompliancePolicy オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="13bdc-128">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="13bdc-129">次の表に、windowsPhone81CompliancePolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="13bdc-129">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="13bdc-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13bdc-130">Property</span></span>|<span data-ttu-id="13bdc-131">型</span><span class="sxs-lookup"><span data-stu-id="13bdc-131">Type</span></span>|<span data-ttu-id="13bdc-132">説明</span><span class="sxs-lookup"><span data-stu-id="13bdc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13bdc-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="13bdc-133">roleScopeTagIds</span></span>|<span data-ttu-id="13bdc-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="13bdc-134">String collection</span></span>|<span data-ttu-id="13bdc-135">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="13bdc-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="13bdc-136">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="13bdc-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="13bdc-137">id</span><span class="sxs-lookup"><span data-stu-id="13bdc-137">id</span></span>|<span data-ttu-id="13bdc-138">String</span><span class="sxs-lookup"><span data-stu-id="13bdc-138">String</span></span>|<span data-ttu-id="13bdc-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="13bdc-139">Key of the entity.</span></span> <span data-ttu-id="13bdc-140">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="13bdc-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="13bdc-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13bdc-141">createdDateTime</span></span>|<span data-ttu-id="13bdc-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13bdc-142">DateTimeOffset</span></span>|<span data-ttu-id="13bdc-143">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="13bdc-143">DateTime the object was created.</span></span> <span data-ttu-id="13bdc-144">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="13bdc-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="13bdc-145">説明</span><span class="sxs-lookup"><span data-stu-id="13bdc-145">description</span></span>|<span data-ttu-id="13bdc-146">String</span><span class="sxs-lookup"><span data-stu-id="13bdc-146">String</span></span>|<span data-ttu-id="13bdc-147">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="13bdc-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="13bdc-148">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="13bdc-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="13bdc-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13bdc-149">lastModifiedDateTime</span></span>|<span data-ttu-id="13bdc-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13bdc-150">DateTimeOffset</span></span>|<span data-ttu-id="13bdc-151">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="13bdc-151">DateTime the object was last modified.</span></span> <span data-ttu-id="13bdc-152">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="13bdc-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="13bdc-153">displayName</span><span class="sxs-lookup"><span data-stu-id="13bdc-153">displayName</span></span>|<span data-ttu-id="13bdc-154">String</span><span class="sxs-lookup"><span data-stu-id="13bdc-154">String</span></span>|<span data-ttu-id="13bdc-155">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="13bdc-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="13bdc-156">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="13bdc-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="13bdc-157">version</span><span class="sxs-lookup"><span data-stu-id="13bdc-157">version</span></span>|<span data-ttu-id="13bdc-158">Int32</span><span class="sxs-lookup"><span data-stu-id="13bdc-158">Int32</span></span>|<span data-ttu-id="13bdc-159">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="13bdc-159">Version of the device configuration.</span></span> <span data-ttu-id="13bdc-160">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="13bdc-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="13bdc-161">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="13bdc-161">passwordBlockSimple</span></span>|<span data-ttu-id="13bdc-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="13bdc-162">Boolean</span></span>|<span data-ttu-id="13bdc-163">カレンダーの同期を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="13bdc-163">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="13bdc-164">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="13bdc-164">passwordExpirationDays</span></span>|<span data-ttu-id="13bdc-165">Int32</span><span class="sxs-lookup"><span data-stu-id="13bdc-165">Int32</span></span>|<span data-ttu-id="13bdc-166">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="13bdc-166">Number of days before the password expires.</span></span>|
|<span data-ttu-id="13bdc-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="13bdc-167">passwordMinimumLength</span></span>|<span data-ttu-id="13bdc-168">Int32</span><span class="sxs-lookup"><span data-stu-id="13bdc-168">Int32</span></span>|<span data-ttu-id="13bdc-169">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="13bdc-169">Minimum length of passwords.</span></span>|
|<span data-ttu-id="13bdc-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="13bdc-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="13bdc-171">Int32</span><span class="sxs-lookup"><span data-stu-id="13bdc-171">Int32</span></span>|<span data-ttu-id="13bdc-172">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="13bdc-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="13bdc-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="13bdc-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="13bdc-174">Int32</span><span class="sxs-lookup"><span data-stu-id="13bdc-174">Int32</span></span>|<span data-ttu-id="13bdc-175">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="13bdc-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="13bdc-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="13bdc-176">passwordRequiredType</span></span>|[<span data-ttu-id="13bdc-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="13bdc-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="13bdc-178">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="13bdc-178">The required password type.</span></span> <span data-ttu-id="13bdc-179">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="13bdc-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="13bdc-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="13bdc-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="13bdc-181">Int32</span><span class="sxs-lookup"><span data-stu-id="13bdc-181">Int32</span></span>|<span data-ttu-id="13bdc-182">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="13bdc-182">Number of previous passwords to block.</span></span> <span data-ttu-id="13bdc-183">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="13bdc-183">Valid values 0 to 24</span></span>|
|<span data-ttu-id="13bdc-184">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="13bdc-184">passwordRequired</span></span>|<span data-ttu-id="13bdc-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="13bdc-185">Boolean</span></span>|<span data-ttu-id="13bdc-186">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="13bdc-186">Whether or not to require a password.</span></span>|
|<span data-ttu-id="13bdc-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="13bdc-187">osMinimumVersion</span></span>|<span data-ttu-id="13bdc-188">String</span><span class="sxs-lookup"><span data-stu-id="13bdc-188">String</span></span>|<span data-ttu-id="13bdc-189">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="13bdc-189">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="13bdc-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="13bdc-190">osMaximumVersion</span></span>|<span data-ttu-id="13bdc-191">String</span><span class="sxs-lookup"><span data-stu-id="13bdc-191">String</span></span>|<span data-ttu-id="13bdc-192">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="13bdc-192">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="13bdc-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="13bdc-193">storageRequireEncryption</span></span>|<span data-ttu-id="13bdc-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="13bdc-194">Boolean</span></span>|<span data-ttu-id="13bdc-195">Windows Phone デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="13bdc-195">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="13bdc-196">応答</span><span class="sxs-lookup"><span data-stu-id="13bdc-196">Response</span></span>
<span data-ttu-id="13bdc-197">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="13bdc-197">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13bdc-198">例</span><span class="sxs-lookup"><span data-stu-id="13bdc-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="13bdc-199">要求</span><span class="sxs-lookup"><span data-stu-id="13bdc-199">Request</span></span>
<span data-ttu-id="13bdc-200">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="13bdc-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="13bdc-201">応答</span><span class="sxs-lookup"><span data-stu-id="13bdc-201">Response</span></span>
<span data-ttu-id="13bdc-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="13bdc-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




