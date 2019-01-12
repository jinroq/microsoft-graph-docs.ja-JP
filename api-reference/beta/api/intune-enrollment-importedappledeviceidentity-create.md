---
title: ImportedAppleDeviceIdentity を作成します。
description: 新しい importedAppleDeviceIdentity オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cf6f897d44774ceba92b2d2c965f7cc561001383
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925081"
---
# <a name="create-importedappledeviceidentity"></a><span data-ttu-id="1fa7a-103">ImportedAppleDeviceIdentity を作成します。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-103">Create importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="1fa7a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1fa7a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1fa7a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1fa7a-107">新しい[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-107">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1fa7a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1fa7a-108">Prerequisites</span></span>
<span data-ttu-id="1fa7a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fa7a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1fa7a-111">Permission type</span></span>|<span data-ttu-id="1fa7a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1fa7a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fa7a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1fa7a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1fa7a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fa7a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1fa7a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1fa7a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fa7a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-116">Not supported.</span></span>|
|<span data-ttu-id="1fa7a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1fa7a-117">Application</span></span>|<span data-ttu-id="1fa7a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fa7a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1fa7a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="1fa7a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1fa7a-120">Request headers</span></span>
|<span data-ttu-id="1fa7a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1fa7a-121">Header</span></span>|<span data-ttu-id="1fa7a-122">値</span><span class="sxs-lookup"><span data-stu-id="1fa7a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fa7a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fa7a-123">Authorization</span></span>|<span data-ttu-id="1fa7a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fa7a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1fa7a-125">Accept</span></span>|<span data-ttu-id="1fa7a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1fa7a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fa7a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1fa7a-127">Request body</span></span>
<span data-ttu-id="1fa7a-128">要求の本文に importedAppleDeviceIdentity オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-128">In the request body, supply a JSON representation for the importedAppleDeviceIdentity object.</span></span>

<span data-ttu-id="1fa7a-129">次の表は、importedAppleDeviceIdentity を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-129">The following table shows the properties that are required when you create the importedAppleDeviceIdentity.</span></span>

|<span data-ttu-id="1fa7a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1fa7a-130">Property</span></span>|<span data-ttu-id="1fa7a-131">種類</span><span class="sxs-lookup"><span data-stu-id="1fa7a-131">Type</span></span>|<span data-ttu-id="1fa7a-132">説明</span><span class="sxs-lookup"><span data-stu-id="1fa7a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fa7a-133">ID</span><span class="sxs-lookup"><span data-stu-id="1fa7a-133">id</span></span>|<span data-ttu-id="1fa7a-134">String</span><span class="sxs-lookup"><span data-stu-id="1fa7a-134">String</span></span>|<span data-ttu-id="1fa7a-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-135">Key of the entity.</span></span>|
|<span data-ttu-id="1fa7a-136">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="1fa7a-136">serialNumber</span></span>|<span data-ttu-id="1fa7a-137">String</span><span class="sxs-lookup"><span data-stu-id="1fa7a-137">String</span></span>|<span data-ttu-id="1fa7a-138">デバイスのシリアル番号</span><span class="sxs-lookup"><span data-stu-id="1fa7a-138">Device serial number</span></span>|
|<span data-ttu-id="1fa7a-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="1fa7a-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="1fa7a-140">String</span><span class="sxs-lookup"><span data-stu-id="1fa7a-140">String</span></span>|<span data-ttu-id="1fa7a-141">登録プロファイル Id の管理者が、次の登録時にデバイスに適用しようとしています。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="1fa7a-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="1fa7a-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="1fa7a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fa7a-143">DateTimeOffset</span></span>|<span data-ttu-id="1fa7a-144">時間登録のプロファイルは、デバイスに割り当てられました。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="1fa7a-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="1fa7a-145">isSupervised</span></span>|<span data-ttu-id="1fa7a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa7a-146">Boolean</span></span>|<span data-ttu-id="1fa7a-147">Apple デバイスが監視された状態を示します。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="1fa7a-148">詳細についてでです。https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="1fa7a-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="1fa7a-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="1fa7a-149">discoverySource</span></span>|[<span data-ttu-id="1fa7a-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="1fa7a-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="1fa7a-151">Apple のデバイス検出のソースです。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-151">Apple device discovery source.</span></span> <span data-ttu-id="1fa7a-152">可能な値は、`unknown`、`adminImport`、`deviceEnrollmentProgram` です。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="1fa7a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1fa7a-153">createdDateTime</span></span>|<span data-ttu-id="1fa7a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fa7a-154">DateTimeOffset</span></span>|<span data-ttu-id="1fa7a-155">デバイスの作成日時</span><span class="sxs-lookup"><span data-stu-id="1fa7a-155">Created Date Time of the device</span></span>|
|<span data-ttu-id="1fa7a-156">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="1fa7a-156">lastContactedDateTime</span></span>|<span data-ttu-id="1fa7a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fa7a-157">DateTimeOffset</span></span>|<span data-ttu-id="1fa7a-158">最終アクセス日時、デバイスの</span><span class="sxs-lookup"><span data-stu-id="1fa7a-158">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="1fa7a-159">説明</span><span class="sxs-lookup"><span data-stu-id="1fa7a-159">description</span></span>|<span data-ttu-id="1fa7a-160">String</span><span class="sxs-lookup"><span data-stu-id="1fa7a-160">String</span></span>|<span data-ttu-id="1fa7a-161">デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="1fa7a-161">The description of the device</span></span>|
|<span data-ttu-id="1fa7a-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="1fa7a-162">enrollmentState</span></span>|[<span data-ttu-id="1fa7a-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="1fa7a-163">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="1fa7a-164">Intune でデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-164">The state of the device in Intune.</span></span> <span data-ttu-id="1fa7a-165">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-165">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="1fa7a-166">platform</span><span class="sxs-lookup"><span data-stu-id="1fa7a-166">platform</span></span>|[<span data-ttu-id="1fa7a-167">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="1fa7a-167">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="1fa7a-168">デバイスのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-168">The platform of the Device.</span></span> <span data-ttu-id="1fa7a-169">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-169">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="1fa7a-170">応答</span><span class="sxs-lookup"><span data-stu-id="1fa7a-170">Response</span></span>
<span data-ttu-id="1fa7a-171">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-171">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fa7a-172">例</span><span class="sxs-lookup"><span data-stu-id="1fa7a-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="1fa7a-173">要求</span><span class="sxs-lookup"><span data-stu-id="1fa7a-173">Request</span></span>
<span data-ttu-id="1fa7a-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
Content-type: application/json
Content-length: 497

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
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

### <a name="response"></a><span data-ttu-id="1fa7a-175">応答</span><span class="sxs-lookup"><span data-stu-id="1fa7a-175">Response</span></span>
<span data-ttu-id="1fa7a-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1fa7a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





