---
title: ImportedAppleDeviceIdentity を更新します。
description: ImportedAppleDeviceIdentity オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7970c0c74c7200d6a991a48f986125747589195c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412171"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="965db-103">ImportedAppleDeviceIdentity を更新します。</span><span class="sxs-lookup"><span data-stu-id="965db-103">Update importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="965db-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="965db-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="965db-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="965db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="965db-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="965db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="965db-107">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="965db-107">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="965db-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="965db-108">Prerequisites</span></span>
<span data-ttu-id="965db-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="965db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="965db-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="965db-111">Permission type</span></span>|<span data-ttu-id="965db-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="965db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="965db-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="965db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="965db-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="965db-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="965db-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="965db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="965db-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="965db-116">Not supported.</span></span>|
|<span data-ttu-id="965db-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="965db-117">Application</span></span>|<span data-ttu-id="965db-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="965db-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="965db-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="965db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="965db-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="965db-120">Request headers</span></span>
|<span data-ttu-id="965db-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="965db-121">Header</span></span>|<span data-ttu-id="965db-122">値</span><span class="sxs-lookup"><span data-stu-id="965db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="965db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="965db-123">Authorization</span></span>|<span data-ttu-id="965db-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="965db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="965db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="965db-125">Accept</span></span>|<span data-ttu-id="965db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="965db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="965db-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="965db-127">Request body</span></span>
<span data-ttu-id="965db-128">要求の本文に[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="965db-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="965db-129">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="965db-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="965db-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="965db-130">Property</span></span>|<span data-ttu-id="965db-131">型</span><span class="sxs-lookup"><span data-stu-id="965db-131">Type</span></span>|<span data-ttu-id="965db-132">説明</span><span class="sxs-lookup"><span data-stu-id="965db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="965db-133">id</span><span class="sxs-lookup"><span data-stu-id="965db-133">id</span></span>|<span data-ttu-id="965db-134">String</span><span class="sxs-lookup"><span data-stu-id="965db-134">String</span></span>|<span data-ttu-id="965db-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="965db-135">Key of the entity.</span></span>|
|<span data-ttu-id="965db-136">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="965db-136">serialNumber</span></span>|<span data-ttu-id="965db-137">String</span><span class="sxs-lookup"><span data-stu-id="965db-137">String</span></span>|<span data-ttu-id="965db-138">デバイスのシリアル番号</span><span class="sxs-lookup"><span data-stu-id="965db-138">Device serial number</span></span>|
|<span data-ttu-id="965db-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="965db-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="965db-140">String</span><span class="sxs-lookup"><span data-stu-id="965db-140">String</span></span>|<span data-ttu-id="965db-141">登録プロファイル Id の管理者が、次の登録時にデバイスに適用しようとしています。</span><span class="sxs-lookup"><span data-stu-id="965db-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="965db-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="965db-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="965db-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="965db-143">DateTimeOffset</span></span>|<span data-ttu-id="965db-144">時間登録のプロファイルは、デバイスに割り当てられました。</span><span class="sxs-lookup"><span data-stu-id="965db-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="965db-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="965db-145">isSupervised</span></span>|<span data-ttu-id="965db-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="965db-146">Boolean</span></span>|<span data-ttu-id="965db-147">Apple デバイスが監視された状態を示します。</span><span class="sxs-lookup"><span data-stu-id="965db-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="965db-148">詳細についてでです。https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="965db-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="965db-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="965db-149">discoverySource</span></span>|[<span data-ttu-id="965db-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="965db-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="965db-151">Apple のデバイス検出のソースです。</span><span class="sxs-lookup"><span data-stu-id="965db-151">Apple device discovery source.</span></span> <span data-ttu-id="965db-152">可能な値は、`unknown`、`adminImport`、`deviceEnrollmentProgram` です。</span><span class="sxs-lookup"><span data-stu-id="965db-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="965db-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="965db-153">createdDateTime</span></span>|<span data-ttu-id="965db-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="965db-154">DateTimeOffset</span></span>|<span data-ttu-id="965db-155">デバイスの作成日時</span><span class="sxs-lookup"><span data-stu-id="965db-155">Created Date Time of the device</span></span>|
|<span data-ttu-id="965db-156">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="965db-156">lastContactedDateTime</span></span>|<span data-ttu-id="965db-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="965db-157">DateTimeOffset</span></span>|<span data-ttu-id="965db-158">最終アクセス日時、デバイスの</span><span class="sxs-lookup"><span data-stu-id="965db-158">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="965db-159">説明</span><span class="sxs-lookup"><span data-stu-id="965db-159">description</span></span>|<span data-ttu-id="965db-160">String</span><span class="sxs-lookup"><span data-stu-id="965db-160">String</span></span>|<span data-ttu-id="965db-161">デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="965db-161">The description of the device</span></span>|
|<span data-ttu-id="965db-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="965db-162">enrollmentState</span></span>|[<span data-ttu-id="965db-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="965db-163">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="965db-164">Intune でデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="965db-164">The state of the device in Intune.</span></span> <span data-ttu-id="965db-165">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="965db-165">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="965db-166">platform</span><span class="sxs-lookup"><span data-stu-id="965db-166">platform</span></span>|[<span data-ttu-id="965db-167">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="965db-167">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="965db-168">デバイスのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="965db-168">The platform of the Device.</span></span> <span data-ttu-id="965db-169">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="965db-169">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="965db-170">応答</span><span class="sxs-lookup"><span data-stu-id="965db-170">Response</span></span>
<span data-ttu-id="965db-171">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="965db-171">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="965db-172">例</span><span class="sxs-lookup"><span data-stu-id="965db-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="965db-173">要求</span><span class="sxs-lookup"><span data-stu-id="965db-173">Request</span></span>
<span data-ttu-id="965db-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="965db-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="965db-175">応答</span><span class="sxs-lookup"><span data-stu-id="965db-175">Response</span></span>
<span data-ttu-id="965db-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="965db-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




