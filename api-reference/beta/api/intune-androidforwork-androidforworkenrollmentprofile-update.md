---
title: androidForWorkEnrollmentProfile の更新
description: androidForWorkEnrollmentProfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 77c5dcd3af7caf26c8320486ccb693c5004acc7a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145627"
---
# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="d9575-103">androidForWorkEnrollmentProfile の更新</span><span class="sxs-lookup"><span data-stu-id="d9575-103">Update androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="d9575-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9575-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9575-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d9575-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9575-106">[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d9575-106">Update the properties of a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9575-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d9575-107">Prerequisites</span></span>
<span data-ttu-id="d9575-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d9575-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d9575-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d9575-110">Permission type</span></span>|<span data-ttu-id="d9575-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d9575-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9575-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d9575-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d9575-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9575-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d9575-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d9575-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9575-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9575-115">Not supported.</span></span>|
|<span data-ttu-id="d9575-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d9575-116">Application</span></span>|<span data-ttu-id="d9575-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9575-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9575-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d9575-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="d9575-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d9575-119">Request headers</span></span>
|<span data-ttu-id="d9575-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d9575-120">Header</span></span>|<span data-ttu-id="d9575-121">値</span><span class="sxs-lookup"><span data-stu-id="d9575-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9575-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9575-122">Authorization</span></span>|<span data-ttu-id="d9575-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d9575-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9575-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d9575-124">Accept</span></span>|<span data-ttu-id="d9575-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d9575-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9575-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d9575-126">Request body</span></span>
<span data-ttu-id="d9575-127">要求本文で、[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d9575-127">In the request body, supply a JSON representation for the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="d9575-128">次の表に、[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d9575-128">The following table shows the properties that are required when you create the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span></span>

|<span data-ttu-id="d9575-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9575-129">Property</span></span>|<span data-ttu-id="d9575-130">型</span><span class="sxs-lookup"><span data-stu-id="d9575-130">Type</span></span>|<span data-ttu-id="d9575-131">説明</span><span class="sxs-lookup"><span data-stu-id="d9575-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9575-132">accountId</span><span class="sxs-lookup"><span data-stu-id="d9575-132">accountId</span></span>|<span data-ttu-id="d9575-133">String</span><span class="sxs-lookup"><span data-stu-id="d9575-133">String</span></span>|<span data-ttu-id="d9575-134">登録プロファイルが属するテナント GUID。</span><span class="sxs-lookup"><span data-stu-id="d9575-134">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="d9575-135">id</span><span class="sxs-lookup"><span data-stu-id="d9575-135">id</span></span>|<span data-ttu-id="d9575-136">文字列</span><span class="sxs-lookup"><span data-stu-id="d9575-136">String</span></span>|<span data-ttu-id="d9575-137">登録プロファイル用の一意な GUID。</span><span class="sxs-lookup"><span data-stu-id="d9575-137">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="d9575-138">displayName</span><span class="sxs-lookup"><span data-stu-id="d9575-138">displayName</span></span>|<span data-ttu-id="d9575-139">String</span><span class="sxs-lookup"><span data-stu-id="d9575-139">String</span></span>|<span data-ttu-id="d9575-140">登録プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="d9575-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="d9575-141">説明</span><span class="sxs-lookup"><span data-stu-id="d9575-141">description</span></span>|<span data-ttu-id="d9575-142">文字列</span><span class="sxs-lookup"><span data-stu-id="d9575-142">String</span></span>|<span data-ttu-id="d9575-143">登録プロファイルの説明。</span><span class="sxs-lookup"><span data-stu-id="d9575-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="d9575-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9575-144">createdDateTime</span></span>|<span data-ttu-id="d9575-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9575-145">DateTimeOffset</span></span>|<span data-ttu-id="d9575-146">登録プロファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="d9575-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="d9575-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9575-147">lastModifiedDateTime</span></span>|<span data-ttu-id="d9575-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9575-148">DateTimeOffset</span></span>|<span data-ttu-id="d9575-149">登録プロファイルが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="d9575-149">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="d9575-150">tokenValue</span><span class="sxs-lookup"><span data-stu-id="d9575-150">tokenValue</span></span>|<span data-ttu-id="d9575-151">String</span><span class="sxs-lookup"><span data-stu-id="d9575-151">String</span></span>|<span data-ttu-id="d9575-152">この登録プロファイル用に最後に作成されたトークンの値。</span><span class="sxs-lookup"><span data-stu-id="d9575-152">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="d9575-153">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d9575-153">tokenExpirationDateTime</span></span>|<span data-ttu-id="d9575-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9575-154">DateTimeOffset</span></span>|<span data-ttu-id="d9575-155">最後に作成されたトークンの有効期限が切れる日時。</span><span class="sxs-lookup"><span data-stu-id="d9575-155">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="d9575-156">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d9575-156">enrolledDeviceCount</span></span>|<span data-ttu-id="d9575-157">Int32</span><span class="sxs-lookup"><span data-stu-id="d9575-157">Int32</span></span>|<span data-ttu-id="d9575-158">この登録プロファイルを使用して登録した Android デバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="d9575-158">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="d9575-159">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="d9575-159">qrCodeContent</span></span>|<span data-ttu-id="d9575-160">String</span><span class="sxs-lookup"><span data-stu-id="d9575-160">String</span></span>|<span data-ttu-id="d9575-161">トークン用の QR コードを生成するために使用された文字列。</span><span class="sxs-lookup"><span data-stu-id="d9575-161">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="d9575-162">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="d9575-162">qrCodeImage</span></span>|[<span data-ttu-id="d9575-163">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d9575-163">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d9575-164">トークン用の QR コードを生成するために使用された文字列。</span><span class="sxs-lookup"><span data-stu-id="d9575-164">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="d9575-165">応答</span><span class="sxs-lookup"><span data-stu-id="d9575-165">Response</span></span>
<span data-ttu-id="d9575-166">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d9575-166">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9575-167">例</span><span class="sxs-lookup"><span data-stu-id="d9575-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9575-168">要求</span><span class="sxs-lookup"><span data-stu-id="d9575-168">Request</span></span>
<span data-ttu-id="d9575-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d9575-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
Content-type: application/json
Content-length: 496

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="d9575-170">応答</span><span class="sxs-lookup"><span data-stu-id="d9575-170">Response</span></span>
<span data-ttu-id="d9575-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d9575-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




