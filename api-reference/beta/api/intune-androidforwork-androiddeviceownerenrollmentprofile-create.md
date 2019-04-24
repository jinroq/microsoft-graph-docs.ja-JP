---
title: androidDeviceOwnerEnrollmentProfile を作成する
description: 新しい androidDeviceOwnerEnrollmentProfile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7589c0842a30068035a1c423339d5df22e5fc1cb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32500322"
---
# <a name="create-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="85c1f-103">androidDeviceOwnerEnrollmentProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="85c1f-103">Create androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="85c1f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85c1f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85c1f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="85c1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85c1f-106">新しい[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="85c1f-106">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85c1f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="85c1f-107">Prerequisites</span></span>
<span data-ttu-id="85c1f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="85c1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85c1f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="85c1f-110">Permission type</span></span>|<span data-ttu-id="85c1f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="85c1f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85c1f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="85c1f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="85c1f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85c1f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="85c1f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="85c1f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85c1f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85c1f-115">Not supported.</span></span>|
|<span data-ttu-id="85c1f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="85c1f-116">Application</span></span>|<span data-ttu-id="85c1f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85c1f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85c1f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="85c1f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="85c1f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85c1f-119">Request headers</span></span>
|<span data-ttu-id="85c1f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85c1f-120">Header</span></span>|<span data-ttu-id="85c1f-121">値</span><span class="sxs-lookup"><span data-stu-id="85c1f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85c1f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="85c1f-122">Authorization</span></span>|<span data-ttu-id="85c1f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="85c1f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85c1f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="85c1f-124">Accept</span></span>|<span data-ttu-id="85c1f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="85c1f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85c1f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="85c1f-126">Request body</span></span>
<span data-ttu-id="85c1f-127">要求本文で、androidDeviceOwnerEnrollmentProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="85c1f-127">In the request body, supply a JSON representation for the androidDeviceOwnerEnrollmentProfile object.</span></span>

<span data-ttu-id="85c1f-128">次の表に、androidDeviceOwnerEnrollmentProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="85c1f-128">The following table shows the properties that are required when you create the androidDeviceOwnerEnrollmentProfile.</span></span>

|<span data-ttu-id="85c1f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85c1f-129">Property</span></span>|<span data-ttu-id="85c1f-130">型</span><span class="sxs-lookup"><span data-stu-id="85c1f-130">Type</span></span>|<span data-ttu-id="85c1f-131">説明</span><span class="sxs-lookup"><span data-stu-id="85c1f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85c1f-132">accountId</span><span class="sxs-lookup"><span data-stu-id="85c1f-132">accountId</span></span>|<span data-ttu-id="85c1f-133">String</span><span class="sxs-lookup"><span data-stu-id="85c1f-133">String</span></span>|<span data-ttu-id="85c1f-134">登録プロファイルが属するテナント GUID。</span><span class="sxs-lookup"><span data-stu-id="85c1f-134">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="85c1f-135">id</span><span class="sxs-lookup"><span data-stu-id="85c1f-135">id</span></span>|<span data-ttu-id="85c1f-136">String</span><span class="sxs-lookup"><span data-stu-id="85c1f-136">String</span></span>|<span data-ttu-id="85c1f-137">登録プロファイルの一意の GUID。</span><span class="sxs-lookup"><span data-stu-id="85c1f-137">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="85c1f-138">displayName</span><span class="sxs-lookup"><span data-stu-id="85c1f-138">displayName</span></span>|<span data-ttu-id="85c1f-139">String</span><span class="sxs-lookup"><span data-stu-id="85c1f-139">String</span></span>|<span data-ttu-id="85c1f-140">登録プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="85c1f-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="85c1f-141">説明</span><span class="sxs-lookup"><span data-stu-id="85c1f-141">description</span></span>|<span data-ttu-id="85c1f-142">String</span><span class="sxs-lookup"><span data-stu-id="85c1f-142">String</span></span>|<span data-ttu-id="85c1f-143">登録プロファイルの説明。</span><span class="sxs-lookup"><span data-stu-id="85c1f-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="85c1f-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85c1f-144">createdDateTime</span></span>|<span data-ttu-id="85c1f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85c1f-145">DateTimeOffset</span></span>|<span data-ttu-id="85c1f-146">登録プロファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="85c1f-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="85c1f-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85c1f-147">lastModifiedDateTime</span></span>|<span data-ttu-id="85c1f-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85c1f-148">DateTimeOffset</span></span>|<span data-ttu-id="85c1f-149">登録プロファイルが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="85c1f-149">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="85c1f-150">tokenValue</span><span class="sxs-lookup"><span data-stu-id="85c1f-150">tokenValue</span></span>|<span data-ttu-id="85c1f-151">String</span><span class="sxs-lookup"><span data-stu-id="85c1f-151">String</span></span>|<span data-ttu-id="85c1f-152">この登録プロファイル用に最後に作成されたトークンの値。</span><span class="sxs-lookup"><span data-stu-id="85c1f-152">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="85c1f-153">tokenの日付/時刻</span><span class="sxs-lookup"><span data-stu-id="85c1f-153">tokenCreationDateTime</span></span>|<span data-ttu-id="85c1f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85c1f-154">DateTimeOffset</span></span>|<span data-ttu-id="85c1f-155">最後に作成されたトークンが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="85c1f-155">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="85c1f-156">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="85c1f-156">tokenExpirationDateTime</span></span>|<span data-ttu-id="85c1f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85c1f-157">DateTimeOffset</span></span>|<span data-ttu-id="85c1f-158">最後に作成されたトークンの有効期限が切れる日時。</span><span class="sxs-lookup"><span data-stu-id="85c1f-158">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="85c1f-159">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="85c1f-159">enrolledDeviceCount</span></span>|<span data-ttu-id="85c1f-160">Int32</span><span class="sxs-lookup"><span data-stu-id="85c1f-160">Int32</span></span>|<span data-ttu-id="85c1f-161">この登録プロファイルを使用して登録した Android デバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="85c1f-161">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="85c1f-162">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="85c1f-162">qrCodeContent</span></span>|<span data-ttu-id="85c1f-163">String</span><span class="sxs-lookup"><span data-stu-id="85c1f-163">String</span></span>|<span data-ttu-id="85c1f-164">トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="85c1f-164">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="85c1f-165">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="85c1f-165">qrCodeImage</span></span>|[<span data-ttu-id="85c1f-166">mimeContent</span><span class="sxs-lookup"><span data-stu-id="85c1f-166">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="85c1f-167">トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="85c1f-167">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="85c1f-168">応答</span><span class="sxs-lookup"><span data-stu-id="85c1f-168">Response</span></span>
<span data-ttu-id="85c1f-169">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="85c1f-169">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85c1f-170">例</span><span class="sxs-lookup"><span data-stu-id="85c1f-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="85c1f-171">要求</span><span class="sxs-lookup"><span data-stu-id="85c1f-171">Request</span></span>
<span data-ttu-id="85c1f-172">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="85c1f-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="85c1f-173">応答</span><span class="sxs-lookup"><span data-stu-id="85c1f-173">Response</span></span>
<span data-ttu-id="85c1f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="85c1f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





