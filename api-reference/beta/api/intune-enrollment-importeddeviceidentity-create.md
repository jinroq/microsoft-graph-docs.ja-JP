---
title: ImportedDeviceIdentity を作成します。
description: 新しい importedDeviceIdentity オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d0274f3a48c3481cc5540eb9025da353f0ea0bf2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396715"
---
# <a name="create-importeddeviceidentity"></a><span data-ttu-id="7f710-103">ImportedDeviceIdentity を作成します。</span><span class="sxs-lookup"><span data-stu-id="7f710-103">Create importedDeviceIdentity</span></span>

> <span data-ttu-id="7f710-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7f710-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7f710-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f710-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f710-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f710-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f710-107">新しい[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7f710-107">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f710-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7f710-108">Prerequisites</span></span>
<span data-ttu-id="7f710-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f710-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7f710-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f710-111">Permission type</span></span>|<span data-ttu-id="7f710-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f710-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f710-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f710-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f710-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f710-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7f710-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f710-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f710-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f710-116">Not supported.</span></span>|
|<span data-ttu-id="7f710-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f710-117">Application</span></span>|<span data-ttu-id="7f710-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f710-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f710-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f710-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="7f710-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f710-120">Request headers</span></span>
|<span data-ttu-id="7f710-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f710-121">Header</span></span>|<span data-ttu-id="7f710-122">値</span><span class="sxs-lookup"><span data-stu-id="7f710-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f710-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f710-123">Authorization</span></span>|<span data-ttu-id="7f710-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7f710-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f710-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7f710-125">Accept</span></span>|<span data-ttu-id="7f710-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f710-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f710-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f710-127">Request body</span></span>
<span data-ttu-id="7f710-128">要求の本文に importedDeviceIdentity オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f710-128">In the request body, supply a JSON representation for the importedDeviceIdentity object.</span></span>

<span data-ttu-id="7f710-129">次の表は、importedDeviceIdentity を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7f710-129">The following table shows the properties that are required when you create the importedDeviceIdentity.</span></span>

|<span data-ttu-id="7f710-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f710-130">Property</span></span>|<span data-ttu-id="7f710-131">型</span><span class="sxs-lookup"><span data-stu-id="7f710-131">Type</span></span>|<span data-ttu-id="7f710-132">説明</span><span class="sxs-lookup"><span data-stu-id="7f710-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f710-133">id</span><span class="sxs-lookup"><span data-stu-id="7f710-133">id</span></span>|<span data-ttu-id="7f710-134">String</span><span class="sxs-lookup"><span data-stu-id="7f710-134">String</span></span>|<span data-ttu-id="7f710-135">インポートされたデバイス id の id</span><span class="sxs-lookup"><span data-stu-id="7f710-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="7f710-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="7f710-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="7f710-137">String</span><span class="sxs-lookup"><span data-stu-id="7f710-137">String</span></span>|<span data-ttu-id="7f710-138">インポートされたデバイスの識別子</span><span class="sxs-lookup"><span data-stu-id="7f710-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="7f710-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="7f710-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="7f710-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="7f710-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="7f710-141">インポートされたデバイスの識別情報の種類です。</span><span class="sxs-lookup"><span data-stu-id="7f710-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="7f710-142">可能な値は、`unknown`、`imei`、`serialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="7f710-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="7f710-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f710-143">lastModifiedDateTime</span></span>|<span data-ttu-id="7f710-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f710-144">DateTimeOffset</span></span>|<span data-ttu-id="7f710-145">説明の最後の変更日時</span><span class="sxs-lookup"><span data-stu-id="7f710-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="7f710-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f710-146">createdDateTime</span></span>|<span data-ttu-id="7f710-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f710-147">DateTimeOffset</span></span>|<span data-ttu-id="7f710-148">デバイスの作成日時</span><span class="sxs-lookup"><span data-stu-id="7f710-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="7f710-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f710-149">lastContactedDateTime</span></span>|<span data-ttu-id="7f710-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f710-150">DateTimeOffset</span></span>|<span data-ttu-id="7f710-151">最終アクセス日時、デバイスの</span><span class="sxs-lookup"><span data-stu-id="7f710-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="7f710-152">説明</span><span class="sxs-lookup"><span data-stu-id="7f710-152">description</span></span>|<span data-ttu-id="7f710-153">String</span><span class="sxs-lookup"><span data-stu-id="7f710-153">String</span></span>|<span data-ttu-id="7f710-154">デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="7f710-154">The description of the device</span></span>|
|<span data-ttu-id="7f710-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="7f710-155">enrollmentState</span></span>|[<span data-ttu-id="7f710-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="7f710-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="7f710-157">Intune でデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="7f710-157">The state of the device in Intune.</span></span> <span data-ttu-id="7f710-158">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="7f710-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="7f710-159">platform</span><span class="sxs-lookup"><span data-stu-id="7f710-159">platform</span></span>|[<span data-ttu-id="7f710-160">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="7f710-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="7f710-161">デバイスのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="7f710-161">The platform of the Device.</span></span> <span data-ttu-id="7f710-162">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="7f710-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="7f710-163">応答</span><span class="sxs-lookup"><span data-stu-id="7f710-163">Response</span></span>
<span data-ttu-id="7f710-164">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7f710-164">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f710-165">例</span><span class="sxs-lookup"><span data-stu-id="7f710-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f710-166">要求</span><span class="sxs-lookup"><span data-stu-id="7f710-166">Request</span></span>
<span data-ttu-id="7f710-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7f710-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7f710-168">応答</span><span class="sxs-lookup"><span data-stu-id="7f710-168">Response</span></span>
<span data-ttu-id="7f710-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7f710-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




