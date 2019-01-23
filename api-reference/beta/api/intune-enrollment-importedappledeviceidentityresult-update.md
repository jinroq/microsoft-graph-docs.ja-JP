---
title: ImportedAppleDeviceIdentityResult を更新します。
description: ImportedAppleDeviceIdentityResult オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d721da146e86e05b1e99a53c6570a8681adf7a06
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396456"
---
# <a name="update-importedappledeviceidentityresult"></a><span data-ttu-id="e4688-103">ImportedAppleDeviceIdentityResult を更新します。</span><span class="sxs-lookup"><span data-stu-id="e4688-103">Update importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="e4688-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e4688-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e4688-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e4688-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4688-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e4688-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4688-107">[ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e4688-107">Update the properties of a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4688-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e4688-108">Prerequisites</span></span>
<span data-ttu-id="e4688-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4688-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e4688-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e4688-111">Permission type</span></span>|<span data-ttu-id="e4688-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e4688-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4688-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e4688-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4688-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4688-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e4688-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e4688-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4688-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e4688-116">Not supported.</span></span>|
|<span data-ttu-id="e4688-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e4688-117">Application</span></span>|<span data-ttu-id="e4688-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e4688-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4688-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e4688-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="e4688-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e4688-120">Request headers</span></span>
|<span data-ttu-id="e4688-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e4688-121">Header</span></span>|<span data-ttu-id="e4688-122">値</span><span class="sxs-lookup"><span data-stu-id="e4688-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4688-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4688-123">Authorization</span></span>|<span data-ttu-id="e4688-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e4688-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4688-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e4688-125">Accept</span></span>|<span data-ttu-id="e4688-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4688-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4688-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e4688-127">Request body</span></span>
<span data-ttu-id="e4688-128">要求の本文に[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="e4688-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

<span data-ttu-id="e4688-129">[ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="e4688-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

|<span data-ttu-id="e4688-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4688-130">Property</span></span>|<span data-ttu-id="e4688-131">型</span><span class="sxs-lookup"><span data-stu-id="e4688-131">Type</span></span>|<span data-ttu-id="e4688-132">説明</span><span class="sxs-lookup"><span data-stu-id="e4688-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4688-133">id</span><span class="sxs-lookup"><span data-stu-id="e4688-133">id</span></span>|<span data-ttu-id="e4688-134">String</span><span class="sxs-lookup"><span data-stu-id="e4688-134">String</span></span>|<span data-ttu-id="e4688-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e4688-135">Key of the entity.</span></span> <span data-ttu-id="e4688-136">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="e4688-136">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="e4688-137">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="e4688-137">serialNumber</span></span>|<span data-ttu-id="e4688-138">String</span><span class="sxs-lookup"><span data-stu-id="e4688-138">String</span></span>|<span data-ttu-id="e4688-139">継承されるデバイス ・ シリアル番号は、 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から</span><span class="sxs-lookup"><span data-stu-id="e4688-139">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="e4688-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="e4688-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="e4688-141">String</span><span class="sxs-lookup"><span data-stu-id="e4688-141">String</span></span>|<span data-ttu-id="e4688-142">登録プロファイル Id の管理者が、 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承される、次の登録時に、デバイスに適用しようとしています。</span><span class="sxs-lookup"><span data-stu-id="e4688-142">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="e4688-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="e4688-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="e4688-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4688-144">DateTimeOffset</span></span>|<span data-ttu-id="e4688-145">時間登録のプロファイルは、 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されるデバイスに割り当てられました。</span><span class="sxs-lookup"><span data-stu-id="e4688-145">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="e4688-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="e4688-146">isSupervised</span></span>|<span data-ttu-id="e4688-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4688-147">Boolean</span></span>|<span data-ttu-id="e4688-148">Apple デバイスが監視された状態を示します。</span><span class="sxs-lookup"><span data-stu-id="e4688-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="e4688-149">詳細については、: https://support.apple.com/en-us/HT202837 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="e4688-149">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="e4688-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="e4688-150">discoverySource</span></span>|[<span data-ttu-id="e4688-151">discoverySource</span><span class="sxs-lookup"><span data-stu-id="e4688-151">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="e4688-152">Apple のデバイス検出のソースです。</span><span class="sxs-lookup"><span data-stu-id="e4688-152">Apple device discovery source.</span></span> <span data-ttu-id="e4688-153">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e4688-153">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="e4688-154">可能な値は、`unknown`、`adminImport`、`deviceEnrollmentProgram` です。</span><span class="sxs-lookup"><span data-stu-id="e4688-154">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="e4688-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4688-155">createdDateTime</span></span>|<span data-ttu-id="e4688-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4688-156">DateTimeOffset</span></span>|<span data-ttu-id="e4688-157">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承される、デバイスの日時を作成</span><span class="sxs-lookup"><span data-stu-id="e4688-157">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="e4688-158">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4688-158">lastContactedDateTime</span></span>|<span data-ttu-id="e4688-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4688-159">DateTimeOffset</span></span>|<span data-ttu-id="e4688-160">最終接続日時[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されるデバイスの</span><span class="sxs-lookup"><span data-stu-id="e4688-160">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="e4688-161">説明</span><span class="sxs-lookup"><span data-stu-id="e4688-161">description</span></span>|<span data-ttu-id="e4688-162">String</span><span class="sxs-lookup"><span data-stu-id="e4688-162">String</span></span>|<span data-ttu-id="e4688-163">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承される、デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="e4688-163">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="e4688-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="e4688-164">enrollmentState</span></span>|[<span data-ttu-id="e4688-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="e4688-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="e4688-166">Intune 継承で[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)からのデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="e4688-166">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="e4688-167">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="e4688-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="e4688-168">platform</span><span class="sxs-lookup"><span data-stu-id="e4688-168">platform</span></span>|[<span data-ttu-id="e4688-169">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="e4688-169">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="e4688-170">デバイスのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="e4688-170">The platform of the Device.</span></span> <span data-ttu-id="e4688-171">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e4688-171">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="e4688-172">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="e4688-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="e4688-173">status</span><span class="sxs-lookup"><span data-stu-id="e4688-173">status</span></span>|<span data-ttu-id="e4688-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4688-174">Boolean</span></span>|<span data-ttu-id="e4688-175">インポートされたデバイス id のステータス</span><span class="sxs-lookup"><span data-stu-id="e4688-175">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="e4688-176">応答</span><span class="sxs-lookup"><span data-stu-id="e4688-176">Response</span></span>
<span data-ttu-id="e4688-177">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e4688-177">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4688-178">例</span><span class="sxs-lookup"><span data-stu-id="e4688-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4688-179">要求</span><span class="sxs-lookup"><span data-stu-id="e4688-179">Request</span></span>
<span data-ttu-id="e4688-180">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e4688-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e4688-181">応答</span><span class="sxs-lookup"><span data-stu-id="e4688-181">Response</span></span>
<span data-ttu-id="e4688-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e4688-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




