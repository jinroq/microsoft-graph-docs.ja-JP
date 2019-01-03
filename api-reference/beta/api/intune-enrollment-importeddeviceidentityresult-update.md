---
title: ImportedDeviceIdentityResult を更新します。
description: ImportedDeviceIdentityResult オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 4c698810bb3fe88f52d8fcba11d8c29aeb508fe6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332439"
---
# <a name="update-importeddeviceidentityresult"></a><span data-ttu-id="917b5-103">ImportedDeviceIdentityResult を更新します。</span><span class="sxs-lookup"><span data-stu-id="917b5-103">Update importedDeviceIdentityResult</span></span>

> <span data-ttu-id="917b5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="917b5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="917b5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="917b5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="917b5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="917b5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="917b5-107">[ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="917b5-107">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="917b5-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="917b5-108">Prerequisites</span></span>
<span data-ttu-id="917b5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="917b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="917b5-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="917b5-111">Permission type</span></span>|<span data-ttu-id="917b5-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="917b5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="917b5-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="917b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="917b5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="917b5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="917b5-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="917b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="917b5-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="917b5-116">Not supported.</span></span>|
|<span data-ttu-id="917b5-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="917b5-117">Application</span></span>|<span data-ttu-id="917b5-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="917b5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="917b5-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="917b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="917b5-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="917b5-120">Request headers</span></span>
|<span data-ttu-id="917b5-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="917b5-121">Header</span></span>|<span data-ttu-id="917b5-122">値</span><span class="sxs-lookup"><span data-stu-id="917b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="917b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="917b5-123">Authorization</span></span>|<span data-ttu-id="917b5-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="917b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="917b5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="917b5-125">Accept</span></span>|<span data-ttu-id="917b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="917b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="917b5-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="917b5-127">Request body</span></span>
<span data-ttu-id="917b5-128">要求の本文に[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="917b5-128">In the request body, supply a JSON representation for the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

<span data-ttu-id="917b5-129">[ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="917b5-129">The following table shows the properties that are required when you create the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>

|<span data-ttu-id="917b5-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="917b5-130">Property</span></span>|<span data-ttu-id="917b5-131">種類</span><span class="sxs-lookup"><span data-stu-id="917b5-131">Type</span></span>|<span data-ttu-id="917b5-132">説明</span><span class="sxs-lookup"><span data-stu-id="917b5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="917b5-133">ID</span><span class="sxs-lookup"><span data-stu-id="917b5-133">id</span></span>|<span data-ttu-id="917b5-134">String</span><span class="sxs-lookup"><span data-stu-id="917b5-134">String</span></span>|<span data-ttu-id="917b5-135">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されるインポート済みのデバイス id の id</span><span class="sxs-lookup"><span data-stu-id="917b5-135">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="917b5-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="917b5-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="917b5-137">String</span><span class="sxs-lookup"><span data-stu-id="917b5-137">String</span></span>|<span data-ttu-id="917b5-138">インポートされたデバイスの識別子から継承された[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="917b5-138">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="917b5-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="917b5-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="917b5-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="917b5-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="917b5-141">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)からインポートされたデバイスの Id を継承の種類。</span><span class="sxs-lookup"><span data-stu-id="917b5-141">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="917b5-142">可能な値は、`unknown`、`imei`、`serialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="917b5-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="917b5-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="917b5-143">lastModifiedDateTime</span></span>|<span data-ttu-id="917b5-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="917b5-144">DateTimeOffset</span></span>|<span data-ttu-id="917b5-145">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承する」の説明の最後の変更日時</span><span class="sxs-lookup"><span data-stu-id="917b5-145">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="917b5-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="917b5-146">createdDateTime</span></span>|<span data-ttu-id="917b5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="917b5-147">DateTimeOffset</span></span>|<span data-ttu-id="917b5-148">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承される、デバイスの日時を作成</span><span class="sxs-lookup"><span data-stu-id="917b5-148">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="917b5-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="917b5-149">lastContactedDateTime</span></span>|<span data-ttu-id="917b5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="917b5-150">DateTimeOffset</span></span>|<span data-ttu-id="917b5-151">最終接続日時[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されるデバイスの</span><span class="sxs-lookup"><span data-stu-id="917b5-151">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="917b5-152">説明</span><span class="sxs-lookup"><span data-stu-id="917b5-152">description</span></span>|<span data-ttu-id="917b5-153">String</span><span class="sxs-lookup"><span data-stu-id="917b5-153">String</span></span>|<span data-ttu-id="917b5-154">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承される、デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="917b5-154">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="917b5-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="917b5-155">enrollmentState</span></span>|[<span data-ttu-id="917b5-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="917b5-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="917b5-157">Intune 継承で[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)からのデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="917b5-157">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="917b5-158">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="917b5-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="917b5-159">platform</span><span class="sxs-lookup"><span data-stu-id="917b5-159">platform</span></span>|[<span data-ttu-id="917b5-160">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="917b5-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="917b5-161">デバイスのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="917b5-161">The platform of the Device.</span></span> <span data-ttu-id="917b5-162">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="917b5-162">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="917b5-163">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="917b5-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="917b5-164">status</span><span class="sxs-lookup"><span data-stu-id="917b5-164">status</span></span>|<span data-ttu-id="917b5-165">ブール型</span><span class="sxs-lookup"><span data-stu-id="917b5-165">Boolean</span></span>|<span data-ttu-id="917b5-166">インポートされたデバイス id のステータス</span><span class="sxs-lookup"><span data-stu-id="917b5-166">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="917b5-167">応答</span><span class="sxs-lookup"><span data-stu-id="917b5-167">Response</span></span>
<span data-ttu-id="917b5-168">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="917b5-168">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="917b5-169">例</span><span class="sxs-lookup"><span data-stu-id="917b5-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="917b5-170">要求</span><span class="sxs-lookup"><span data-stu-id="917b5-170">Request</span></span>
<span data-ttu-id="917b5-171">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="917b5-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
Content-type: application/json
Content-length: 354

{
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a><span data-ttu-id="917b5-172">応答</span><span class="sxs-lookup"><span data-stu-id="917b5-172">Response</span></span>
<span data-ttu-id="917b5-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="917b5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




