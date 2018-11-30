---
title: applePushNotificationCertificate の更新
description: applePushNotificationCertificate オブジェクトのプロパティを更新します。
ms.openlocfilehash: 640fae8367813682f890ee41e11614c44d933412
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022486"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="1c726-103">applePushNotificationCertificate の更新</span><span class="sxs-lookup"><span data-stu-id="1c726-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="1c726-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1c726-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c726-105">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1c726-105">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1c726-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="1c726-106">Prerequisites</span></span>
<span data-ttu-id="1c726-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c726-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c726-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1c726-109">Permission type</span></span>|<span data-ttu-id="1c726-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1c726-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c726-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1c726-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1c726-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c726-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1c726-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1c726-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c726-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c726-114">Not supported.</span></span>|
|<span data-ttu-id="1c726-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1c726-115">Application</span></span>|<span data-ttu-id="1c726-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c726-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c726-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1c726-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="1c726-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c726-118">Request headers</span></span>
|<span data-ttu-id="1c726-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c726-119">Header</span></span>|<span data-ttu-id="1c726-120">値</span><span class="sxs-lookup"><span data-stu-id="1c726-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c726-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c726-121">Authorization</span></span>|<span data-ttu-id="1c726-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1c726-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c726-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1c726-123">Accept</span></span>|<span data-ttu-id="1c726-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1c726-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c726-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1c726-125">Request body</span></span>
<span data-ttu-id="1c726-126">要求本文で、[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1c726-126">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="1c726-127">次の表に、[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1c726-127">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="1c726-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c726-128">Property</span></span>|<span data-ttu-id="1c726-129">型</span><span class="sxs-lookup"><span data-stu-id="1c726-129">Type</span></span>|<span data-ttu-id="1c726-130">説明</span><span class="sxs-lookup"><span data-stu-id="1c726-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c726-131">id</span><span class="sxs-lookup"><span data-stu-id="1c726-131">id</span></span>|<span data-ttu-id="1c726-132">String</span><span class="sxs-lookup"><span data-stu-id="1c726-132">String</span></span>|<span data-ttu-id="1c726-133">証明書の一意識別子</span><span class="sxs-lookup"><span data-stu-id="1c726-133">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="1c726-134">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="1c726-134">appleIdentifier</span></span>|<span data-ttu-id="1c726-135">String</span><span class="sxs-lookup"><span data-stu-id="1c726-135">String</span></span>|<span data-ttu-id="1c726-136">MDM プッシュ証明書の作成に使用するアカウントの Apple ID。</span><span class="sxs-lookup"><span data-stu-id="1c726-136">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="1c726-137">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="1c726-137">topicIdentifier</span></span>|<span data-ttu-id="1c726-138">String</span><span class="sxs-lookup"><span data-stu-id="1c726-138">String</span></span>|<span data-ttu-id="1c726-139">トピック ID。</span><span class="sxs-lookup"><span data-stu-id="1c726-139">Topic Id.</span></span>|
|<span data-ttu-id="1c726-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c726-140">lastModifiedDateTime</span></span>|<span data-ttu-id="1c726-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c726-141">DateTimeOffset</span></span>|<span data-ttu-id="1c726-142">Apple プッシュ通知証明書の最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="1c726-142">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="1c726-143">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1c726-143">expirationDateTime</span></span>|<span data-ttu-id="1c726-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c726-144">DateTimeOffset</span></span>|<span data-ttu-id="1c726-145">Apple プッシュ通知証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="1c726-145">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="1c726-146">証明書</span><span class="sxs-lookup"><span data-stu-id="1c726-146">certificate</span></span>|<span data-ttu-id="1c726-147">String</span><span class="sxs-lookup"><span data-stu-id="1c726-147">String</span></span>|<span data-ttu-id="1c726-148">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1c726-148">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1c726-149">応答</span><span class="sxs-lookup"><span data-stu-id="1c726-149">Response</span></span>
<span data-ttu-id="1c726-150">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1c726-150">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c726-151">例</span><span class="sxs-lookup"><span data-stu-id="1c726-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="1c726-152">要求</span><span class="sxs-lookup"><span data-stu-id="1c726-152">Request</span></span>
<span data-ttu-id="1c726-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1c726-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="1c726-154">応答</span><span class="sxs-lookup"><span data-stu-id="1c726-154">Response</span></span>
<span data-ttu-id="1c726-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1c726-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 384

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```


