---
title: ImportedDeviceIdentityResult を作成する
description: 新しい importedDeviceIdentityResult オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c4482ca743f4f6cada865ca53d34e9333f0597bb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356362"
---
# <a name="create-importeddeviceidentityresult"></a><span data-ttu-id="31870-103">ImportedDeviceIdentityResult を作成する</span><span class="sxs-lookup"><span data-stu-id="31870-103">Create importedDeviceIdentityResult</span></span>

> <span data-ttu-id="31870-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31870-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31870-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="31870-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31870-106">新しい[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="31870-106">Create a new [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31870-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="31870-107">Prerequisites</span></span>
<span data-ttu-id="31870-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31870-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31870-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="31870-110">Permission type</span></span>|<span data-ttu-id="31870-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="31870-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31870-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="31870-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31870-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31870-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="31870-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="31870-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31870-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31870-115">Not supported.</span></span>|
|<span data-ttu-id="31870-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="31870-116">Application</span></span>|<span data-ttu-id="31870-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31870-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31870-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="31870-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="31870-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31870-119">Request headers</span></span>
|<span data-ttu-id="31870-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31870-120">Header</span></span>|<span data-ttu-id="31870-121">値</span><span class="sxs-lookup"><span data-stu-id="31870-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31870-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="31870-122">Authorization</span></span>|<span data-ttu-id="31870-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="31870-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31870-124">承諾</span><span class="sxs-lookup"><span data-stu-id="31870-124">Accept</span></span>|<span data-ttu-id="31870-125">application/json</span><span class="sxs-lookup"><span data-stu-id="31870-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31870-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="31870-126">Request body</span></span>
<span data-ttu-id="31870-127">要求本文で、importedDeviceIdentityResult オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="31870-127">In the request body, supply a JSON representation for the importedDeviceIdentityResult object.</span></span>

<span data-ttu-id="31870-128">次の表に、importedDeviceIdentityResult の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="31870-128">The following table shows the properties that are required when you create the importedDeviceIdentityResult.</span></span>

|<span data-ttu-id="31870-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31870-129">Property</span></span>|<span data-ttu-id="31870-130">型</span><span class="sxs-lookup"><span data-stu-id="31870-130">Type</span></span>|<span data-ttu-id="31870-131">説明</span><span class="sxs-lookup"><span data-stu-id="31870-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31870-132">id</span><span class="sxs-lookup"><span data-stu-id="31870-132">id</span></span>|<span data-ttu-id="31870-133">String</span><span class="sxs-lookup"><span data-stu-id="31870-133">String</span></span>|<span data-ttu-id="31870-134">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された、インポートされたデバイス id の id</span><span class="sxs-lookup"><span data-stu-id="31870-134">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="31870-135">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="31870-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="31870-136">String</span><span class="sxs-lookup"><span data-stu-id="31870-136">String</span></span>|<span data-ttu-id="31870-137">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された、インポートされたデバイス識別子</span><span class="sxs-lookup"><span data-stu-id="31870-137">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="31870-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="31870-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="31870-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="31870-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="31870-140">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された、インポートされたデバイス id の種類。</span><span class="sxs-lookup"><span data-stu-id="31870-140">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="31870-141">可能な値は、`unknown`、`imei`、`serialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="31870-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="31870-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31870-142">lastModifiedDateTime</span></span>|<span data-ttu-id="31870-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31870-143">DateTimeOffset</span></span>|<span data-ttu-id="31870-144">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された説明の最終更新日時。</span><span class="sxs-lookup"><span data-stu-id="31870-144">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="31870-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31870-145">createdDateTime</span></span>|<span data-ttu-id="31870-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31870-146">DateTimeOffset</span></span>|<span data-ttu-id="31870-147">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されたデバイスの日時の作成日時</span><span class="sxs-lookup"><span data-stu-id="31870-147">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="31870-148">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="31870-148">lastContactedDateTime</span></span>|<span data-ttu-id="31870-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31870-149">DateTimeOffset</span></span>|<span data-ttu-id="31870-150">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されたデバイスの最後の連絡日時。</span><span class="sxs-lookup"><span data-stu-id="31870-150">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="31870-151">description</span><span class="sxs-lookup"><span data-stu-id="31870-151">description</span></span>|<span data-ttu-id="31870-152">String</span><span class="sxs-lookup"><span data-stu-id="31870-152">String</span></span>|<span data-ttu-id="31870-153">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されたデバイスの説明</span><span class="sxs-lookup"><span data-stu-id="31870-153">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="31870-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="31870-154">enrollmentState</span></span>|[<span data-ttu-id="31870-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="31870-155">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="31870-156">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された Intune のデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="31870-156">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="31870-157">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="31870-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="31870-158">platform</span><span class="sxs-lookup"><span data-stu-id="31870-158">platform</span></span>|[<span data-ttu-id="31870-159">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="31870-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="31870-160">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="31870-160">The platform of the Device.</span></span> <span data-ttu-id="31870-161">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="31870-161">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="31870-162">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="31870-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="31870-163">status</span><span class="sxs-lookup"><span data-stu-id="31870-163">status</span></span>|<span data-ttu-id="31870-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="31870-164">Boolean</span></span>|<span data-ttu-id="31870-165">インポートされたデバイス id の状態</span><span class="sxs-lookup"><span data-stu-id="31870-165">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="31870-166">応答</span><span class="sxs-lookup"><span data-stu-id="31870-166">Response</span></span>
<span data-ttu-id="31870-167">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="31870-167">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31870-168">例</span><span class="sxs-lookup"><span data-stu-id="31870-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="31870-169">要求</span><span class="sxs-lookup"><span data-stu-id="31870-169">Request</span></span>
<span data-ttu-id="31870-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="31870-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
Content-type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a><span data-ttu-id="31870-171">応答</span><span class="sxs-lookup"><span data-stu-id="31870-171">Response</span></span>
<span data-ttu-id="31870-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="31870-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```






