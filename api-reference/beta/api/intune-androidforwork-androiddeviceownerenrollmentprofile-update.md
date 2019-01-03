---
title: AndroidDeviceOwnerEnrollmentProfile を更新します。
description: AndroidDeviceOwnerEnrollmentProfile オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 136b11dd16023b3394d5c5cf084123acbef93c6d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361881"
---
# <a name="update-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="75b99-103">AndroidDeviceOwnerEnrollmentProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="75b99-103">Update androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="75b99-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="75b99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75b99-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75b99-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="75b99-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="75b99-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75b99-107">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="75b99-107">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="75b99-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="75b99-108">Prerequisites</span></span>
<span data-ttu-id="75b99-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75b99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75b99-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="75b99-111">Permission type</span></span>|<span data-ttu-id="75b99-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="75b99-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75b99-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="75b99-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75b99-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75b99-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75b99-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="75b99-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75b99-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75b99-116">Not supported.</span></span>|
|<span data-ttu-id="75b99-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="75b99-117">Application</span></span>|<span data-ttu-id="75b99-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75b99-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75b99-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="75b99-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="75b99-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75b99-120">Request headers</span></span>
|<span data-ttu-id="75b99-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75b99-121">Header</span></span>|<span data-ttu-id="75b99-122">値</span><span class="sxs-lookup"><span data-stu-id="75b99-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75b99-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="75b99-123">Authorization</span></span>|<span data-ttu-id="75b99-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="75b99-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75b99-125">Accept</span><span class="sxs-lookup"><span data-stu-id="75b99-125">Accept</span></span>|<span data-ttu-id="75b99-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75b99-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75b99-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="75b99-127">Request body</span></span>
<span data-ttu-id="75b99-128">要求の本文に[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="75b99-128">In the request body, supply a JSON representation for the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

<span data-ttu-id="75b99-129">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="75b99-129">The following table shows the properties that are required when you create the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>

|<span data-ttu-id="75b99-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75b99-130">Property</span></span>|<span data-ttu-id="75b99-131">種類</span><span class="sxs-lookup"><span data-stu-id="75b99-131">Type</span></span>|<span data-ttu-id="75b99-132">説明</span><span class="sxs-lookup"><span data-stu-id="75b99-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75b99-133">accountId</span><span class="sxs-lookup"><span data-stu-id="75b99-133">accountId</span></span>|<span data-ttu-id="75b99-134">String</span><span class="sxs-lookup"><span data-stu-id="75b99-134">String</span></span>|<span data-ttu-id="75b99-135">登録プロファイルが属するテナント GUID。</span><span class="sxs-lookup"><span data-stu-id="75b99-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="75b99-136">id</span><span class="sxs-lookup"><span data-stu-id="75b99-136">id</span></span>|<span data-ttu-id="75b99-137">String</span><span class="sxs-lookup"><span data-stu-id="75b99-137">String</span></span>|<span data-ttu-id="75b99-138">登録プロファイル用の一意な GUID。</span><span class="sxs-lookup"><span data-stu-id="75b99-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="75b99-139">displayName</span><span class="sxs-lookup"><span data-stu-id="75b99-139">displayName</span></span>|<span data-ttu-id="75b99-140">String</span><span class="sxs-lookup"><span data-stu-id="75b99-140">String</span></span>|<span data-ttu-id="75b99-141">登録プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="75b99-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="75b99-142">説明</span><span class="sxs-lookup"><span data-stu-id="75b99-142">description</span></span>|<span data-ttu-id="75b99-143">String</span><span class="sxs-lookup"><span data-stu-id="75b99-143">String</span></span>|<span data-ttu-id="75b99-144">登録プロファイルの説明。</span><span class="sxs-lookup"><span data-stu-id="75b99-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="75b99-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75b99-145">createdDateTime</span></span>|<span data-ttu-id="75b99-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75b99-146">DateTimeOffset</span></span>|<span data-ttu-id="75b99-147">登録プロファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="75b99-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="75b99-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75b99-148">lastModifiedDateTime</span></span>|<span data-ttu-id="75b99-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75b99-149">DateTimeOffset</span></span>|<span data-ttu-id="75b99-150">登録プロファイルが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="75b99-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="75b99-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="75b99-151">tokenValue</span></span>|<span data-ttu-id="75b99-152">String</span><span class="sxs-lookup"><span data-stu-id="75b99-152">String</span></span>|<span data-ttu-id="75b99-153">この登録プロファイル用に最後に作成されたトークンの値。</span><span class="sxs-lookup"><span data-stu-id="75b99-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="75b99-154">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="75b99-154">tokenCreationDateTime</span></span>|<span data-ttu-id="75b99-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75b99-155">DateTimeOffset</span></span>|<span data-ttu-id="75b99-156">直前に作成されたトークンが作成された日時です。</span><span class="sxs-lookup"><span data-stu-id="75b99-156">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="75b99-157">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="75b99-157">tokenExpirationDateTime</span></span>|<span data-ttu-id="75b99-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75b99-158">DateTimeOffset</span></span>|<span data-ttu-id="75b99-159">最後に作成されたトークンの有効期限が切れる日時。</span><span class="sxs-lookup"><span data-stu-id="75b99-159">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="75b99-160">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75b99-160">enrolledDeviceCount</span></span>|<span data-ttu-id="75b99-161">Int32</span><span class="sxs-lookup"><span data-stu-id="75b99-161">Int32</span></span>|<span data-ttu-id="75b99-162">この登録プロファイルを使用して登録した Android デバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="75b99-162">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="75b99-163">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="75b99-163">qrCodeContent</span></span>|<span data-ttu-id="75b99-164">String</span><span class="sxs-lookup"><span data-stu-id="75b99-164">String</span></span>|<span data-ttu-id="75b99-165">トークン用の QR コードを生成するために使用された文字列。</span><span class="sxs-lookup"><span data-stu-id="75b99-165">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="75b99-166">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="75b99-166">qrCodeImage</span></span>|[<span data-ttu-id="75b99-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="75b99-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="75b99-168">トークン用の QR コードを生成するために使用された文字列。</span><span class="sxs-lookup"><span data-stu-id="75b99-168">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="75b99-169">応答</span><span class="sxs-lookup"><span data-stu-id="75b99-169">Response</span></span>
<span data-ttu-id="75b99-170">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="75b99-170">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75b99-171">例</span><span class="sxs-lookup"><span data-stu-id="75b99-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="75b99-172">要求</span><span class="sxs-lookup"><span data-stu-id="75b99-172">Request</span></span>
<span data-ttu-id="75b99-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="75b99-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
Content-type: application/json
Content-length: 555

{
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="75b99-174">応答</span><span class="sxs-lookup"><span data-stu-id="75b99-174">Response</span></span>
<span data-ttu-id="75b99-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="75b99-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




