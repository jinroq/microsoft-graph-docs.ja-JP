---
title: ImportedDeviceIdentity を更新します。
description: ImportedDeviceIdentity オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a66ceb575363f8a48dd0d23e61a6ecbc994ea582
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973490"
---
# <a name="update-importeddeviceidentity"></a><span data-ttu-id="973ef-103">ImportedDeviceIdentity を更新します。</span><span class="sxs-lookup"><span data-stu-id="973ef-103">Update importedDeviceIdentity</span></span>

> <span data-ttu-id="973ef-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="973ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="973ef-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="973ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="973ef-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="973ef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="973ef-107">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="973ef-107">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="973ef-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="973ef-108">Prerequisites</span></span>
<span data-ttu-id="973ef-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="973ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="973ef-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="973ef-111">Permission type</span></span>|<span data-ttu-id="973ef-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="973ef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="973ef-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="973ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="973ef-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="973ef-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="973ef-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="973ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="973ef-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="973ef-116">Not supported.</span></span>|
|<span data-ttu-id="973ef-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="973ef-117">Application</span></span>|<span data-ttu-id="973ef-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="973ef-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="973ef-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="973ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="973ef-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="973ef-120">Request headers</span></span>
|<span data-ttu-id="973ef-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="973ef-121">Header</span></span>|<span data-ttu-id="973ef-122">値</span><span class="sxs-lookup"><span data-stu-id="973ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="973ef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="973ef-123">Authorization</span></span>|<span data-ttu-id="973ef-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="973ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="973ef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="973ef-125">Accept</span></span>|<span data-ttu-id="973ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="973ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="973ef-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="973ef-127">Request body</span></span>
<span data-ttu-id="973ef-128">要求の本文に[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="973ef-128">In the request body, supply a JSON representation for the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

<span data-ttu-id="973ef-129">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="973ef-129">The following table shows the properties that are required when you create the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>

|<span data-ttu-id="973ef-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="973ef-130">Property</span></span>|<span data-ttu-id="973ef-131">型</span><span class="sxs-lookup"><span data-stu-id="973ef-131">Type</span></span>|<span data-ttu-id="973ef-132">説明</span><span class="sxs-lookup"><span data-stu-id="973ef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="973ef-133">ID</span><span class="sxs-lookup"><span data-stu-id="973ef-133">id</span></span>|<span data-ttu-id="973ef-134">String</span><span class="sxs-lookup"><span data-stu-id="973ef-134">String</span></span>|<span data-ttu-id="973ef-135">インポートされたデバイス id の id</span><span class="sxs-lookup"><span data-stu-id="973ef-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="973ef-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="973ef-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="973ef-137">String</span><span class="sxs-lookup"><span data-stu-id="973ef-137">String</span></span>|<span data-ttu-id="973ef-138">インポートされたデバイスの識別子</span><span class="sxs-lookup"><span data-stu-id="973ef-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="973ef-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="973ef-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="973ef-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="973ef-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="973ef-141">インポートされたデバイスの識別情報の種類です。</span><span class="sxs-lookup"><span data-stu-id="973ef-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="973ef-142">可能な値は、`unknown`、`imei`、`serialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="973ef-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="973ef-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="973ef-143">lastModifiedDateTime</span></span>|<span data-ttu-id="973ef-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="973ef-144">DateTimeOffset</span></span>|<span data-ttu-id="973ef-145">説明の最後の変更日時</span><span class="sxs-lookup"><span data-stu-id="973ef-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="973ef-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="973ef-146">createdDateTime</span></span>|<span data-ttu-id="973ef-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="973ef-147">DateTimeOffset</span></span>|<span data-ttu-id="973ef-148">デバイスの作成日時</span><span class="sxs-lookup"><span data-stu-id="973ef-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="973ef-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="973ef-149">lastContactedDateTime</span></span>|<span data-ttu-id="973ef-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="973ef-150">DateTimeOffset</span></span>|<span data-ttu-id="973ef-151">最終アクセス日時、デバイスの</span><span class="sxs-lookup"><span data-stu-id="973ef-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="973ef-152">説明</span><span class="sxs-lookup"><span data-stu-id="973ef-152">description</span></span>|<span data-ttu-id="973ef-153">String</span><span class="sxs-lookup"><span data-stu-id="973ef-153">String</span></span>|<span data-ttu-id="973ef-154">デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="973ef-154">The description of the device</span></span>|
|<span data-ttu-id="973ef-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="973ef-155">enrollmentState</span></span>|[<span data-ttu-id="973ef-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="973ef-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="973ef-157">Intune でデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="973ef-157">The state of the device in Intune.</span></span> <span data-ttu-id="973ef-158">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="973ef-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="973ef-159">platform</span><span class="sxs-lookup"><span data-stu-id="973ef-159">platform</span></span>|[<span data-ttu-id="973ef-160">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="973ef-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="973ef-161">デバイスのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="973ef-161">The platform of the Device.</span></span> <span data-ttu-id="973ef-162">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="973ef-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="973ef-163">応答</span><span class="sxs-lookup"><span data-stu-id="973ef-163">Response</span></span>
<span data-ttu-id="973ef-164">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="973ef-164">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="973ef-165">例</span><span class="sxs-lookup"><span data-stu-id="973ef-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="973ef-166">要求</span><span class="sxs-lookup"><span data-stu-id="973ef-166">Request</span></span>
<span data-ttu-id="973ef-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="973ef-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
Content-type: application/json
Content-length: 335

{
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="973ef-168">応答</span><span class="sxs-lookup"><span data-stu-id="973ef-168">Response</span></span>
<span data-ttu-id="973ef-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="973ef-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





