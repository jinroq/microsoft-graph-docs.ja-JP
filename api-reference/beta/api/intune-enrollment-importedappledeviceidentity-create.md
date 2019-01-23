---
title: ImportedAppleDeviceIdentity を作成します。
description: 新しい importedAppleDeviceIdentity オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 839e604fc52c22ff08a963d5601b987780ee241c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422377"
---
# <a name="create-importedappledeviceidentity"></a><span data-ttu-id="7d692-103">ImportedAppleDeviceIdentity を作成します。</span><span class="sxs-lookup"><span data-stu-id="7d692-103">Create importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="7d692-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7d692-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7d692-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d692-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d692-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d692-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d692-107">新しい[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7d692-107">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d692-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7d692-108">Prerequisites</span></span>
<span data-ttu-id="7d692-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d692-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7d692-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d692-111">Permission type</span></span>|<span data-ttu-id="7d692-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d692-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d692-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d692-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d692-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d692-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7d692-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d692-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d692-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d692-116">Not supported.</span></span>|
|<span data-ttu-id="7d692-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d692-117">Application</span></span>|<span data-ttu-id="7d692-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d692-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d692-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d692-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="7d692-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d692-120">Request headers</span></span>
|<span data-ttu-id="7d692-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d692-121">Header</span></span>|<span data-ttu-id="7d692-122">値</span><span class="sxs-lookup"><span data-stu-id="7d692-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d692-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d692-123">Authorization</span></span>|<span data-ttu-id="7d692-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7d692-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d692-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7d692-125">Accept</span></span>|<span data-ttu-id="7d692-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d692-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d692-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7d692-127">Request body</span></span>
<span data-ttu-id="7d692-128">要求の本文に importedAppleDeviceIdentity オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="7d692-128">In the request body, supply a JSON representation for the importedAppleDeviceIdentity object.</span></span>

<span data-ttu-id="7d692-129">次の表は、importedAppleDeviceIdentity を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7d692-129">The following table shows the properties that are required when you create the importedAppleDeviceIdentity.</span></span>

|<span data-ttu-id="7d692-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d692-130">Property</span></span>|<span data-ttu-id="7d692-131">型</span><span class="sxs-lookup"><span data-stu-id="7d692-131">Type</span></span>|<span data-ttu-id="7d692-132">説明</span><span class="sxs-lookup"><span data-stu-id="7d692-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d692-133">id</span><span class="sxs-lookup"><span data-stu-id="7d692-133">id</span></span>|<span data-ttu-id="7d692-134">String</span><span class="sxs-lookup"><span data-stu-id="7d692-134">String</span></span>|<span data-ttu-id="7d692-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7d692-135">Key of the entity.</span></span>|
|<span data-ttu-id="7d692-136">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="7d692-136">serialNumber</span></span>|<span data-ttu-id="7d692-137">String</span><span class="sxs-lookup"><span data-stu-id="7d692-137">String</span></span>|<span data-ttu-id="7d692-138">デバイスのシリアル番号</span><span class="sxs-lookup"><span data-stu-id="7d692-138">Device serial number</span></span>|
|<span data-ttu-id="7d692-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="7d692-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="7d692-140">String</span><span class="sxs-lookup"><span data-stu-id="7d692-140">String</span></span>|<span data-ttu-id="7d692-141">登録プロファイル Id の管理者が、次の登録時にデバイスに適用しようとしています。</span><span class="sxs-lookup"><span data-stu-id="7d692-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="7d692-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="7d692-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="7d692-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d692-143">DateTimeOffset</span></span>|<span data-ttu-id="7d692-144">時間登録のプロファイルは、デバイスに割り当てられました。</span><span class="sxs-lookup"><span data-stu-id="7d692-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="7d692-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="7d692-145">isSupervised</span></span>|<span data-ttu-id="7d692-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d692-146">Boolean</span></span>|<span data-ttu-id="7d692-147">Apple デバイスが監視された状態を示します。</span><span class="sxs-lookup"><span data-stu-id="7d692-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="7d692-148">詳細についてでです。https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="7d692-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="7d692-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="7d692-149">discoverySource</span></span>|[<span data-ttu-id="7d692-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="7d692-150">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="7d692-151">Apple のデバイス検出のソースです。</span><span class="sxs-lookup"><span data-stu-id="7d692-151">Apple device discovery source.</span></span> <span data-ttu-id="7d692-152">可能な値は、`unknown`、`adminImport`、`deviceEnrollmentProgram` です。</span><span class="sxs-lookup"><span data-stu-id="7d692-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="7d692-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d692-153">createdDateTime</span></span>|<span data-ttu-id="7d692-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d692-154">DateTimeOffset</span></span>|<span data-ttu-id="7d692-155">デバイスの作成日時</span><span class="sxs-lookup"><span data-stu-id="7d692-155">Created Date Time of the device</span></span>|
|<span data-ttu-id="7d692-156">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d692-156">lastContactedDateTime</span></span>|<span data-ttu-id="7d692-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d692-157">DateTimeOffset</span></span>|<span data-ttu-id="7d692-158">最終アクセス日時、デバイスの</span><span class="sxs-lookup"><span data-stu-id="7d692-158">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="7d692-159">説明</span><span class="sxs-lookup"><span data-stu-id="7d692-159">description</span></span>|<span data-ttu-id="7d692-160">String</span><span class="sxs-lookup"><span data-stu-id="7d692-160">String</span></span>|<span data-ttu-id="7d692-161">デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="7d692-161">The description of the device</span></span>|
|<span data-ttu-id="7d692-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="7d692-162">enrollmentState</span></span>|[<span data-ttu-id="7d692-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="7d692-163">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="7d692-164">Intune でデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="7d692-164">The state of the device in Intune.</span></span> <span data-ttu-id="7d692-165">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="7d692-165">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="7d692-166">platform</span><span class="sxs-lookup"><span data-stu-id="7d692-166">platform</span></span>|[<span data-ttu-id="7d692-167">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="7d692-167">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="7d692-168">デバイスのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="7d692-168">The platform of the Device.</span></span> <span data-ttu-id="7d692-169">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="7d692-169">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="7d692-170">応答</span><span class="sxs-lookup"><span data-stu-id="7d692-170">Response</span></span>
<span data-ttu-id="7d692-171">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7d692-171">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d692-172">例</span><span class="sxs-lookup"><span data-stu-id="7d692-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d692-173">要求</span><span class="sxs-lookup"><span data-stu-id="7d692-173">Request</span></span>
<span data-ttu-id="7d692-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7d692-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7d692-175">応答</span><span class="sxs-lookup"><span data-stu-id="7d692-175">Response</span></span>
<span data-ttu-id="7d692-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7d692-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




