---
title: windows81CompliancePolicy の更新
description: windows81CompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c9fcc9d06ec02db77de0a3608f80a44632e667c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975337"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="623ba-103">windows81CompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="623ba-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="623ba-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="623ba-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="623ba-105">[windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="623ba-105">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="623ba-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="623ba-106">Prerequisites</span></span>
<span data-ttu-id="623ba-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="623ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="623ba-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="623ba-109">Permission type</span></span>|<span data-ttu-id="623ba-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="623ba-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="623ba-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="623ba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="623ba-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="623ba-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="623ba-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="623ba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="623ba-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="623ba-114">Not supported.</span></span>|
|<span data-ttu-id="623ba-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="623ba-115">Application</span></span>|<span data-ttu-id="623ba-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="623ba-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="623ba-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="623ba-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="623ba-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="623ba-118">Request headers</span></span>
|<span data-ttu-id="623ba-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="623ba-119">Header</span></span>|<span data-ttu-id="623ba-120">値</span><span class="sxs-lookup"><span data-stu-id="623ba-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="623ba-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="623ba-121">Authorization</span></span>|<span data-ttu-id="623ba-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="623ba-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="623ba-123">承諾</span><span class="sxs-lookup"><span data-stu-id="623ba-123">Accept</span></span>|<span data-ttu-id="623ba-124">application/json</span><span class="sxs-lookup"><span data-stu-id="623ba-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="623ba-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="623ba-125">Request body</span></span>
<span data-ttu-id="623ba-126">要求本文で、[windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="623ba-126">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="623ba-127">次の表に、[windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="623ba-127">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="623ba-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="623ba-128">Property</span></span>|<span data-ttu-id="623ba-129">型</span><span class="sxs-lookup"><span data-stu-id="623ba-129">Type</span></span>|<span data-ttu-id="623ba-130">説明</span><span class="sxs-lookup"><span data-stu-id="623ba-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="623ba-131">id</span><span class="sxs-lookup"><span data-stu-id="623ba-131">id</span></span>|<span data-ttu-id="623ba-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="623ba-132">String</span></span>|<span data-ttu-id="623ba-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="623ba-133">Key of the entity.</span></span> <span data-ttu-id="623ba-134">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="623ba-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="623ba-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="623ba-135">createdDateTime</span></span>|<span data-ttu-id="623ba-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="623ba-136">DateTimeOffset</span></span>|<span data-ttu-id="623ba-137">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="623ba-137">DateTime the object was created.</span></span> <span data-ttu-id="623ba-138">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="623ba-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="623ba-139">description</span><span class="sxs-lookup"><span data-stu-id="623ba-139">description</span></span>|<span data-ttu-id="623ba-140">String</span><span class="sxs-lookup"><span data-stu-id="623ba-140">String</span></span>|<span data-ttu-id="623ba-141">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="623ba-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="623ba-142">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="623ba-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="623ba-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="623ba-143">lastModifiedDateTime</span></span>|<span data-ttu-id="623ba-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="623ba-144">DateTimeOffset</span></span>|<span data-ttu-id="623ba-145">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="623ba-145">DateTime the object was last modified.</span></span> <span data-ttu-id="623ba-146">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="623ba-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="623ba-147">displayName</span><span class="sxs-lookup"><span data-stu-id="623ba-147">displayName</span></span>|<span data-ttu-id="623ba-148">String</span><span class="sxs-lookup"><span data-stu-id="623ba-148">String</span></span>|<span data-ttu-id="623ba-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="623ba-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="623ba-150">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="623ba-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="623ba-151">version</span><span class="sxs-lookup"><span data-stu-id="623ba-151">version</span></span>|<span data-ttu-id="623ba-152">Int32</span><span class="sxs-lookup"><span data-stu-id="623ba-152">Int32</span></span>|<span data-ttu-id="623ba-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="623ba-153">Version of the device configuration.</span></span> <span data-ttu-id="623ba-154">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="623ba-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="623ba-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="623ba-155">passwordRequired</span></span>|<span data-ttu-id="623ba-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="623ba-156">Boolean</span></span>|<span data-ttu-id="623ba-157">Windows デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="623ba-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="623ba-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="623ba-158">passwordBlockSimple</span></span>|<span data-ttu-id="623ba-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="623ba-159">Boolean</span></span>|<span data-ttu-id="623ba-160">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="623ba-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="623ba-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="623ba-161">passwordExpirationDays</span></span>|<span data-ttu-id="623ba-162">Int32</span><span class="sxs-lookup"><span data-stu-id="623ba-162">Int32</span></span>|<span data-ttu-id="623ba-163">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="623ba-163">Password expiration in days.</span></span>|
|<span data-ttu-id="623ba-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="623ba-164">passwordMinimumLength</span></span>|<span data-ttu-id="623ba-165">Int32</span><span class="sxs-lookup"><span data-stu-id="623ba-165">Int32</span></span>|<span data-ttu-id="623ba-166">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="623ba-166">The minimum password length.</span></span>|
|<span data-ttu-id="623ba-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="623ba-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="623ba-168">Int32</span><span class="sxs-lookup"><span data-stu-id="623ba-168">Int32</span></span>|<span data-ttu-id="623ba-169">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="623ba-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="623ba-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="623ba-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="623ba-171">Int32</span><span class="sxs-lookup"><span data-stu-id="623ba-171">Int32</span></span>|<span data-ttu-id="623ba-172">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="623ba-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="623ba-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="623ba-173">passwordRequiredType</span></span>|[<span data-ttu-id="623ba-174">requiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="623ba-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="623ba-175">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="623ba-175">The required password type.</span></span> <span data-ttu-id="623ba-176">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="623ba-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="623ba-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="623ba-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="623ba-178">Int32</span><span class="sxs-lookup"><span data-stu-id="623ba-178">Int32</span></span>|<span data-ttu-id="623ba-179">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="623ba-179">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="623ba-180">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="623ba-180">Valid values 0 to 24</span></span>|
|<span data-ttu-id="623ba-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="623ba-181">osMinimumVersion</span></span>|<span data-ttu-id="623ba-182">String</span><span class="sxs-lookup"><span data-stu-id="623ba-182">String</span></span>|<span data-ttu-id="623ba-183">Windows 8.1 の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="623ba-183">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="623ba-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="623ba-184">osMaximumVersion</span></span>|<span data-ttu-id="623ba-185">String</span><span class="sxs-lookup"><span data-stu-id="623ba-185">String</span></span>|<span data-ttu-id="623ba-186">Windows 8.1 の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="623ba-186">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="623ba-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="623ba-187">storageRequireEncryption</span></span>|<span data-ttu-id="623ba-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="623ba-188">Boolean</span></span>|<span data-ttu-id="623ba-189">Windows 8.1 のデバイスでの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="623ba-189">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="623ba-190">応答</span><span class="sxs-lookup"><span data-stu-id="623ba-190">Response</span></span>
<span data-ttu-id="623ba-191">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="623ba-191">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="623ba-192">例</span><span class="sxs-lookup"><span data-stu-id="623ba-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="623ba-193">要求</span><span class="sxs-lookup"><span data-stu-id="623ba-193">Request</span></span>
<span data-ttu-id="623ba-194">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="623ba-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="623ba-195">応答</span><span class="sxs-lookup"><span data-stu-id="623ba-195">Response</span></span>
<span data-ttu-id="623ba-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="623ba-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 774

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
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



