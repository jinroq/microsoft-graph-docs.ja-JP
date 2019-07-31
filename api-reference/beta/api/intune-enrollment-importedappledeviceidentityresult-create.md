---
title: ImportedAppleDeviceIdentityResult を作成する
description: 新しい importedAppleDeviceIdentityResult オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9e7f05e2933c7b70a783d0fe614707528a1ac808
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35985106"
---
# <a name="create-importedappledeviceidentityresult"></a><span data-ttu-id="a8289-103">ImportedAppleDeviceIdentityResult を作成する</span><span class="sxs-lookup"><span data-stu-id="a8289-103">Create importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="a8289-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8289-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8289-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a8289-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8289-106">新しい[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a8289-106">Create a new [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8289-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a8289-107">Prerequisites</span></span>
<span data-ttu-id="a8289-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a8289-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8289-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a8289-110">Permission type</span></span>|<span data-ttu-id="a8289-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a8289-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8289-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a8289-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a8289-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8289-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a8289-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a8289-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8289-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8289-115">Not supported.</span></span>|
|<span data-ttu-id="a8289-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a8289-116">Application</span></span>|<span data-ttu-id="a8289-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8289-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8289-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a8289-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="a8289-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a8289-119">Request headers</span></span>
|<span data-ttu-id="a8289-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a8289-120">Header</span></span>|<span data-ttu-id="a8289-121">値</span><span class="sxs-lookup"><span data-stu-id="a8289-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8289-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8289-122">Authorization</span></span>|<span data-ttu-id="a8289-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a8289-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8289-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a8289-124">Accept</span></span>|<span data-ttu-id="a8289-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a8289-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8289-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a8289-126">Request body</span></span>
<span data-ttu-id="a8289-127">要求本文で、importedAppleDeviceIdentityResult オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a8289-127">In the request body, supply a JSON representation for the importedAppleDeviceIdentityResult object.</span></span>

<span data-ttu-id="a8289-128">次の表に、importedAppleDeviceIdentityResult の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a8289-128">The following table shows the properties that are required when you create the importedAppleDeviceIdentityResult.</span></span>

|<span data-ttu-id="a8289-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8289-129">Property</span></span>|<span data-ttu-id="a8289-130">型</span><span class="sxs-lookup"><span data-stu-id="a8289-130">Type</span></span>|<span data-ttu-id="a8289-131">説明</span><span class="sxs-lookup"><span data-stu-id="a8289-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8289-132">id</span><span class="sxs-lookup"><span data-stu-id="a8289-132">id</span></span>|<span data-ttu-id="a8289-133">String</span><span class="sxs-lookup"><span data-stu-id="a8289-133">String</span></span>|<span data-ttu-id="a8289-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a8289-134">Key of the entity.</span></span> <span data-ttu-id="a8289-135">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a8289-135">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="a8289-136">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="a8289-136">serialNumber</span></span>|<span data-ttu-id="a8289-137">String</span><span class="sxs-lookup"><span data-stu-id="a8289-137">String</span></span>|<span data-ttu-id="a8289-138">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスのシリアル番号</span><span class="sxs-lookup"><span data-stu-id="a8289-138">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="a8289-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="a8289-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="a8289-140">String</span><span class="sxs-lookup"><span data-stu-id="a8289-140">String</span></span>|<span data-ttu-id="a8289-141">登録プロファイル Id 管理者は、 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承した次の登録時にデバイスに適用する予定です。</span><span class="sxs-lookup"><span data-stu-id="a8289-141">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="a8289-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="a8289-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="a8289-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8289-143">DateTimeOffset</span></span>|<span data-ttu-id="a8289-144">時間登録プロファイルが[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスに割り当てられています。</span><span class="sxs-lookup"><span data-stu-id="a8289-144">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="a8289-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="a8289-145">isSupervised</span></span>|<span data-ttu-id="a8289-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8289-146">Boolean</span></span>|<span data-ttu-id="a8289-147">Apple デバイスが監視されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a8289-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="a8289-148">詳細についてはhttps://support.apple.com/en-us/HT202837 、「 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a8289-148">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="a8289-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="a8289-149">discoverySource</span></span>|[<span data-ttu-id="a8289-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="a8289-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="a8289-151">Apple デバイスの検出ソース。</span><span class="sxs-lookup"><span data-stu-id="a8289-151">Apple device discovery source.</span></span> <span data-ttu-id="a8289-152">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a8289-152">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="a8289-153">可能な値は、`unknown`、`adminImport`、`deviceEnrollmentProgram` です。</span><span class="sxs-lookup"><span data-stu-id="a8289-153">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="a8289-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8289-154">createdDateTime</span></span>|<span data-ttu-id="a8289-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8289-155">DateTimeOffset</span></span>|<span data-ttu-id="a8289-156">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスの日時の作成日時</span><span class="sxs-lookup"><span data-stu-id="a8289-156">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="a8289-157">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8289-157">lastContactedDateTime</span></span>|<span data-ttu-id="a8289-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8289-158">DateTimeOffset</span></span>|<span data-ttu-id="a8289-159">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスの最後の連絡日時。</span><span class="sxs-lookup"><span data-stu-id="a8289-159">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="a8289-160">description</span><span class="sxs-lookup"><span data-stu-id="a8289-160">description</span></span>|<span data-ttu-id="a8289-161">String</span><span class="sxs-lookup"><span data-stu-id="a8289-161">String</span></span>|<span data-ttu-id="a8289-162">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスの説明</span><span class="sxs-lookup"><span data-stu-id="a8289-162">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="a8289-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="a8289-163">enrollmentState</span></span>|[<span data-ttu-id="a8289-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="a8289-164">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="a8289-165">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承された Intune のデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="a8289-165">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="a8289-166">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="a8289-166">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="a8289-167">platform</span><span class="sxs-lookup"><span data-stu-id="a8289-167">platform</span></span>|[<span data-ttu-id="a8289-168">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="a8289-168">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="a8289-169">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="a8289-169">The platform of the Device.</span></span> <span data-ttu-id="a8289-170">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a8289-170">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="a8289-171">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="a8289-171">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="a8289-172">status</span><span class="sxs-lookup"><span data-stu-id="a8289-172">status</span></span>|<span data-ttu-id="a8289-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8289-173">Boolean</span></span>|<span data-ttu-id="a8289-174">インポートされたデバイス id の状態</span><span class="sxs-lookup"><span data-stu-id="a8289-174">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="a8289-175">応答</span><span class="sxs-lookup"><span data-stu-id="a8289-175">Response</span></span>
<span data-ttu-id="a8289-176">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a8289-176">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8289-177">例</span><span class="sxs-lookup"><span data-stu-id="a8289-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8289-178">要求</span><span class="sxs-lookup"><span data-stu-id="a8289-178">Request</span></span>
<span data-ttu-id="a8289-179">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a8289-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a8289-180">応答</span><span class="sxs-lookup"><span data-stu-id="a8289-180">Response</span></span>
<span data-ttu-id="a8289-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a8289-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





