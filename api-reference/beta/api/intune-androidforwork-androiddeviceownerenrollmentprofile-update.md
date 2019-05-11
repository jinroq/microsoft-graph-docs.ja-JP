---
title: AndroidDeviceOwnerEnrollmentProfile の更新
description: AndroidDeviceOwnerEnrollmentProfile オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 691058b863533703d0d69760659c91305f8c4180
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939148"
---
# <a name="update-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="cc792-103">AndroidDeviceOwnerEnrollmentProfile の更新</span><span class="sxs-lookup"><span data-stu-id="cc792-103">Update androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="cc792-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc792-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc792-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cc792-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc792-106">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cc792-106">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc792-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="cc792-107">Prerequisites</span></span>
<span data-ttu-id="cc792-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc792-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc792-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc792-110">Permission type</span></span>|<span data-ttu-id="cc792-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc792-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc792-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc792-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cc792-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc792-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cc792-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc792-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc792-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc792-115">Not supported.</span></span>|
|<span data-ttu-id="cc792-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc792-116">Application</span></span>|<span data-ttu-id="cc792-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc792-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc792-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc792-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="cc792-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc792-119">Request headers</span></span>
|<span data-ttu-id="cc792-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc792-120">Header</span></span>|<span data-ttu-id="cc792-121">値</span><span class="sxs-lookup"><span data-stu-id="cc792-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc792-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc792-122">Authorization</span></span>|<span data-ttu-id="cc792-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="cc792-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc792-124">承諾</span><span class="sxs-lookup"><span data-stu-id="cc792-124">Accept</span></span>|<span data-ttu-id="cc792-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cc792-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc792-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc792-126">Request body</span></span>
<span data-ttu-id="cc792-127">要求本文で、 [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cc792-127">In the request body, supply a JSON representation for the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

<span data-ttu-id="cc792-128">次の表に、 [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cc792-128">The following table shows the properties that are required when you create the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>

|<span data-ttu-id="cc792-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc792-129">Property</span></span>|<span data-ttu-id="cc792-130">型</span><span class="sxs-lookup"><span data-stu-id="cc792-130">Type</span></span>|<span data-ttu-id="cc792-131">説明</span><span class="sxs-lookup"><span data-stu-id="cc792-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc792-132">accountId</span><span class="sxs-lookup"><span data-stu-id="cc792-132">accountId</span></span>|<span data-ttu-id="cc792-133">String</span><span class="sxs-lookup"><span data-stu-id="cc792-133">String</span></span>|<span data-ttu-id="cc792-134">登録プロファイルが属するテナント GUID。</span><span class="sxs-lookup"><span data-stu-id="cc792-134">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="cc792-135">id</span><span class="sxs-lookup"><span data-stu-id="cc792-135">id</span></span>|<span data-ttu-id="cc792-136">文字列</span><span class="sxs-lookup"><span data-stu-id="cc792-136">String</span></span>|<span data-ttu-id="cc792-137">登録プロファイルの一意の GUID。</span><span class="sxs-lookup"><span data-stu-id="cc792-137">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="cc792-138">displayName</span><span class="sxs-lookup"><span data-stu-id="cc792-138">displayName</span></span>|<span data-ttu-id="cc792-139">String</span><span class="sxs-lookup"><span data-stu-id="cc792-139">String</span></span>|<span data-ttu-id="cc792-140">登録プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="cc792-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="cc792-141">description</span><span class="sxs-lookup"><span data-stu-id="cc792-141">description</span></span>|<span data-ttu-id="cc792-142">String</span><span class="sxs-lookup"><span data-stu-id="cc792-142">String</span></span>|<span data-ttu-id="cc792-143">登録プロファイルの説明。</span><span class="sxs-lookup"><span data-stu-id="cc792-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="cc792-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc792-144">createdDateTime</span></span>|<span data-ttu-id="cc792-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc792-145">DateTimeOffset</span></span>|<span data-ttu-id="cc792-146">登録プロファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="cc792-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="cc792-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc792-147">lastModifiedDateTime</span></span>|<span data-ttu-id="cc792-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc792-148">DateTimeOffset</span></span>|<span data-ttu-id="cc792-149">登録プロファイルが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="cc792-149">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="cc792-150">tokenValue</span><span class="sxs-lookup"><span data-stu-id="cc792-150">tokenValue</span></span>|<span data-ttu-id="cc792-151">String</span><span class="sxs-lookup"><span data-stu-id="cc792-151">String</span></span>|<span data-ttu-id="cc792-152">この登録プロファイル用に最後に作成されたトークンの値。</span><span class="sxs-lookup"><span data-stu-id="cc792-152">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="cc792-153">Tokenの日付/時刻</span><span class="sxs-lookup"><span data-stu-id="cc792-153">tokenCreationDateTime</span></span>|<span data-ttu-id="cc792-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc792-154">DateTimeOffset</span></span>|<span data-ttu-id="cc792-155">最後に作成されたトークンが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="cc792-155">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="cc792-156">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cc792-156">tokenExpirationDateTime</span></span>|<span data-ttu-id="cc792-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc792-157">DateTimeOffset</span></span>|<span data-ttu-id="cc792-158">最後に作成されたトークンの有効期限が切れる日時。</span><span class="sxs-lookup"><span data-stu-id="cc792-158">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="cc792-159">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cc792-159">enrolledDeviceCount</span></span>|<span data-ttu-id="cc792-160">Int32</span><span class="sxs-lookup"><span data-stu-id="cc792-160">Int32</span></span>|<span data-ttu-id="cc792-161">この登録プロファイルを使用して登録した Android デバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="cc792-161">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="cc792-162">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="cc792-162">qrCodeContent</span></span>|<span data-ttu-id="cc792-163">String</span><span class="sxs-lookup"><span data-stu-id="cc792-163">String</span></span>|<span data-ttu-id="cc792-164">トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="cc792-164">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="cc792-165">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="cc792-165">qrCodeImage</span></span>|[<span data-ttu-id="cc792-166">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cc792-166">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cc792-167">トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="cc792-167">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="cc792-168">応答</span><span class="sxs-lookup"><span data-stu-id="cc792-168">Response</span></span>
<span data-ttu-id="cc792-169">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cc792-169">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc792-170">例</span><span class="sxs-lookup"><span data-stu-id="cc792-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc792-171">要求</span><span class="sxs-lookup"><span data-stu-id="cc792-171">Request</span></span>
<span data-ttu-id="cc792-172">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cc792-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cc792-173">応答</span><span class="sxs-lookup"><span data-stu-id="cc792-173">Response</span></span>
<span data-ttu-id="cc792-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cc792-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




