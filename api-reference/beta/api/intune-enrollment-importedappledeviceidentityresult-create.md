---
title: ImportedAppleDeviceIdentityResult を作成する
description: 新しい importedAppleDeviceIdentityResult オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 02a673d4128c917c8368ec895cc493998e7066f2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356509"
---
# <a name="create-importedappledeviceidentityresult"></a><span data-ttu-id="6a419-103">ImportedAppleDeviceIdentityResult を作成する</span><span class="sxs-lookup"><span data-stu-id="6a419-103">Create importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="6a419-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a419-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a419-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a419-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a419-106">新しい[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6a419-106">Create a new [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a419-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6a419-107">Prerequisites</span></span>
<span data-ttu-id="6a419-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a419-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a419-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a419-110">Permission type</span></span>|<span data-ttu-id="6a419-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a419-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a419-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a419-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a419-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a419-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6a419-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a419-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a419-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a419-115">Not supported.</span></span>|
|<span data-ttu-id="6a419-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a419-116">Application</span></span>|<span data-ttu-id="6a419-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a419-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a419-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a419-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="6a419-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a419-119">Request headers</span></span>
|<span data-ttu-id="6a419-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a419-120">Header</span></span>|<span data-ttu-id="6a419-121">値</span><span class="sxs-lookup"><span data-stu-id="6a419-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a419-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a419-122">Authorization</span></span>|<span data-ttu-id="6a419-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a419-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a419-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6a419-124">Accept</span></span>|<span data-ttu-id="6a419-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a419-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a419-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a419-126">Request body</span></span>
<span data-ttu-id="6a419-127">要求本文で、importedAppleDeviceIdentityResult オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6a419-127">In the request body, supply a JSON representation for the importedAppleDeviceIdentityResult object.</span></span>

<span data-ttu-id="6a419-128">次の表に、importedAppleDeviceIdentityResult の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6a419-128">The following table shows the properties that are required when you create the importedAppleDeviceIdentityResult.</span></span>

|<span data-ttu-id="6a419-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a419-129">Property</span></span>|<span data-ttu-id="6a419-130">型</span><span class="sxs-lookup"><span data-stu-id="6a419-130">Type</span></span>|<span data-ttu-id="6a419-131">説明</span><span class="sxs-lookup"><span data-stu-id="6a419-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a419-132">id</span><span class="sxs-lookup"><span data-stu-id="6a419-132">id</span></span>|<span data-ttu-id="6a419-133">String</span><span class="sxs-lookup"><span data-stu-id="6a419-133">String</span></span>|<span data-ttu-id="6a419-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6a419-134">Key of the entity.</span></span> <span data-ttu-id="6a419-135">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6a419-135">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="6a419-136">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="6a419-136">serialNumber</span></span>|<span data-ttu-id="6a419-137">String</span><span class="sxs-lookup"><span data-stu-id="6a419-137">String</span></span>|<span data-ttu-id="6a419-138">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスのシリアル番号</span><span class="sxs-lookup"><span data-stu-id="6a419-138">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="6a419-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="6a419-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="6a419-140">String</span><span class="sxs-lookup"><span data-stu-id="6a419-140">String</span></span>|<span data-ttu-id="6a419-141">登録プロファイル Id 管理者は、 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承した次の登録時にデバイスに適用する予定です。</span><span class="sxs-lookup"><span data-stu-id="6a419-141">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="6a419-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="6a419-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="6a419-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a419-143">DateTimeOffset</span></span>|<span data-ttu-id="6a419-144">時間登録プロファイルが[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスに割り当てられています。</span><span class="sxs-lookup"><span data-stu-id="6a419-144">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="6a419-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="6a419-145">isSupervised</span></span>|<span data-ttu-id="6a419-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a419-146">Boolean</span></span>|<span data-ttu-id="6a419-147">Apple デバイスが監視されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6a419-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="6a419-148">詳細についてはhttps://support.apple.com/en-us/HT202837 、「 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a419-148">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="6a419-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="6a419-149">discoverySource</span></span>|[<span data-ttu-id="6a419-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="6a419-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="6a419-151">Apple デバイスの検出ソース。</span><span class="sxs-lookup"><span data-stu-id="6a419-151">Apple device discovery source.</span></span> <span data-ttu-id="6a419-152">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="6a419-152">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="6a419-153">可能な値は、`unknown`、`adminImport`、`deviceEnrollmentProgram` です。</span><span class="sxs-lookup"><span data-stu-id="6a419-153">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="6a419-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a419-154">createdDateTime</span></span>|<span data-ttu-id="6a419-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a419-155">DateTimeOffset</span></span>|<span data-ttu-id="6a419-156">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスの日時の作成日時</span><span class="sxs-lookup"><span data-stu-id="6a419-156">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="6a419-157">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a419-157">lastContactedDateTime</span></span>|<span data-ttu-id="6a419-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a419-158">DateTimeOffset</span></span>|<span data-ttu-id="6a419-159">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスの最後の連絡日時。</span><span class="sxs-lookup"><span data-stu-id="6a419-159">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="6a419-160">description</span><span class="sxs-lookup"><span data-stu-id="6a419-160">description</span></span>|<span data-ttu-id="6a419-161">String</span><span class="sxs-lookup"><span data-stu-id="6a419-161">String</span></span>|<span data-ttu-id="6a419-162">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスの説明</span><span class="sxs-lookup"><span data-stu-id="6a419-162">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="6a419-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="6a419-163">enrollmentState</span></span>|[<span data-ttu-id="6a419-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="6a419-164">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="6a419-165">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承された Intune のデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="6a419-165">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="6a419-166">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="6a419-166">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="6a419-167">platform</span><span class="sxs-lookup"><span data-stu-id="6a419-167">platform</span></span>|[<span data-ttu-id="6a419-168">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="6a419-168">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="6a419-169">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="6a419-169">The platform of the Device.</span></span> <span data-ttu-id="6a419-170">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="6a419-170">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="6a419-171">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="6a419-171">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="6a419-172">status</span><span class="sxs-lookup"><span data-stu-id="6a419-172">status</span></span>|<span data-ttu-id="6a419-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a419-173">Boolean</span></span>|<span data-ttu-id="6a419-174">インポートされたデバイス id の状態</span><span class="sxs-lookup"><span data-stu-id="6a419-174">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="6a419-175">応答</span><span class="sxs-lookup"><span data-stu-id="6a419-175">Response</span></span>
<span data-ttu-id="6a419-176">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6a419-176">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a419-177">例</span><span class="sxs-lookup"><span data-stu-id="6a419-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a419-178">要求</span><span class="sxs-lookup"><span data-stu-id="6a419-178">Request</span></span>
<span data-ttu-id="6a419-179">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6a419-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6a419-180">応答</span><span class="sxs-lookup"><span data-stu-id="6a419-180">Response</span></span>
<span data-ttu-id="6a419-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6a419-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






