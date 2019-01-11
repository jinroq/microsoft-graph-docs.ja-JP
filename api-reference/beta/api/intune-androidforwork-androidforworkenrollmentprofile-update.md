---
title: androidForWorkEnrollmentProfile の更新
description: androidForWorkEnrollmentProfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a9f7f98e8fc1192ce80ce054f6699690189905b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824046"
---
# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="0422a-103">androidForWorkEnrollmentProfile の更新</span><span class="sxs-lookup"><span data-stu-id="0422a-103">Update androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="0422a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0422a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0422a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0422a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0422a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0422a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0422a-107">[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0422a-107">Update the properties of a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0422a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0422a-108">Prerequisites</span></span>
<span data-ttu-id="0422a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0422a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0422a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0422a-111">Permission type</span></span>|<span data-ttu-id="0422a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0422a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0422a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0422a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0422a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0422a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0422a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0422a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0422a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0422a-116">Not supported.</span></span>|
|<span data-ttu-id="0422a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0422a-117">Application</span></span>|<span data-ttu-id="0422a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0422a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0422a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0422a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="0422a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0422a-120">Request headers</span></span>
|<span data-ttu-id="0422a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0422a-121">Header</span></span>|<span data-ttu-id="0422a-122">値</span><span class="sxs-lookup"><span data-stu-id="0422a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0422a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0422a-123">Authorization</span></span>|<span data-ttu-id="0422a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0422a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0422a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0422a-125">Accept</span></span>|<span data-ttu-id="0422a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0422a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0422a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0422a-127">Request body</span></span>
<span data-ttu-id="0422a-128">要求本文で、[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0422a-128">In the request body, supply a JSON representation for the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="0422a-129">次の表に、[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0422a-129">The following table shows the properties that are required when you create the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span></span>

|<span data-ttu-id="0422a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0422a-130">Property</span></span>|<span data-ttu-id="0422a-131">種類</span><span class="sxs-lookup"><span data-stu-id="0422a-131">Type</span></span>|<span data-ttu-id="0422a-132">説明</span><span class="sxs-lookup"><span data-stu-id="0422a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0422a-133">accountId</span><span class="sxs-lookup"><span data-stu-id="0422a-133">accountId</span></span>|<span data-ttu-id="0422a-134">String</span><span class="sxs-lookup"><span data-stu-id="0422a-134">String</span></span>|<span data-ttu-id="0422a-135">登録プロファイルが属するテナント GUID。</span><span class="sxs-lookup"><span data-stu-id="0422a-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="0422a-136">id</span><span class="sxs-lookup"><span data-stu-id="0422a-136">id</span></span>|<span data-ttu-id="0422a-137">String</span><span class="sxs-lookup"><span data-stu-id="0422a-137">String</span></span>|<span data-ttu-id="0422a-138">登録プロファイル用の一意な GUID。</span><span class="sxs-lookup"><span data-stu-id="0422a-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="0422a-139">displayName</span><span class="sxs-lookup"><span data-stu-id="0422a-139">displayName</span></span>|<span data-ttu-id="0422a-140">String</span><span class="sxs-lookup"><span data-stu-id="0422a-140">String</span></span>|<span data-ttu-id="0422a-141">登録プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="0422a-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="0422a-142">説明</span><span class="sxs-lookup"><span data-stu-id="0422a-142">description</span></span>|<span data-ttu-id="0422a-143">String</span><span class="sxs-lookup"><span data-stu-id="0422a-143">String</span></span>|<span data-ttu-id="0422a-144">登録プロファイルの説明。</span><span class="sxs-lookup"><span data-stu-id="0422a-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="0422a-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0422a-145">createdDateTime</span></span>|<span data-ttu-id="0422a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0422a-146">DateTimeOffset</span></span>|<span data-ttu-id="0422a-147">登録プロファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="0422a-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="0422a-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0422a-148">lastModifiedDateTime</span></span>|<span data-ttu-id="0422a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0422a-149">DateTimeOffset</span></span>|<span data-ttu-id="0422a-150">登録プロファイルが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="0422a-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="0422a-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="0422a-151">tokenValue</span></span>|<span data-ttu-id="0422a-152">String</span><span class="sxs-lookup"><span data-stu-id="0422a-152">String</span></span>|<span data-ttu-id="0422a-153">この登録プロファイル用に最後に作成されたトークンの値。</span><span class="sxs-lookup"><span data-stu-id="0422a-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="0422a-154">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0422a-154">tokenExpirationDateTime</span></span>|<span data-ttu-id="0422a-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0422a-155">DateTimeOffset</span></span>|<span data-ttu-id="0422a-156">最後に作成されたトークンの有効期限が切れる日時。</span><span class="sxs-lookup"><span data-stu-id="0422a-156">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="0422a-157">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0422a-157">enrolledDeviceCount</span></span>|<span data-ttu-id="0422a-158">Int32</span><span class="sxs-lookup"><span data-stu-id="0422a-158">Int32</span></span>|<span data-ttu-id="0422a-159">この登録プロファイルを使用して登録した Android デバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="0422a-159">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="0422a-160">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="0422a-160">qrCodeContent</span></span>|<span data-ttu-id="0422a-161">String</span><span class="sxs-lookup"><span data-stu-id="0422a-161">String</span></span>|<span data-ttu-id="0422a-162">トークン用の QR コードを生成するために使用された文字列。</span><span class="sxs-lookup"><span data-stu-id="0422a-162">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="0422a-163">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="0422a-163">qrCodeImage</span></span>|[<span data-ttu-id="0422a-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0422a-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0422a-165">トークン用の QR コードを生成するために使用された文字列。</span><span class="sxs-lookup"><span data-stu-id="0422a-165">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="0422a-166">応答</span><span class="sxs-lookup"><span data-stu-id="0422a-166">Response</span></span>
<span data-ttu-id="0422a-167">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0422a-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0422a-168">例</span><span class="sxs-lookup"><span data-stu-id="0422a-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="0422a-169">要求</span><span class="sxs-lookup"><span data-stu-id="0422a-169">Request</span></span>
<span data-ttu-id="0422a-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0422a-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
Content-type: application/json
Content-length: 490

{
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
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

### <a name="response"></a><span data-ttu-id="0422a-171">応答</span><span class="sxs-lookup"><span data-stu-id="0422a-171">Response</span></span>
<span data-ttu-id="0422a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0422a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 668

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "e6742553-2553-e674-5325-74e6532574e6",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
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





