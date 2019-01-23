---
title: ImportedDeviceIdentityResult を作成します。
description: 新しい importedDeviceIdentityResult オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 05f3880d005d78463c3225b0eef501dba5e21299
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416273"
---
# <a name="create-importeddeviceidentityresult"></a><span data-ttu-id="7d0f9-103">ImportedDeviceIdentityResult を作成します。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-103">Create importedDeviceIdentityResult</span></span>

> <span data-ttu-id="7d0f9-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7d0f9-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d0f9-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d0f9-107">新しい[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-107">Create a new [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d0f9-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7d0f9-108">Prerequisites</span></span>
<span data-ttu-id="7d0f9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7d0f9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d0f9-111">Permission type</span></span>|<span data-ttu-id="7d0f9-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d0f9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d0f9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d0f9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d0f9-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d0f9-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7d0f9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d0f9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d0f9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-116">Not supported.</span></span>|
|<span data-ttu-id="7d0f9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d0f9-117">Application</span></span>|<span data-ttu-id="7d0f9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d0f9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d0f9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="7d0f9-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d0f9-120">Request headers</span></span>
|<span data-ttu-id="7d0f9-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d0f9-121">Header</span></span>|<span data-ttu-id="7d0f9-122">値</span><span class="sxs-lookup"><span data-stu-id="7d0f9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d0f9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d0f9-123">Authorization</span></span>|<span data-ttu-id="7d0f9-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d0f9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7d0f9-125">Accept</span></span>|<span data-ttu-id="7d0f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d0f9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d0f9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7d0f9-127">Request body</span></span>
<span data-ttu-id="7d0f9-128">要求の本文に importedDeviceIdentityResult オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-128">In the request body, supply a JSON representation for the importedDeviceIdentityResult object.</span></span>

<span data-ttu-id="7d0f9-129">次の表は、importedDeviceIdentityResult を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-129">The following table shows the properties that are required when you create the importedDeviceIdentityResult.</span></span>

|<span data-ttu-id="7d0f9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d0f9-130">Property</span></span>|<span data-ttu-id="7d0f9-131">型</span><span class="sxs-lookup"><span data-stu-id="7d0f9-131">Type</span></span>|<span data-ttu-id="7d0f9-132">説明</span><span class="sxs-lookup"><span data-stu-id="7d0f9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d0f9-133">id</span><span class="sxs-lookup"><span data-stu-id="7d0f9-133">id</span></span>|<span data-ttu-id="7d0f9-134">String</span><span class="sxs-lookup"><span data-stu-id="7d0f9-134">String</span></span>|<span data-ttu-id="7d0f9-135">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されるインポート済みのデバイス id の id</span><span class="sxs-lookup"><span data-stu-id="7d0f9-135">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="7d0f9-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="7d0f9-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="7d0f9-137">String</span><span class="sxs-lookup"><span data-stu-id="7d0f9-137">String</span></span>|<span data-ttu-id="7d0f9-138">インポートされたデバイスの識別子から継承された[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="7d0f9-138">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="7d0f9-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="7d0f9-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="7d0f9-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="7d0f9-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="7d0f9-141">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)からインポートされたデバイスの Id を継承の種類。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-141">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="7d0f9-142">可能な値は、`unknown`、`imei`、`serialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="7d0f9-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d0f9-143">lastModifiedDateTime</span></span>|<span data-ttu-id="7d0f9-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d0f9-144">DateTimeOffset</span></span>|<span data-ttu-id="7d0f9-145">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承する」の説明の最後の変更日時</span><span class="sxs-lookup"><span data-stu-id="7d0f9-145">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="7d0f9-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d0f9-146">createdDateTime</span></span>|<span data-ttu-id="7d0f9-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d0f9-147">DateTimeOffset</span></span>|<span data-ttu-id="7d0f9-148">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承される、デバイスの日時を作成</span><span class="sxs-lookup"><span data-stu-id="7d0f9-148">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="7d0f9-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d0f9-149">lastContactedDateTime</span></span>|<span data-ttu-id="7d0f9-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d0f9-150">DateTimeOffset</span></span>|<span data-ttu-id="7d0f9-151">最終接続日時[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されるデバイスの</span><span class="sxs-lookup"><span data-stu-id="7d0f9-151">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="7d0f9-152">説明</span><span class="sxs-lookup"><span data-stu-id="7d0f9-152">description</span></span>|<span data-ttu-id="7d0f9-153">String</span><span class="sxs-lookup"><span data-stu-id="7d0f9-153">String</span></span>|<span data-ttu-id="7d0f9-154">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承される、デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="7d0f9-154">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="7d0f9-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="7d0f9-155">enrollmentState</span></span>|[<span data-ttu-id="7d0f9-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="7d0f9-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="7d0f9-157">Intune 継承で[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)からのデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-157">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="7d0f9-158">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="7d0f9-159">platform</span><span class="sxs-lookup"><span data-stu-id="7d0f9-159">platform</span></span>|[<span data-ttu-id="7d0f9-160">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="7d0f9-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="7d0f9-161">デバイスのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-161">The platform of the Device.</span></span> <span data-ttu-id="7d0f9-162">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-162">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="7d0f9-163">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="7d0f9-164">status</span><span class="sxs-lookup"><span data-stu-id="7d0f9-164">status</span></span>|<span data-ttu-id="7d0f9-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d0f9-165">Boolean</span></span>|<span data-ttu-id="7d0f9-166">インポートされたデバイス id のステータス</span><span class="sxs-lookup"><span data-stu-id="7d0f9-166">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="7d0f9-167">応答</span><span class="sxs-lookup"><span data-stu-id="7d0f9-167">Response</span></span>
<span data-ttu-id="7d0f9-168">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-168">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d0f9-169">例</span><span class="sxs-lookup"><span data-stu-id="7d0f9-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d0f9-170">要求</span><span class="sxs-lookup"><span data-stu-id="7d0f9-170">Request</span></span>
<span data-ttu-id="7d0f9-171">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7d0f9-172">応答</span><span class="sxs-lookup"><span data-stu-id="7d0f9-172">Response</span></span>
<span data-ttu-id="7d0f9-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7d0f9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




