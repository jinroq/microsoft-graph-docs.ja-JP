---
title: applePushNotificationCertificate の更新
description: applePushNotificationCertificate オブジェクトのプロパティを更新します。
ms.openlocfilehash: 7fbb7db93290fb6f455bdcca3053c6f3affb1375
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068767"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="34e9e-103">applePushNotificationCertificate の更新</span><span class="sxs-lookup"><span data-stu-id="34e9e-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="34e9e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="34e9e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34e9e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34e9e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34e9e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="34e9e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34e9e-107">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="34e9e-107">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="34e9e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="34e9e-108">Prerequisites</span></span>
<span data-ttu-id="34e9e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34e9e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34e9e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="34e9e-111">Permission type</span></span>|<span data-ttu-id="34e9e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="34e9e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34e9e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="34e9e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34e9e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34e9e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="34e9e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="34e9e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34e9e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34e9e-116">Not supported.</span></span>|
|<span data-ttu-id="34e9e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="34e9e-117">Application</span></span>|<span data-ttu-id="34e9e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34e9e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34e9e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="34e9e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="34e9e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="34e9e-120">Request headers</span></span>
|<span data-ttu-id="34e9e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="34e9e-121">Header</span></span>|<span data-ttu-id="34e9e-122">値</span><span class="sxs-lookup"><span data-stu-id="34e9e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34e9e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="34e9e-123">Authorization</span></span>|<span data-ttu-id="34e9e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="34e9e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34e9e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="34e9e-125">Accept</span></span>|<span data-ttu-id="34e9e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="34e9e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34e9e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="34e9e-127">Request body</span></span>
<span data-ttu-id="34e9e-128">要求本文で、[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="34e9e-128">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="34e9e-129">次の表に、[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="34e9e-129">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="34e9e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34e9e-130">Property</span></span>|<span data-ttu-id="34e9e-131">型</span><span class="sxs-lookup"><span data-stu-id="34e9e-131">Type</span></span>|<span data-ttu-id="34e9e-132">説明</span><span class="sxs-lookup"><span data-stu-id="34e9e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34e9e-133">id</span><span class="sxs-lookup"><span data-stu-id="34e9e-133">id</span></span>|<span data-ttu-id="34e9e-134">String</span><span class="sxs-lookup"><span data-stu-id="34e9e-134">String</span></span>|<span data-ttu-id="34e9e-135">証明書の一意識別子</span><span class="sxs-lookup"><span data-stu-id="34e9e-135">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="34e9e-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="34e9e-136">appleIdentifier</span></span>|<span data-ttu-id="34e9e-137">String</span><span class="sxs-lookup"><span data-stu-id="34e9e-137">String</span></span>|<span data-ttu-id="34e9e-138">MDM プッシュ証明書の作成に使用するアカウントの Apple ID。</span><span class="sxs-lookup"><span data-stu-id="34e9e-138">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="34e9e-139">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="34e9e-139">topicIdentifier</span></span>|<span data-ttu-id="34e9e-140">String</span><span class="sxs-lookup"><span data-stu-id="34e9e-140">String</span></span>|<span data-ttu-id="34e9e-141">トピック ID。</span><span class="sxs-lookup"><span data-stu-id="34e9e-141">Topic Id.</span></span>|
|<span data-ttu-id="34e9e-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34e9e-142">lastModifiedDateTime</span></span>|<span data-ttu-id="34e9e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34e9e-143">DateTimeOffset</span></span>|<span data-ttu-id="34e9e-144">Apple プッシュ通知証明書の最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="34e9e-144">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="34e9e-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="34e9e-145">expirationDateTime</span></span>|<span data-ttu-id="34e9e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34e9e-146">DateTimeOffset</span></span>|<span data-ttu-id="34e9e-147">Apple プッシュ通知証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="34e9e-147">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="34e9e-148">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="34e9e-148">certificateUploadStatus</span></span>|<span data-ttu-id="34e9e-149">String</span><span class="sxs-lookup"><span data-stu-id="34e9e-149">String</span></span>|<span data-ttu-id="34e9e-150">証明書のアップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="34e9e-150">The certificate upload status.</span></span>|
|<span data-ttu-id="34e9e-151">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="34e9e-151">certificateUploadFailureReason</span></span>|<span data-ttu-id="34e9e-152">String</span><span class="sxs-lookup"><span data-stu-id="34e9e-152">String</span></span>|<span data-ttu-id="34e9e-153">理由の証明書のアップロードに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="34e9e-153">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="34e9e-154">証明書</span><span class="sxs-lookup"><span data-stu-id="34e9e-154">certificate</span></span>|<span data-ttu-id="34e9e-155">String</span><span class="sxs-lookup"><span data-stu-id="34e9e-155">String</span></span>|<span data-ttu-id="34e9e-156">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="34e9e-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="34e9e-157">応答</span><span class="sxs-lookup"><span data-stu-id="34e9e-157">Response</span></span>
<span data-ttu-id="34e9e-158">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="34e9e-158">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34e9e-159">例</span><span class="sxs-lookup"><span data-stu-id="34e9e-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="34e9e-160">要求</span><span class="sxs-lookup"><span data-stu-id="34e9e-160">Request</span></span>
<span data-ttu-id="34e9e-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="34e9e-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 409

{
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="34e9e-162">応答</span><span class="sxs-lookup"><span data-stu-id="34e9e-162">Response</span></span>
<span data-ttu-id="34e9e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="34e9e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificate": "Certificate value"
}
```





