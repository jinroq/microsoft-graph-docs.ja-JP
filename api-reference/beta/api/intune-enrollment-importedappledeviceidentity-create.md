---
title: ImportedAppleDeviceIdentity を作成する
description: 新しい importedAppleDeviceIdentity オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4e01f31fec4ca071f3c3409bf0865fb91e036d2e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908694"
---
# <a name="create-importedappledeviceidentity"></a><span data-ttu-id="d2d57-103">ImportedAppleDeviceIdentity を作成する</span><span class="sxs-lookup"><span data-stu-id="d2d57-103">Create importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="d2d57-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2d57-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2d57-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d2d57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2d57-106">新しい[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d2d57-106">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2d57-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d2d57-107">Prerequisites</span></span>
<span data-ttu-id="d2d57-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2d57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2d57-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2d57-110">Permission type</span></span>|<span data-ttu-id="d2d57-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2d57-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2d57-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d2d57-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d2d57-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2d57-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d2d57-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2d57-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2d57-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2d57-115">Not supported.</span></span>|
|<span data-ttu-id="d2d57-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2d57-116">Application</span></span>|<span data-ttu-id="d2d57-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2d57-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2d57-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2d57-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="d2d57-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2d57-119">Request headers</span></span>
|<span data-ttu-id="d2d57-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2d57-120">Header</span></span>|<span data-ttu-id="d2d57-121">値</span><span class="sxs-lookup"><span data-stu-id="d2d57-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2d57-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2d57-122">Authorization</span></span>|<span data-ttu-id="d2d57-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d2d57-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2d57-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d2d57-124">Accept</span></span>|<span data-ttu-id="d2d57-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d2d57-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2d57-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2d57-126">Request body</span></span>
<span data-ttu-id="d2d57-127">要求本文で、importedAppleDeviceIdentity オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d2d57-127">In the request body, supply a JSON representation for the importedAppleDeviceIdentity object.</span></span>

<span data-ttu-id="d2d57-128">次の表に、importedAppleDeviceIdentity の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d2d57-128">The following table shows the properties that are required when you create the importedAppleDeviceIdentity.</span></span>

|<span data-ttu-id="d2d57-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2d57-129">Property</span></span>|<span data-ttu-id="d2d57-130">型</span><span class="sxs-lookup"><span data-stu-id="d2d57-130">Type</span></span>|<span data-ttu-id="d2d57-131">説明</span><span class="sxs-lookup"><span data-stu-id="d2d57-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2d57-132">id</span><span class="sxs-lookup"><span data-stu-id="d2d57-132">id</span></span>|<span data-ttu-id="d2d57-133">String</span><span class="sxs-lookup"><span data-stu-id="d2d57-133">String</span></span>|<span data-ttu-id="d2d57-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d2d57-134">Key of the entity.</span></span>|
|<span data-ttu-id="d2d57-135">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="d2d57-135">serialNumber</span></span>|<span data-ttu-id="d2d57-136">String</span><span class="sxs-lookup"><span data-stu-id="d2d57-136">String</span></span>|<span data-ttu-id="d2d57-137">デバイスのシリアル番号</span><span class="sxs-lookup"><span data-stu-id="d2d57-137">Device serial number</span></span>|
|<span data-ttu-id="d2d57-138">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="d2d57-138">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="d2d57-139">String</span><span class="sxs-lookup"><span data-stu-id="d2d57-139">String</span></span>|<span data-ttu-id="d2d57-140">登録プロファイル Id 管理者が次回の登録時にデバイスに適用する予定</span><span class="sxs-lookup"><span data-stu-id="d2d57-140">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="d2d57-141">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="d2d57-141">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="d2d57-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2d57-142">DateTimeOffset</span></span>|<span data-ttu-id="d2d57-143">時間登録プロファイルがデバイスに割り当てられている</span><span class="sxs-lookup"><span data-stu-id="d2d57-143">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="d2d57-144">isSupervised</span><span class="sxs-lookup"><span data-stu-id="d2d57-144">isSupervised</span></span>|<span data-ttu-id="d2d57-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2d57-145">Boolean</span></span>|<span data-ttu-id="d2d57-146">Apple デバイスが監視されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d2d57-146">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="d2d57-147">詳細情報は次のとおりです。https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="d2d57-147">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="d2d57-148">discoverySource</span><span class="sxs-lookup"><span data-stu-id="d2d57-148">discoverySource</span></span>|[<span data-ttu-id="d2d57-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="d2d57-149">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="d2d57-150">Apple デバイスの検出ソース。</span><span class="sxs-lookup"><span data-stu-id="d2d57-150">Apple device discovery source.</span></span> <span data-ttu-id="d2d57-151">可能な値は、`unknown`、`adminImport`、`deviceEnrollmentProgram` です。</span><span class="sxs-lookup"><span data-stu-id="d2d57-151">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="d2d57-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d2d57-152">createdDateTime</span></span>|<span data-ttu-id="d2d57-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2d57-153">DateTimeOffset</span></span>|<span data-ttu-id="d2d57-154">デバイスの日時の作成日時</span><span class="sxs-lookup"><span data-stu-id="d2d57-154">Created Date Time of the device</span></span>|
|<span data-ttu-id="d2d57-155">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2d57-155">lastContactedDateTime</span></span>|<span data-ttu-id="d2d57-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2d57-156">DateTimeOffset</span></span>|<span data-ttu-id="d2d57-157">デバイスの最終連絡日時</span><span class="sxs-lookup"><span data-stu-id="d2d57-157">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="d2d57-158">description</span><span class="sxs-lookup"><span data-stu-id="d2d57-158">description</span></span>|<span data-ttu-id="d2d57-159">String</span><span class="sxs-lookup"><span data-stu-id="d2d57-159">String</span></span>|<span data-ttu-id="d2d57-160">デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="d2d57-160">The description of the device</span></span>|
|<span data-ttu-id="d2d57-161">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="d2d57-161">enrollmentState</span></span>|[<span data-ttu-id="d2d57-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="d2d57-162">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="d2d57-163">Intune でのデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="d2d57-163">The state of the device in Intune.</span></span> <span data-ttu-id="d2d57-164">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="d2d57-164">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="d2d57-165">platform</span><span class="sxs-lookup"><span data-stu-id="d2d57-165">platform</span></span>|[<span data-ttu-id="d2d57-166">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="d2d57-166">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="d2d57-167">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="d2d57-167">The platform of the Device.</span></span> <span data-ttu-id="d2d57-168">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="d2d57-168">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="d2d57-169">応答</span><span class="sxs-lookup"><span data-stu-id="d2d57-169">Response</span></span>
<span data-ttu-id="d2d57-170">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d2d57-170">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2d57-171">例</span><span class="sxs-lookup"><span data-stu-id="d2d57-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2d57-172">要求</span><span class="sxs-lookup"><span data-stu-id="d2d57-172">Request</span></span>
<span data-ttu-id="d2d57-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d2d57-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d2d57-174">応答</span><span class="sxs-lookup"><span data-stu-id="d2d57-174">Response</span></span>
<span data-ttu-id="d2d57-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d2d57-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




