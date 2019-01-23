---
title: AndroidDeviceOwnerEnrollmentProfile を更新します。
description: AndroidDeviceOwnerEnrollmentProfile オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 966b538b161dca2bc5c85390cab5cd8bd371b236
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413830"
---
# <a name="update-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="75eaf-103">AndroidDeviceOwnerEnrollmentProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="75eaf-103">Update androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="75eaf-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="75eaf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="75eaf-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75eaf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="75eaf-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="75eaf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75eaf-107">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="75eaf-107">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75eaf-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="75eaf-108">Prerequisites</span></span>
<span data-ttu-id="75eaf-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75eaf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="75eaf-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="75eaf-111">Permission type</span></span>|<span data-ttu-id="75eaf-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="75eaf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75eaf-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="75eaf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75eaf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75eaf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75eaf-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="75eaf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75eaf-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75eaf-116">Not supported.</span></span>|
|<span data-ttu-id="75eaf-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="75eaf-117">Application</span></span>|<span data-ttu-id="75eaf-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75eaf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75eaf-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="75eaf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="75eaf-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75eaf-120">Request headers</span></span>
|<span data-ttu-id="75eaf-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75eaf-121">Header</span></span>|<span data-ttu-id="75eaf-122">値</span><span class="sxs-lookup"><span data-stu-id="75eaf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75eaf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="75eaf-123">Authorization</span></span>|<span data-ttu-id="75eaf-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="75eaf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75eaf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="75eaf-125">Accept</span></span>|<span data-ttu-id="75eaf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75eaf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75eaf-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="75eaf-127">Request body</span></span>
<span data-ttu-id="75eaf-128">要求の本文に[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="75eaf-128">In the request body, supply a JSON representation for the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

<span data-ttu-id="75eaf-129">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="75eaf-129">The following table shows the properties that are required when you create the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>

|<span data-ttu-id="75eaf-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75eaf-130">Property</span></span>|<span data-ttu-id="75eaf-131">型</span><span class="sxs-lookup"><span data-stu-id="75eaf-131">Type</span></span>|<span data-ttu-id="75eaf-132">説明</span><span class="sxs-lookup"><span data-stu-id="75eaf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75eaf-133">accountId</span><span class="sxs-lookup"><span data-stu-id="75eaf-133">accountId</span></span>|<span data-ttu-id="75eaf-134">String</span><span class="sxs-lookup"><span data-stu-id="75eaf-134">String</span></span>|<span data-ttu-id="75eaf-135">登録プロファイルが属するテナント GUID。</span><span class="sxs-lookup"><span data-stu-id="75eaf-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="75eaf-136">id</span><span class="sxs-lookup"><span data-stu-id="75eaf-136">id</span></span>|<span data-ttu-id="75eaf-137">String</span><span class="sxs-lookup"><span data-stu-id="75eaf-137">String</span></span>|<span data-ttu-id="75eaf-138">登録プロファイル用の一意な GUID。</span><span class="sxs-lookup"><span data-stu-id="75eaf-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="75eaf-139">displayName</span><span class="sxs-lookup"><span data-stu-id="75eaf-139">displayName</span></span>|<span data-ttu-id="75eaf-140">String</span><span class="sxs-lookup"><span data-stu-id="75eaf-140">String</span></span>|<span data-ttu-id="75eaf-141">登録プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="75eaf-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="75eaf-142">説明</span><span class="sxs-lookup"><span data-stu-id="75eaf-142">description</span></span>|<span data-ttu-id="75eaf-143">String</span><span class="sxs-lookup"><span data-stu-id="75eaf-143">String</span></span>|<span data-ttu-id="75eaf-144">登録プロファイルの説明。</span><span class="sxs-lookup"><span data-stu-id="75eaf-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="75eaf-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75eaf-145">createdDateTime</span></span>|<span data-ttu-id="75eaf-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75eaf-146">DateTimeOffset</span></span>|<span data-ttu-id="75eaf-147">登録プロファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="75eaf-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="75eaf-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75eaf-148">lastModifiedDateTime</span></span>|<span data-ttu-id="75eaf-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75eaf-149">DateTimeOffset</span></span>|<span data-ttu-id="75eaf-150">登録プロファイルが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="75eaf-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="75eaf-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="75eaf-151">tokenValue</span></span>|<span data-ttu-id="75eaf-152">String</span><span class="sxs-lookup"><span data-stu-id="75eaf-152">String</span></span>|<span data-ttu-id="75eaf-153">この登録プロファイル用に最後に作成されたトークンの値。</span><span class="sxs-lookup"><span data-stu-id="75eaf-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="75eaf-154">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="75eaf-154">tokenCreationDateTime</span></span>|<span data-ttu-id="75eaf-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75eaf-155">DateTimeOffset</span></span>|<span data-ttu-id="75eaf-156">直前に作成されたトークンが作成された日時です。</span><span class="sxs-lookup"><span data-stu-id="75eaf-156">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="75eaf-157">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="75eaf-157">tokenExpirationDateTime</span></span>|<span data-ttu-id="75eaf-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75eaf-158">DateTimeOffset</span></span>|<span data-ttu-id="75eaf-159">最後に作成されたトークンの有効期限が切れる日時。</span><span class="sxs-lookup"><span data-stu-id="75eaf-159">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="75eaf-160">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75eaf-160">enrolledDeviceCount</span></span>|<span data-ttu-id="75eaf-161">Int32</span><span class="sxs-lookup"><span data-stu-id="75eaf-161">Int32</span></span>|<span data-ttu-id="75eaf-162">この登録プロファイルを使用して登録した Android デバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="75eaf-162">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="75eaf-163">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="75eaf-163">qrCodeContent</span></span>|<span data-ttu-id="75eaf-164">String</span><span class="sxs-lookup"><span data-stu-id="75eaf-164">String</span></span>|<span data-ttu-id="75eaf-165">トークン用の QR コードを生成するために使用された文字列。</span><span class="sxs-lookup"><span data-stu-id="75eaf-165">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="75eaf-166">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="75eaf-166">qrCodeImage</span></span>|[<span data-ttu-id="75eaf-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="75eaf-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="75eaf-168">トークン用の QR コードを生成するために使用された文字列。</span><span class="sxs-lookup"><span data-stu-id="75eaf-168">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="75eaf-169">応答</span><span class="sxs-lookup"><span data-stu-id="75eaf-169">Response</span></span>
<span data-ttu-id="75eaf-170">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="75eaf-170">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75eaf-171">例</span><span class="sxs-lookup"><span data-stu-id="75eaf-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="75eaf-172">要求</span><span class="sxs-lookup"><span data-stu-id="75eaf-172">Request</span></span>
<span data-ttu-id="75eaf-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="75eaf-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
Content-type: application/json
Content-length: 565

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "tokenValue": "Token Value value",
  "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a><span data-ttu-id="75eaf-174">応答</span><span class="sxs-lookup"><span data-stu-id="75eaf-174">Response</span></span>
<span data-ttu-id="75eaf-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="75eaf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 737

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```




