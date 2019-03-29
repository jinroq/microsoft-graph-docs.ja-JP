---
title: importedAppleDeviceIdentityResult の更新
description: importedAppleDeviceIdentityResult オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c52a6c6dc591a2ccb5c8bd71dbc7f5c074d8564
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969604"
---
# <a name="update-importedappledeviceidentityresult"></a><span data-ttu-id="66887-103">importedAppleDeviceIdentityResult の更新</span><span class="sxs-lookup"><span data-stu-id="66887-103">Update importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="66887-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66887-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66887-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="66887-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66887-106">[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="66887-106">Update the properties of a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66887-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="66887-107">Prerequisites</span></span>
<span data-ttu-id="66887-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66887-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66887-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66887-110">Permission type</span></span>|<span data-ttu-id="66887-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="66887-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66887-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="66887-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66887-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66887-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="66887-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66887-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66887-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66887-115">Not supported.</span></span>|
|<span data-ttu-id="66887-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66887-116">Application</span></span>|<span data-ttu-id="66887-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66887-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66887-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66887-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="66887-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66887-119">Request headers</span></span>
|<span data-ttu-id="66887-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66887-120">Header</span></span>|<span data-ttu-id="66887-121">値</span><span class="sxs-lookup"><span data-stu-id="66887-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66887-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="66887-122">Authorization</span></span>|<span data-ttu-id="66887-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="66887-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66887-124">承諾</span><span class="sxs-lookup"><span data-stu-id="66887-124">Accept</span></span>|<span data-ttu-id="66887-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66887-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66887-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="66887-126">Request body</span></span>
<span data-ttu-id="66887-127">要求本文で、 [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="66887-127">In the request body, supply a JSON representation for the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

<span data-ttu-id="66887-128">次の表に、 [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="66887-128">The following table shows the properties that are required when you create the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

|<span data-ttu-id="66887-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66887-129">Property</span></span>|<span data-ttu-id="66887-130">型</span><span class="sxs-lookup"><span data-stu-id="66887-130">Type</span></span>|<span data-ttu-id="66887-131">説明</span><span class="sxs-lookup"><span data-stu-id="66887-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66887-132">id</span><span class="sxs-lookup"><span data-stu-id="66887-132">id</span></span>|<span data-ttu-id="66887-133">String</span><span class="sxs-lookup"><span data-stu-id="66887-133">String</span></span>|<span data-ttu-id="66887-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="66887-134">Key of the entity.</span></span> <span data-ttu-id="66887-135">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="66887-135">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="66887-136">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="66887-136">serialNumber</span></span>|<span data-ttu-id="66887-137">String</span><span class="sxs-lookup"><span data-stu-id="66887-137">String</span></span>|<span data-ttu-id="66887-138">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスのシリアル番号</span><span class="sxs-lookup"><span data-stu-id="66887-138">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="66887-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="66887-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="66887-140">String</span><span class="sxs-lookup"><span data-stu-id="66887-140">String</span></span>|<span data-ttu-id="66887-141">登録プロファイル Id 管理者は、 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承した次の登録時にデバイスに適用する予定です。</span><span class="sxs-lookup"><span data-stu-id="66887-141">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="66887-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="66887-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="66887-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66887-143">DateTimeOffset</span></span>|<span data-ttu-id="66887-144">時間登録プロファイルが[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスに割り当てられています。</span><span class="sxs-lookup"><span data-stu-id="66887-144">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="66887-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="66887-145">isSupervised</span></span>|<span data-ttu-id="66887-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="66887-146">Boolean</span></span>|<span data-ttu-id="66887-147">Apple デバイスが監視されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="66887-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="66887-148">詳細についてはhttps://support.apple.com/en-us/HT202837 、「 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66887-148">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="66887-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="66887-149">discoverySource</span></span>|[<span data-ttu-id="66887-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="66887-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="66887-151">Apple デバイスの検出ソース。</span><span class="sxs-lookup"><span data-stu-id="66887-151">Apple device discovery source.</span></span> <span data-ttu-id="66887-152">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="66887-152">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="66887-153">使用可能な値は、`unknown`、`adminImport`、`deviceEnrollmentProgram` です。</span><span class="sxs-lookup"><span data-stu-id="66887-153">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="66887-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66887-154">createdDateTime</span></span>|<span data-ttu-id="66887-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66887-155">DateTimeOffset</span></span>|<span data-ttu-id="66887-156">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスの日時の作成日時</span><span class="sxs-lookup"><span data-stu-id="66887-156">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="66887-157">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="66887-157">lastContactedDateTime</span></span>|<span data-ttu-id="66887-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66887-158">DateTimeOffset</span></span>|<span data-ttu-id="66887-159">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスの最後の連絡日時。</span><span class="sxs-lookup"><span data-stu-id="66887-159">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="66887-160">description</span><span class="sxs-lookup"><span data-stu-id="66887-160">description</span></span>|<span data-ttu-id="66887-161">String</span><span class="sxs-lookup"><span data-stu-id="66887-161">String</span></span>|<span data-ttu-id="66887-162">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されたデバイスの説明</span><span class="sxs-lookup"><span data-stu-id="66887-162">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="66887-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="66887-163">enrollmentState</span></span>|[<span data-ttu-id="66887-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="66887-164">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="66887-165">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承された Intune のデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="66887-165">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="66887-166">可能な値は `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked` です。</span><span class="sxs-lookup"><span data-stu-id="66887-166">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="66887-167">platform</span><span class="sxs-lookup"><span data-stu-id="66887-167">platform</span></span>|[<span data-ttu-id="66887-168">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="66887-168">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="66887-169">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="66887-169">The platform of the Device.</span></span> <span data-ttu-id="66887-170">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="66887-170">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="66887-171">可能な値は `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS` です。</span><span class="sxs-lookup"><span data-stu-id="66887-171">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="66887-172">status</span><span class="sxs-lookup"><span data-stu-id="66887-172">status</span></span>|<span data-ttu-id="66887-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="66887-173">Boolean</span></span>|<span data-ttu-id="66887-174">インポートされたデバイス id の状態</span><span class="sxs-lookup"><span data-stu-id="66887-174">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="66887-175">応答</span><span class="sxs-lookup"><span data-stu-id="66887-175">Response</span></span>
<span data-ttu-id="66887-176">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="66887-176">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66887-177">例</span><span class="sxs-lookup"><span data-stu-id="66887-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="66887-178">要求</span><span class="sxs-lookup"><span data-stu-id="66887-178">Request</span></span>
<span data-ttu-id="66887-179">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="66887-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="66887-180">応答</span><span class="sxs-lookup"><span data-stu-id="66887-180">Response</span></span>
<span data-ttu-id="66887-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="66887-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




