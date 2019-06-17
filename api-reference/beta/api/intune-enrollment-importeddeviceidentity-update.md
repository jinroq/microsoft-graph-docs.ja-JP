---
title: ImportedDeviceIdentity の更新
description: ImportedDeviceIdentity オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a95cd0b74c35d0d9a8e3a22b6fc9ad66d80d397
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981840"
---
# <a name="update-importeddeviceidentity"></a><span data-ttu-id="a46ff-103">ImportedDeviceIdentity の更新</span><span class="sxs-lookup"><span data-stu-id="a46ff-103">Update importedDeviceIdentity</span></span>

> <span data-ttu-id="a46ff-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a46ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a46ff-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a46ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a46ff-106">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a46ff-106">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a46ff-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a46ff-107">Prerequisites</span></span>
<span data-ttu-id="a46ff-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a46ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a46ff-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a46ff-110">Permission type</span></span>|<span data-ttu-id="a46ff-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a46ff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a46ff-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a46ff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a46ff-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a46ff-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a46ff-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a46ff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a46ff-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a46ff-115">Not supported.</span></span>|
|<span data-ttu-id="a46ff-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a46ff-116">Application</span></span>|<span data-ttu-id="a46ff-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a46ff-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a46ff-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a46ff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="a46ff-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a46ff-119">Request headers</span></span>
|<span data-ttu-id="a46ff-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a46ff-120">Header</span></span>|<span data-ttu-id="a46ff-121">値</span><span class="sxs-lookup"><span data-stu-id="a46ff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a46ff-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a46ff-122">Authorization</span></span>|<span data-ttu-id="a46ff-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a46ff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a46ff-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a46ff-124">Accept</span></span>|<span data-ttu-id="a46ff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a46ff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a46ff-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a46ff-126">Request body</span></span>
<span data-ttu-id="a46ff-127">要求本文で、 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a46ff-127">In the request body, supply a JSON representation for the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

<span data-ttu-id="a46ff-128">次の表に、 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a46ff-128">The following table shows the properties that are required when you create the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>

|<span data-ttu-id="a46ff-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a46ff-129">Property</span></span>|<span data-ttu-id="a46ff-130">型</span><span class="sxs-lookup"><span data-stu-id="a46ff-130">Type</span></span>|<span data-ttu-id="a46ff-131">説明</span><span class="sxs-lookup"><span data-stu-id="a46ff-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a46ff-132">id</span><span class="sxs-lookup"><span data-stu-id="a46ff-132">id</span></span>|<span data-ttu-id="a46ff-133">String</span><span class="sxs-lookup"><span data-stu-id="a46ff-133">String</span></span>|<span data-ttu-id="a46ff-134">インポートされたデバイス id の id</span><span class="sxs-lookup"><span data-stu-id="a46ff-134">Id of the imported device identity</span></span>|
|<span data-ttu-id="a46ff-135">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="a46ff-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="a46ff-136">String</span><span class="sxs-lookup"><span data-stu-id="a46ff-136">String</span></span>|<span data-ttu-id="a46ff-137">インポートされたデバイス識別子</span><span class="sxs-lookup"><span data-stu-id="a46ff-137">Imported Device Identifier</span></span>|
|<span data-ttu-id="a46ff-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="a46ff-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="a46ff-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="a46ff-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="a46ff-140">インポートされたデバイス Id の種類。</span><span class="sxs-lookup"><span data-stu-id="a46ff-140">Type of Imported Device Identity.</span></span> <span data-ttu-id="a46ff-141">可能な値は、`unknown`、`imei`、`serialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="a46ff-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="a46ff-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a46ff-142">lastModifiedDateTime</span></span>|<span data-ttu-id="a46ff-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a46ff-143">DateTimeOffset</span></span>|<span data-ttu-id="a46ff-144">説明の最終更新日時</span><span class="sxs-lookup"><span data-stu-id="a46ff-144">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="a46ff-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a46ff-145">createdDateTime</span></span>|<span data-ttu-id="a46ff-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a46ff-146">DateTimeOffset</span></span>|<span data-ttu-id="a46ff-147">デバイスの日時の作成日時</span><span class="sxs-lookup"><span data-stu-id="a46ff-147">Created Date Time of the device</span></span>|
|<span data-ttu-id="a46ff-148">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="a46ff-148">lastContactedDateTime</span></span>|<span data-ttu-id="a46ff-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a46ff-149">DateTimeOffset</span></span>|<span data-ttu-id="a46ff-150">デバイスの最終連絡日時</span><span class="sxs-lookup"><span data-stu-id="a46ff-150">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="a46ff-151">description</span><span class="sxs-lookup"><span data-stu-id="a46ff-151">description</span></span>|<span data-ttu-id="a46ff-152">String</span><span class="sxs-lookup"><span data-stu-id="a46ff-152">String</span></span>|<span data-ttu-id="a46ff-153">デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="a46ff-153">The description of the device</span></span>|
|<span data-ttu-id="a46ff-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="a46ff-154">enrollmentState</span></span>|[<span data-ttu-id="a46ff-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="a46ff-155">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="a46ff-156">Intune でのデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="a46ff-156">The state of the device in Intune.</span></span> <span data-ttu-id="a46ff-157">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="a46ff-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="a46ff-158">platform</span><span class="sxs-lookup"><span data-stu-id="a46ff-158">platform</span></span>|[<span data-ttu-id="a46ff-159">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="a46ff-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="a46ff-160">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="a46ff-160">The platform of the Device.</span></span> <span data-ttu-id="a46ff-161">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="a46ff-161">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="a46ff-162">応答</span><span class="sxs-lookup"><span data-stu-id="a46ff-162">Response</span></span>
<span data-ttu-id="a46ff-163">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a46ff-163">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a46ff-164">例</span><span class="sxs-lookup"><span data-stu-id="a46ff-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="a46ff-165">要求</span><span class="sxs-lookup"><span data-stu-id="a46ff-165">Request</span></span>
<span data-ttu-id="a46ff-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a46ff-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
Content-type: application/json
Content-length: 332

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="a46ff-167">応答</span><span class="sxs-lookup"><span data-stu-id="a46ff-167">Response</span></span>
<span data-ttu-id="a46ff-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a46ff-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```





