---
title: ImportedAppleDeviceIdentityResult を作成します。
description: 新しい importedAppleDeviceIdentityResult オブジェクトを作成します。
ms.openlocfilehash: 1f3b7091ba904843ed95a802ece9a5fa42e05b4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071900"
---
# <a name="create-importedappledeviceidentityresult"></a><span data-ttu-id="e47c8-103">ImportedAppleDeviceIdentityResult を作成します。</span><span class="sxs-lookup"><span data-stu-id="e47c8-103">Create importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="e47c8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e47c8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e47c8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e47c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e47c8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e47c8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e47c8-107">新しい[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e47c8-107">Create a new [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e47c8-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e47c8-108">Prerequisites</span></span>
<span data-ttu-id="e47c8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e47c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e47c8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e47c8-111">Permission type</span></span>|<span data-ttu-id="e47c8-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e47c8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e47c8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e47c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e47c8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e47c8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e47c8-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e47c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e47c8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e47c8-116">Not supported.</span></span>|
|<span data-ttu-id="e47c8-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e47c8-117">Application</span></span>|<span data-ttu-id="e47c8-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e47c8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e47c8-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e47c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="e47c8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e47c8-120">Request headers</span></span>
|<span data-ttu-id="e47c8-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e47c8-121">Header</span></span>|<span data-ttu-id="e47c8-122">値</span><span class="sxs-lookup"><span data-stu-id="e47c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e47c8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e47c8-123">Authorization</span></span>|<span data-ttu-id="e47c8-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e47c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e47c8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e47c8-125">Accept</span></span>|<span data-ttu-id="e47c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e47c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e47c8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e47c8-127">Request body</span></span>
<span data-ttu-id="e47c8-128">要求の本文に importedAppleDeviceIdentityResult オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="e47c8-128">In the request body, supply a JSON representation for the importedAppleDeviceIdentityResult object.</span></span>

<span data-ttu-id="e47c8-129">次の表は、importedAppleDeviceIdentityResult を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e47c8-129">The following table shows the properties that are required when you create the importedAppleDeviceIdentityResult.</span></span>

|<span data-ttu-id="e47c8-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e47c8-130">Property</span></span>|<span data-ttu-id="e47c8-131">型</span><span class="sxs-lookup"><span data-stu-id="e47c8-131">Type</span></span>|<span data-ttu-id="e47c8-132">説明</span><span class="sxs-lookup"><span data-stu-id="e47c8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e47c8-133">id</span><span class="sxs-lookup"><span data-stu-id="e47c8-133">id</span></span>|<span data-ttu-id="e47c8-134">String</span><span class="sxs-lookup"><span data-stu-id="e47c8-134">String</span></span>|<span data-ttu-id="e47c8-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e47c8-135">Key of the entity.</span></span> <span data-ttu-id="e47c8-136">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="e47c8-136">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="e47c8-137">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="e47c8-137">serialNumber</span></span>|<span data-ttu-id="e47c8-138">String</span><span class="sxs-lookup"><span data-stu-id="e47c8-138">String</span></span>|<span data-ttu-id="e47c8-139">継承されるデバイス ・ シリアル番号は、 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から</span><span class="sxs-lookup"><span data-stu-id="e47c8-139">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="e47c8-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="e47c8-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="e47c8-141">String</span><span class="sxs-lookup"><span data-stu-id="e47c8-141">String</span></span>|<span data-ttu-id="e47c8-142">登録プロファイル Id の管理者が、 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承される、次の登録時に、デバイスに適用しようとしています。</span><span class="sxs-lookup"><span data-stu-id="e47c8-142">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="e47c8-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="e47c8-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="e47c8-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e47c8-144">DateTimeOffset</span></span>|<span data-ttu-id="e47c8-145">時間登録のプロファイルは、 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されるデバイスに割り当てられました。</span><span class="sxs-lookup"><span data-stu-id="e47c8-145">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="e47c8-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="e47c8-146">isSupervised</span></span>|<span data-ttu-id="e47c8-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="e47c8-147">Boolean</span></span>|<span data-ttu-id="e47c8-148">Apple デバイスが監視された状態を示します。</span><span class="sxs-lookup"><span data-stu-id="e47c8-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="e47c8-149">詳細については、: https://support.apple.com/en-us/HT202837 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="e47c8-149">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="e47c8-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="e47c8-150">discoverySource</span></span>|[<span data-ttu-id="e47c8-151">discoverySource</span><span class="sxs-lookup"><span data-stu-id="e47c8-151">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="e47c8-152">Apple のデバイス検出のソースです。</span><span class="sxs-lookup"><span data-stu-id="e47c8-152">Apple device discovery source.</span></span> <span data-ttu-id="e47c8-153">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e47c8-153">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="e47c8-154">可能な値は、`unknown`、`adminImport`、`deviceEnrollmentProgram` です。</span><span class="sxs-lookup"><span data-stu-id="e47c8-154">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="e47c8-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e47c8-155">createdDateTime</span></span>|<span data-ttu-id="e47c8-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e47c8-156">DateTimeOffset</span></span>|<span data-ttu-id="e47c8-157">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承される、デバイスの日時を作成</span><span class="sxs-lookup"><span data-stu-id="e47c8-157">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="e47c8-158">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="e47c8-158">lastContactedDateTime</span></span>|<span data-ttu-id="e47c8-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e47c8-159">DateTimeOffset</span></span>|<span data-ttu-id="e47c8-160">最終接続日時[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されるデバイスの</span><span class="sxs-lookup"><span data-stu-id="e47c8-160">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="e47c8-161">説明</span><span class="sxs-lookup"><span data-stu-id="e47c8-161">description</span></span>|<span data-ttu-id="e47c8-162">String</span><span class="sxs-lookup"><span data-stu-id="e47c8-162">String</span></span>|<span data-ttu-id="e47c8-163">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承される、デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="e47c8-163">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="e47c8-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="e47c8-164">enrollmentState</span></span>|[<span data-ttu-id="e47c8-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="e47c8-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="e47c8-166">Intune 継承で[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)からのデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="e47c8-166">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="e47c8-167">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="e47c8-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="e47c8-168">platform</span><span class="sxs-lookup"><span data-stu-id="e47c8-168">platform</span></span>|[<span data-ttu-id="e47c8-169">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="e47c8-169">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="e47c8-170">デバイスのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="e47c8-170">The platform of the Device.</span></span> <span data-ttu-id="e47c8-171">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e47c8-171">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="e47c8-172">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="e47c8-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="e47c8-173">status</span><span class="sxs-lookup"><span data-stu-id="e47c8-173">status</span></span>|<span data-ttu-id="e47c8-174">ブール値</span><span class="sxs-lookup"><span data-stu-id="e47c8-174">Boolean</span></span>|<span data-ttu-id="e47c8-175">インポートされたデバイス id のステータス</span><span class="sxs-lookup"><span data-stu-id="e47c8-175">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="e47c8-176">応答</span><span class="sxs-lookup"><span data-stu-id="e47c8-176">Response</span></span>
<span data-ttu-id="e47c8-177">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e47c8-177">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e47c8-178">例</span><span class="sxs-lookup"><span data-stu-id="e47c8-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="e47c8-179">要求</span><span class="sxs-lookup"><span data-stu-id="e47c8-179">Request</span></span>
<span data-ttu-id="e47c8-180">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e47c8-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
Content-type: application/json
Content-length: 522

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a><span data-ttu-id="e47c8-181">応答</span><span class="sxs-lookup"><span data-stu-id="e47c8-181">Response</span></span>
<span data-ttu-id="e47c8-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e47c8-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 630

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```





