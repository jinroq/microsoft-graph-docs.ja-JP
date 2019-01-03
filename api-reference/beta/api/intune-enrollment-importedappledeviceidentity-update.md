---
title: ImportedAppleDeviceIdentity を更新します。
description: ImportedAppleDeviceIdentity オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: e2248a781ac4f6bb8ce238d12f2679217e7badd6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352088"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="cc0a9-103">ImportedAppleDeviceIdentity を更新します。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-103">Update importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="cc0a9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc0a9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc0a9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc0a9-107">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-107">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cc0a9-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="cc0a9-108">Prerequisites</span></span>
<span data-ttu-id="cc0a9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc0a9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc0a9-111">Permission type</span></span>|<span data-ttu-id="cc0a9-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc0a9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc0a9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc0a9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc0a9-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc0a9-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cc0a9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc0a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc0a9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-116">Not supported.</span></span>|
|<span data-ttu-id="cc0a9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc0a9-117">Application</span></span>|<span data-ttu-id="cc0a9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc0a9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc0a9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="cc0a9-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc0a9-120">Request headers</span></span>
|<span data-ttu-id="cc0a9-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc0a9-121">Header</span></span>|<span data-ttu-id="cc0a9-122">値</span><span class="sxs-lookup"><span data-stu-id="cc0a9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc0a9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc0a9-123">Authorization</span></span>|<span data-ttu-id="cc0a9-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc0a9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cc0a9-125">Accept</span></span>|<span data-ttu-id="cc0a9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cc0a9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc0a9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc0a9-127">Request body</span></span>
<span data-ttu-id="cc0a9-128">要求の本文に[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="cc0a9-129">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="cc0a9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc0a9-130">Property</span></span>|<span data-ttu-id="cc0a9-131">種類</span><span class="sxs-lookup"><span data-stu-id="cc0a9-131">Type</span></span>|<span data-ttu-id="cc0a9-132">説明</span><span class="sxs-lookup"><span data-stu-id="cc0a9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc0a9-133">ID</span><span class="sxs-lookup"><span data-stu-id="cc0a9-133">id</span></span>|<span data-ttu-id="cc0a9-134">String</span><span class="sxs-lookup"><span data-stu-id="cc0a9-134">String</span></span>|<span data-ttu-id="cc0a9-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-135">Key of the entity.</span></span>|
|<span data-ttu-id="cc0a9-136">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="cc0a9-136">serialNumber</span></span>|<span data-ttu-id="cc0a9-137">String</span><span class="sxs-lookup"><span data-stu-id="cc0a9-137">String</span></span>|<span data-ttu-id="cc0a9-138">デバイスのシリアル番号</span><span class="sxs-lookup"><span data-stu-id="cc0a9-138">Device serial number</span></span>|
|<span data-ttu-id="cc0a9-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="cc0a9-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="cc0a9-140">String</span><span class="sxs-lookup"><span data-stu-id="cc0a9-140">String</span></span>|<span data-ttu-id="cc0a9-141">登録プロファイル Id の管理者が、次の登録時にデバイスに適用しようとしています。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="cc0a9-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="cc0a9-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="cc0a9-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc0a9-143">DateTimeOffset</span></span>|<span data-ttu-id="cc0a9-144">時間登録のプロファイルは、デバイスに割り当てられました。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="cc0a9-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="cc0a9-145">isSupervised</span></span>|<span data-ttu-id="cc0a9-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc0a9-146">Boolean</span></span>|<span data-ttu-id="cc0a9-147">Apple デバイスが監視された状態を示します。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="cc0a9-148">詳細についてでです。https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="cc0a9-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="cc0a9-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="cc0a9-149">discoverySource</span></span>|[<span data-ttu-id="cc0a9-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="cc0a9-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="cc0a9-151">Apple のデバイス検出のソースです。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-151">Apple device discovery source.</span></span> <span data-ttu-id="cc0a9-152">可能な値は、`unknown`、`adminImport`、`deviceEnrollmentProgram` です。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="cc0a9-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc0a9-153">createdDateTime</span></span>|<span data-ttu-id="cc0a9-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc0a9-154">DateTimeOffset</span></span>|<span data-ttu-id="cc0a9-155">デバイスの作成日時</span><span class="sxs-lookup"><span data-stu-id="cc0a9-155">Created Date Time of the device</span></span>|
|<span data-ttu-id="cc0a9-156">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc0a9-156">lastContactedDateTime</span></span>|<span data-ttu-id="cc0a9-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc0a9-157">DateTimeOffset</span></span>|<span data-ttu-id="cc0a9-158">最終アクセス日時、デバイスの</span><span class="sxs-lookup"><span data-stu-id="cc0a9-158">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="cc0a9-159">説明</span><span class="sxs-lookup"><span data-stu-id="cc0a9-159">description</span></span>|<span data-ttu-id="cc0a9-160">String</span><span class="sxs-lookup"><span data-stu-id="cc0a9-160">String</span></span>|<span data-ttu-id="cc0a9-161">デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="cc0a9-161">The description of the device</span></span>|
|<span data-ttu-id="cc0a9-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="cc0a9-162">enrollmentState</span></span>|[<span data-ttu-id="cc0a9-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="cc0a9-163">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="cc0a9-164">Intune でデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-164">The state of the device in Intune.</span></span> <span data-ttu-id="cc0a9-165">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-165">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="cc0a9-166">platform</span><span class="sxs-lookup"><span data-stu-id="cc0a9-166">platform</span></span>|[<span data-ttu-id="cc0a9-167">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="cc0a9-167">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="cc0a9-168">デバイスのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-168">The platform of the Device.</span></span> <span data-ttu-id="cc0a9-169">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-169">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="cc0a9-170">応答</span><span class="sxs-lookup"><span data-stu-id="cc0a9-170">Response</span></span>
<span data-ttu-id="cc0a9-171">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-171">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc0a9-172">例</span><span class="sxs-lookup"><span data-stu-id="cc0a9-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="cc0a9-173">要求</span><span class="sxs-lookup"><span data-stu-id="cc0a9-173">Request</span></span>
<span data-ttu-id="cc0a9-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
Content-type: application/json
Content-length: 431

{
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="cc0a9-175">応答</span><span class="sxs-lookup"><span data-stu-id="cc0a9-175">Response</span></span>
<span data-ttu-id="cc0a9-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cc0a9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 605

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "352e3c2f-3c2f-352e-2f3c-2e352f3c2e35",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```




