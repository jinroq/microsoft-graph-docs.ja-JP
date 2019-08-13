---
title: ImportedDeviceIdentity を作成する
description: 新しい importedDeviceIdentity オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4b1f23e95a8012a2804e943a30c95fe89261d963
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356460"
---
# <a name="create-importeddeviceidentity"></a><span data-ttu-id="ee4cb-103">ImportedDeviceIdentity を作成する</span><span class="sxs-lookup"><span data-stu-id="ee4cb-103">Create importedDeviceIdentity</span></span>

> <span data-ttu-id="ee4cb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee4cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee4cb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee4cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee4cb-106">新しい[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ee4cb-106">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee4cb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ee4cb-107">Prerequisites</span></span>
<span data-ttu-id="ee4cb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee4cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee4cb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee4cb-110">Permission type</span></span>|<span data-ttu-id="ee4cb-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee4cb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee4cb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee4cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee4cb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee4cb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ee4cb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee4cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee4cb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee4cb-115">Not supported.</span></span>|
|<span data-ttu-id="ee4cb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee4cb-116">Application</span></span>|<span data-ttu-id="ee4cb-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee4cb-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee4cb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee4cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="ee4cb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee4cb-119">Request headers</span></span>
|<span data-ttu-id="ee4cb-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee4cb-120">Header</span></span>|<span data-ttu-id="ee4cb-121">値</span><span class="sxs-lookup"><span data-stu-id="ee4cb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee4cb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee4cb-122">Authorization</span></span>|<span data-ttu-id="ee4cb-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee4cb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee4cb-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ee4cb-124">Accept</span></span>|<span data-ttu-id="ee4cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee4cb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee4cb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee4cb-126">Request body</span></span>
<span data-ttu-id="ee4cb-127">要求本文で、importedDeviceIdentity オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee4cb-127">In the request body, supply a JSON representation for the importedDeviceIdentity object.</span></span>

<span data-ttu-id="ee4cb-128">次の表に、importedDeviceIdentity の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ee4cb-128">The following table shows the properties that are required when you create the importedDeviceIdentity.</span></span>

|<span data-ttu-id="ee4cb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee4cb-129">Property</span></span>|<span data-ttu-id="ee4cb-130">型</span><span class="sxs-lookup"><span data-stu-id="ee4cb-130">Type</span></span>|<span data-ttu-id="ee4cb-131">説明</span><span class="sxs-lookup"><span data-stu-id="ee4cb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee4cb-132">id</span><span class="sxs-lookup"><span data-stu-id="ee4cb-132">id</span></span>|<span data-ttu-id="ee4cb-133">String</span><span class="sxs-lookup"><span data-stu-id="ee4cb-133">String</span></span>|<span data-ttu-id="ee4cb-134">インポートされたデバイス id の id</span><span class="sxs-lookup"><span data-stu-id="ee4cb-134">Id of the imported device identity</span></span>|
|<span data-ttu-id="ee4cb-135">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="ee4cb-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="ee4cb-136">String</span><span class="sxs-lookup"><span data-stu-id="ee4cb-136">String</span></span>|<span data-ttu-id="ee4cb-137">インポートされたデバイス識別子</span><span class="sxs-lookup"><span data-stu-id="ee4cb-137">Imported Device Identifier</span></span>|
|<span data-ttu-id="ee4cb-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="ee4cb-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="ee4cb-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="ee4cb-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="ee4cb-140">インポートされたデバイス Id の種類。</span><span class="sxs-lookup"><span data-stu-id="ee4cb-140">Type of Imported Device Identity.</span></span> <span data-ttu-id="ee4cb-141">可能な値は、`unknown`、`imei`、`serialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="ee4cb-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="ee4cb-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee4cb-142">lastModifiedDateTime</span></span>|<span data-ttu-id="ee4cb-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee4cb-143">DateTimeOffset</span></span>|<span data-ttu-id="ee4cb-144">説明の最終更新日時</span><span class="sxs-lookup"><span data-stu-id="ee4cb-144">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="ee4cb-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee4cb-145">createdDateTime</span></span>|<span data-ttu-id="ee4cb-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee4cb-146">DateTimeOffset</span></span>|<span data-ttu-id="ee4cb-147">デバイスの日時の作成日時</span><span class="sxs-lookup"><span data-stu-id="ee4cb-147">Created Date Time of the device</span></span>|
|<span data-ttu-id="ee4cb-148">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee4cb-148">lastContactedDateTime</span></span>|<span data-ttu-id="ee4cb-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee4cb-149">DateTimeOffset</span></span>|<span data-ttu-id="ee4cb-150">デバイスの最終連絡日時</span><span class="sxs-lookup"><span data-stu-id="ee4cb-150">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="ee4cb-151">description</span><span class="sxs-lookup"><span data-stu-id="ee4cb-151">description</span></span>|<span data-ttu-id="ee4cb-152">String</span><span class="sxs-lookup"><span data-stu-id="ee4cb-152">String</span></span>|<span data-ttu-id="ee4cb-153">デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="ee4cb-153">The description of the device</span></span>|
|<span data-ttu-id="ee4cb-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="ee4cb-154">enrollmentState</span></span>|[<span data-ttu-id="ee4cb-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="ee4cb-155">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="ee4cb-156">Intune でのデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="ee4cb-156">The state of the device in Intune.</span></span> <span data-ttu-id="ee4cb-157">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="ee4cb-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="ee4cb-158">platform</span><span class="sxs-lookup"><span data-stu-id="ee4cb-158">platform</span></span>|[<span data-ttu-id="ee4cb-159">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="ee4cb-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="ee4cb-160">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="ee4cb-160">The platform of the Device.</span></span> <span data-ttu-id="ee4cb-161">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="ee4cb-161">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="ee4cb-162">応答</span><span class="sxs-lookup"><span data-stu-id="ee4cb-162">Response</span></span>
<span data-ttu-id="ee4cb-163">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ee4cb-163">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee4cb-164">例</span><span class="sxs-lookup"><span data-stu-id="ee4cb-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee4cb-165">要求</span><span class="sxs-lookup"><span data-stu-id="ee4cb-165">Request</span></span>
<span data-ttu-id="ee4cb-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ee4cb-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="ee4cb-167">応答</span><span class="sxs-lookup"><span data-stu-id="ee4cb-167">Response</span></span>
<span data-ttu-id="ee4cb-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ee4cb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






