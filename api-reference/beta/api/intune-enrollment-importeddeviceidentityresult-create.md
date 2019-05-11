---
title: ImportedDeviceIdentityResult を作成する
description: 新しい importedDeviceIdentityResult オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd9253c0f37be07c2a38461fb1fdfdb961e0fc06
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908330"
---
# <a name="create-importeddeviceidentityresult"></a><span data-ttu-id="86dc8-103">ImportedDeviceIdentityResult を作成する</span><span class="sxs-lookup"><span data-stu-id="86dc8-103">Create importedDeviceIdentityResult</span></span>

> <span data-ttu-id="86dc8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86dc8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86dc8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="86dc8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86dc8-106">新しい[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="86dc8-106">Create a new [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86dc8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="86dc8-107">Prerequisites</span></span>
<span data-ttu-id="86dc8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86dc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86dc8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="86dc8-110">Permission type</span></span>|<span data-ttu-id="86dc8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="86dc8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86dc8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="86dc8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86dc8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86dc8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="86dc8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="86dc8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86dc8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86dc8-115">Not supported.</span></span>|
|<span data-ttu-id="86dc8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="86dc8-116">Application</span></span>|<span data-ttu-id="86dc8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86dc8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86dc8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="86dc8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="86dc8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86dc8-119">Request headers</span></span>
|<span data-ttu-id="86dc8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86dc8-120">Header</span></span>|<span data-ttu-id="86dc8-121">値</span><span class="sxs-lookup"><span data-stu-id="86dc8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86dc8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="86dc8-122">Authorization</span></span>|<span data-ttu-id="86dc8-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="86dc8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86dc8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="86dc8-124">Accept</span></span>|<span data-ttu-id="86dc8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86dc8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86dc8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="86dc8-126">Request body</span></span>
<span data-ttu-id="86dc8-127">要求本文で、importedDeviceIdentityResult オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="86dc8-127">In the request body, supply a JSON representation for the importedDeviceIdentityResult object.</span></span>

<span data-ttu-id="86dc8-128">次の表に、importedDeviceIdentityResult の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="86dc8-128">The following table shows the properties that are required when you create the importedDeviceIdentityResult.</span></span>

|<span data-ttu-id="86dc8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86dc8-129">Property</span></span>|<span data-ttu-id="86dc8-130">型</span><span class="sxs-lookup"><span data-stu-id="86dc8-130">Type</span></span>|<span data-ttu-id="86dc8-131">説明</span><span class="sxs-lookup"><span data-stu-id="86dc8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86dc8-132">id</span><span class="sxs-lookup"><span data-stu-id="86dc8-132">id</span></span>|<span data-ttu-id="86dc8-133">String</span><span class="sxs-lookup"><span data-stu-id="86dc8-133">String</span></span>|<span data-ttu-id="86dc8-134">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された、インポートされたデバイス Id の id</span><span class="sxs-lookup"><span data-stu-id="86dc8-134">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="86dc8-135">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="86dc8-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="86dc8-136">String</span><span class="sxs-lookup"><span data-stu-id="86dc8-136">String</span></span>|<span data-ttu-id="86dc8-137">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された、インポートされたデバイス識別子</span><span class="sxs-lookup"><span data-stu-id="86dc8-137">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="86dc8-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="86dc8-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="86dc8-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="86dc8-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="86dc8-140">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された、インポートされたデバイス Id の種類。</span><span class="sxs-lookup"><span data-stu-id="86dc8-140">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="86dc8-141">可能な値は、`unknown`、`imei`、`serialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="86dc8-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="86dc8-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86dc8-142">lastModifiedDateTime</span></span>|<span data-ttu-id="86dc8-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86dc8-143">DateTimeOffset</span></span>|<span data-ttu-id="86dc8-144">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された説明の最終更新日時。</span><span class="sxs-lookup"><span data-stu-id="86dc8-144">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="86dc8-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86dc8-145">createdDateTime</span></span>|<span data-ttu-id="86dc8-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86dc8-146">DateTimeOffset</span></span>|<span data-ttu-id="86dc8-147">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されたデバイスの日時の作成日時</span><span class="sxs-lookup"><span data-stu-id="86dc8-147">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="86dc8-148">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="86dc8-148">lastContactedDateTime</span></span>|<span data-ttu-id="86dc8-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86dc8-149">DateTimeOffset</span></span>|<span data-ttu-id="86dc8-150">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されたデバイスの最後の連絡日時。</span><span class="sxs-lookup"><span data-stu-id="86dc8-150">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="86dc8-151">description</span><span class="sxs-lookup"><span data-stu-id="86dc8-151">description</span></span>|<span data-ttu-id="86dc8-152">String</span><span class="sxs-lookup"><span data-stu-id="86dc8-152">String</span></span>|<span data-ttu-id="86dc8-153">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されたデバイスの説明</span><span class="sxs-lookup"><span data-stu-id="86dc8-153">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="86dc8-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="86dc8-154">enrollmentState</span></span>|[<span data-ttu-id="86dc8-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="86dc8-155">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="86dc8-156">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された Intune のデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="86dc8-156">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="86dc8-157">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="86dc8-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="86dc8-158">platform</span><span class="sxs-lookup"><span data-stu-id="86dc8-158">platform</span></span>|[<span data-ttu-id="86dc8-159">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="86dc8-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="86dc8-160">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="86dc8-160">The platform of the Device.</span></span> <span data-ttu-id="86dc8-161">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="86dc8-161">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="86dc8-162">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="86dc8-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="86dc8-163">status</span><span class="sxs-lookup"><span data-stu-id="86dc8-163">status</span></span>|<span data-ttu-id="86dc8-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="86dc8-164">Boolean</span></span>|<span data-ttu-id="86dc8-165">インポートされたデバイス id の状態</span><span class="sxs-lookup"><span data-stu-id="86dc8-165">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="86dc8-166">応答</span><span class="sxs-lookup"><span data-stu-id="86dc8-166">Response</span></span>
<span data-ttu-id="86dc8-167">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="86dc8-167">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86dc8-168">例</span><span class="sxs-lookup"><span data-stu-id="86dc8-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="86dc8-169">要求</span><span class="sxs-lookup"><span data-stu-id="86dc8-169">Request</span></span>
<span data-ttu-id="86dc8-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="86dc8-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="86dc8-171">応答</span><span class="sxs-lookup"><span data-stu-id="86dc8-171">Response</span></span>
<span data-ttu-id="86dc8-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="86dc8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




