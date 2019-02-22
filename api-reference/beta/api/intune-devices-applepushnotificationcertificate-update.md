---
title: applePushNotificationCertificate の更新
description: applePushNotificationCertificate オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee760b38c8f684c0ca7f0c8bcca0c98d8a87d931
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172045"
---
# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="d6c05-103">applePushNotificationCertificate の更新</span><span class="sxs-lookup"><span data-stu-id="d6c05-103">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="d6c05-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6c05-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6c05-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d6c05-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6c05-106">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d6c05-106">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6c05-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d6c05-107">Prerequisites</span></span>
<span data-ttu-id="d6c05-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6c05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d6c05-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d6c05-110">Permission type</span></span>|<span data-ttu-id="d6c05-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d6c05-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6c05-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d6c05-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d6c05-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6c05-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d6c05-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d6c05-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6c05-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6c05-115">Not supported.</span></span>|
|<span data-ttu-id="d6c05-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d6c05-116">Application</span></span>|<span data-ttu-id="d6c05-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6c05-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6c05-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d6c05-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="d6c05-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6c05-119">Request headers</span></span>
|<span data-ttu-id="d6c05-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6c05-120">Header</span></span>|<span data-ttu-id="d6c05-121">値</span><span class="sxs-lookup"><span data-stu-id="d6c05-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6c05-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6c05-122">Authorization</span></span>|<span data-ttu-id="d6c05-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d6c05-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6c05-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d6c05-124">Accept</span></span>|<span data-ttu-id="d6c05-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d6c05-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6c05-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d6c05-126">Request body</span></span>
<span data-ttu-id="d6c05-127">要求本文で、[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d6c05-127">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="d6c05-128">次の表に、[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d6c05-128">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="d6c05-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6c05-129">Property</span></span>|<span data-ttu-id="d6c05-130">型</span><span class="sxs-lookup"><span data-stu-id="d6c05-130">Type</span></span>|<span data-ttu-id="d6c05-131">説明</span><span class="sxs-lookup"><span data-stu-id="d6c05-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6c05-132">id</span><span class="sxs-lookup"><span data-stu-id="d6c05-132">id</span></span>|<span data-ttu-id="d6c05-133">String</span><span class="sxs-lookup"><span data-stu-id="d6c05-133">String</span></span>|<span data-ttu-id="d6c05-134">証明書の一意識別子</span><span class="sxs-lookup"><span data-stu-id="d6c05-134">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="d6c05-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="d6c05-135">appleIdentifier</span></span>|<span data-ttu-id="d6c05-136">String</span><span class="sxs-lookup"><span data-stu-id="d6c05-136">String</span></span>|<span data-ttu-id="d6c05-137">MDM プッシュ証明書の作成に使用するアカウントの Apple ID。</span><span class="sxs-lookup"><span data-stu-id="d6c05-137">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="d6c05-138">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="d6c05-138">topicIdentifier</span></span>|<span data-ttu-id="d6c05-139">String</span><span class="sxs-lookup"><span data-stu-id="d6c05-139">String</span></span>|<span data-ttu-id="d6c05-140">トピック ID。</span><span class="sxs-lookup"><span data-stu-id="d6c05-140">Topic Id.</span></span>|
|<span data-ttu-id="d6c05-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6c05-141">lastModifiedDateTime</span></span>|<span data-ttu-id="d6c05-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6c05-142">DateTimeOffset</span></span>|<span data-ttu-id="d6c05-143">Apple プッシュ通知証明書の最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="d6c05-143">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="d6c05-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d6c05-144">expirationDateTime</span></span>|<span data-ttu-id="d6c05-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6c05-145">DateTimeOffset</span></span>|<span data-ttu-id="d6c05-146">Apple プッシュ通知証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="d6c05-146">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="d6c05-147">certificateuploadstatus</span><span class="sxs-lookup"><span data-stu-id="d6c05-147">certificateUploadStatus</span></span>|<span data-ttu-id="d6c05-148">String</span><span class="sxs-lookup"><span data-stu-id="d6c05-148">String</span></span>|<span data-ttu-id="d6c05-149">証明書のアップロード状態。</span><span class="sxs-lookup"><span data-stu-id="d6c05-149">The certificate upload status.</span></span>|
|<span data-ttu-id="d6c05-150">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="d6c05-150">certificateUploadFailureReason</span></span>|<span data-ttu-id="d6c05-151">String</span><span class="sxs-lookup"><span data-stu-id="d6c05-151">String</span></span>|<span data-ttu-id="d6c05-152">証明書のアップロードが失敗した理由。</span><span class="sxs-lookup"><span data-stu-id="d6c05-152">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="d6c05-153">証明書</span><span class="sxs-lookup"><span data-stu-id="d6c05-153">certificate</span></span>|<span data-ttu-id="d6c05-154">String</span><span class="sxs-lookup"><span data-stu-id="d6c05-154">String</span></span>|<span data-ttu-id="d6c05-155">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d6c05-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d6c05-156">応答</span><span class="sxs-lookup"><span data-stu-id="d6c05-156">Response</span></span>
<span data-ttu-id="d6c05-157">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d6c05-157">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6c05-158">例</span><span class="sxs-lookup"><span data-stu-id="d6c05-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6c05-159">要求</span><span class="sxs-lookup"><span data-stu-id="d6c05-159">Request</span></span>
<span data-ttu-id="d6c05-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d6c05-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 416

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificateUploadStatus": "Certificate Upload Status value",
  "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="d6c05-161">応答</span><span class="sxs-lookup"><span data-stu-id="d6c05-161">Response</span></span>
<span data-ttu-id="d6c05-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d6c05-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




