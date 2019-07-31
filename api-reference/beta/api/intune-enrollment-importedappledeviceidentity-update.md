---
title: ImportedAppleDeviceIdentity の更新
description: ImportedAppleDeviceIdentity オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7d04157845e556d927ab6ed4d5cb15c1d34d7659
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35986919"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="ede63-103">ImportedAppleDeviceIdentity の更新</span><span class="sxs-lookup"><span data-stu-id="ede63-103">Update importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="ede63-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ede63-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ede63-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ede63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ede63-106">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ede63-106">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ede63-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ede63-107">Prerequisites</span></span>
<span data-ttu-id="ede63-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ede63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ede63-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ede63-110">Permission type</span></span>|<span data-ttu-id="ede63-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ede63-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ede63-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ede63-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ede63-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ede63-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ede63-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ede63-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ede63-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ede63-115">Not supported.</span></span>|
|<span data-ttu-id="ede63-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ede63-116">Application</span></span>|<span data-ttu-id="ede63-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ede63-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ede63-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ede63-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="ede63-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ede63-119">Request headers</span></span>
|<span data-ttu-id="ede63-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ede63-120">Header</span></span>|<span data-ttu-id="ede63-121">値</span><span class="sxs-lookup"><span data-stu-id="ede63-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ede63-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ede63-122">Authorization</span></span>|<span data-ttu-id="ede63-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ede63-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ede63-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ede63-124">Accept</span></span>|<span data-ttu-id="ede63-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ede63-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ede63-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ede63-126">Request body</span></span>
<span data-ttu-id="ede63-127">要求本文で、 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ede63-127">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="ede63-128">次の表に、 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ede63-128">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="ede63-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ede63-129">Property</span></span>|<span data-ttu-id="ede63-130">型</span><span class="sxs-lookup"><span data-stu-id="ede63-130">Type</span></span>|<span data-ttu-id="ede63-131">説明</span><span class="sxs-lookup"><span data-stu-id="ede63-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ede63-132">id</span><span class="sxs-lookup"><span data-stu-id="ede63-132">id</span></span>|<span data-ttu-id="ede63-133">String</span><span class="sxs-lookup"><span data-stu-id="ede63-133">String</span></span>|<span data-ttu-id="ede63-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ede63-134">Key of the entity.</span></span>|
|<span data-ttu-id="ede63-135">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="ede63-135">serialNumber</span></span>|<span data-ttu-id="ede63-136">String</span><span class="sxs-lookup"><span data-stu-id="ede63-136">String</span></span>|<span data-ttu-id="ede63-137">デバイスのシリアル番号</span><span class="sxs-lookup"><span data-stu-id="ede63-137">Device serial number</span></span>|
|<span data-ttu-id="ede63-138">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="ede63-138">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="ede63-139">String</span><span class="sxs-lookup"><span data-stu-id="ede63-139">String</span></span>|<span data-ttu-id="ede63-140">登録プロファイル Id 管理者が次回の登録時にデバイスに適用する予定</span><span class="sxs-lookup"><span data-stu-id="ede63-140">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="ede63-141">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="ede63-141">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="ede63-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ede63-142">DateTimeOffset</span></span>|<span data-ttu-id="ede63-143">時間登録プロファイルがデバイスに割り当てられている</span><span class="sxs-lookup"><span data-stu-id="ede63-143">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="ede63-144">isSupervised</span><span class="sxs-lookup"><span data-stu-id="ede63-144">isSupervised</span></span>|<span data-ttu-id="ede63-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ede63-145">Boolean</span></span>|<span data-ttu-id="ede63-146">Apple デバイスが監視されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ede63-146">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="ede63-147">詳細情報は次のとおりです。https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="ede63-147">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="ede63-148">discoverySource</span><span class="sxs-lookup"><span data-stu-id="ede63-148">discoverySource</span></span>|[<span data-ttu-id="ede63-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="ede63-149">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="ede63-150">Apple デバイスの検出ソース。</span><span class="sxs-lookup"><span data-stu-id="ede63-150">Apple device discovery source.</span></span> <span data-ttu-id="ede63-151">可能な値は、`unknown`、`adminImport`、`deviceEnrollmentProgram` です。</span><span class="sxs-lookup"><span data-stu-id="ede63-151">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="ede63-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ede63-152">createdDateTime</span></span>|<span data-ttu-id="ede63-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ede63-153">DateTimeOffset</span></span>|<span data-ttu-id="ede63-154">デバイスの日時の作成日時</span><span class="sxs-lookup"><span data-stu-id="ede63-154">Created Date Time of the device</span></span>|
|<span data-ttu-id="ede63-155">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="ede63-155">lastContactedDateTime</span></span>|<span data-ttu-id="ede63-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ede63-156">DateTimeOffset</span></span>|<span data-ttu-id="ede63-157">デバイスの最終連絡日時</span><span class="sxs-lookup"><span data-stu-id="ede63-157">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="ede63-158">description</span><span class="sxs-lookup"><span data-stu-id="ede63-158">description</span></span>|<span data-ttu-id="ede63-159">String</span><span class="sxs-lookup"><span data-stu-id="ede63-159">String</span></span>|<span data-ttu-id="ede63-160">デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="ede63-160">The description of the device</span></span>|
|<span data-ttu-id="ede63-161">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="ede63-161">enrollmentState</span></span>|[<span data-ttu-id="ede63-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="ede63-162">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="ede63-163">Intune でのデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="ede63-163">The state of the device in Intune.</span></span> <span data-ttu-id="ede63-164">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="ede63-164">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="ede63-165">platform</span><span class="sxs-lookup"><span data-stu-id="ede63-165">platform</span></span>|[<span data-ttu-id="ede63-166">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="ede63-166">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="ede63-167">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="ede63-167">The platform of the Device.</span></span> <span data-ttu-id="ede63-168">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="ede63-168">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="ede63-169">応答</span><span class="sxs-lookup"><span data-stu-id="ede63-169">Response</span></span>
<span data-ttu-id="ede63-170">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ede63-170">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ede63-171">例</span><span class="sxs-lookup"><span data-stu-id="ede63-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="ede63-172">要求</span><span class="sxs-lookup"><span data-stu-id="ede63-172">Request</span></span>
<span data-ttu-id="ede63-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ede63-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="ede63-174">応答</span><span class="sxs-lookup"><span data-stu-id="ede63-174">Response</span></span>
<span data-ttu-id="ede63-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ede63-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





