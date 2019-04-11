---
title: androidForWorkEnrollmentProfile の更新
description: androidForWorkEnrollmentProfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2bbb90bda3e9e3306fc71be5ce38d6605f0d306
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776886"
---
# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="efad9-103">androidForWorkEnrollmentProfile の更新</span><span class="sxs-lookup"><span data-stu-id="efad9-103">Update androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="efad9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="efad9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efad9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="efad9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efad9-106">[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="efad9-106">Update the properties of a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efad9-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="efad9-107">Prerequisites</span></span>
<span data-ttu-id="efad9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="efad9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efad9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="efad9-110">Permission type</span></span>|<span data-ttu-id="efad9-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="efad9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efad9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="efad9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="efad9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efad9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="efad9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="efad9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efad9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="efad9-115">Not supported.</span></span>|
|<span data-ttu-id="efad9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="efad9-116">Application</span></span>|<span data-ttu-id="efad9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="efad9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efad9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="efad9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="efad9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="efad9-119">Request headers</span></span>
|<span data-ttu-id="efad9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="efad9-120">Header</span></span>|<span data-ttu-id="efad9-121">値</span><span class="sxs-lookup"><span data-stu-id="efad9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efad9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="efad9-122">Authorization</span></span>|<span data-ttu-id="efad9-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="efad9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efad9-124">承諾</span><span class="sxs-lookup"><span data-stu-id="efad9-124">Accept</span></span>|<span data-ttu-id="efad9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="efad9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efad9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="efad9-126">Request body</span></span>
<span data-ttu-id="efad9-127">要求本文で、[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="efad9-127">In the request body, supply a JSON representation for the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="efad9-128">次の表に、[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="efad9-128">The following table shows the properties that are required when you create the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span></span>

|<span data-ttu-id="efad9-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="efad9-129">Property</span></span>|<span data-ttu-id="efad9-130">型</span><span class="sxs-lookup"><span data-stu-id="efad9-130">Type</span></span>|<span data-ttu-id="efad9-131">説明</span><span class="sxs-lookup"><span data-stu-id="efad9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efad9-132">accountId</span><span class="sxs-lookup"><span data-stu-id="efad9-132">accountId</span></span>|<span data-ttu-id="efad9-133">文字列</span><span class="sxs-lookup"><span data-stu-id="efad9-133">String</span></span>|<span data-ttu-id="efad9-134">登録プロファイルが属するテナント GUID。</span><span class="sxs-lookup"><span data-stu-id="efad9-134">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="efad9-135">id</span><span class="sxs-lookup"><span data-stu-id="efad9-135">id</span></span>|<span data-ttu-id="efad9-136">文字列</span><span class="sxs-lookup"><span data-stu-id="efad9-136">String</span></span>|<span data-ttu-id="efad9-137">登録プロファイルの一意の GUID。</span><span class="sxs-lookup"><span data-stu-id="efad9-137">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="efad9-138">displayName</span><span class="sxs-lookup"><span data-stu-id="efad9-138">displayName</span></span>|<span data-ttu-id="efad9-139">String</span><span class="sxs-lookup"><span data-stu-id="efad9-139">String</span></span>|<span data-ttu-id="efad9-140">登録プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="efad9-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="efad9-141">説明</span><span class="sxs-lookup"><span data-stu-id="efad9-141">description</span></span>|<span data-ttu-id="efad9-142">String</span><span class="sxs-lookup"><span data-stu-id="efad9-142">String</span></span>|<span data-ttu-id="efad9-143">登録プロファイルの説明。</span><span class="sxs-lookup"><span data-stu-id="efad9-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="efad9-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="efad9-144">createdDateTime</span></span>|<span data-ttu-id="efad9-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efad9-145">DateTimeOffset</span></span>|<span data-ttu-id="efad9-146">登録プロファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="efad9-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="efad9-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="efad9-147">lastModifiedDateTime</span></span>|<span data-ttu-id="efad9-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efad9-148">DateTimeOffset</span></span>|<span data-ttu-id="efad9-149">登録プロファイルが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="efad9-149">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="efad9-150">tokenValue</span><span class="sxs-lookup"><span data-stu-id="efad9-150">tokenValue</span></span>|<span data-ttu-id="efad9-151">文字列</span><span class="sxs-lookup"><span data-stu-id="efad9-151">String</span></span>|<span data-ttu-id="efad9-152">この登録プロファイル用に最後に作成されたトークンの値。</span><span class="sxs-lookup"><span data-stu-id="efad9-152">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="efad9-153">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="efad9-153">tokenExpirationDateTime</span></span>|<span data-ttu-id="efad9-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efad9-154">DateTimeOffset</span></span>|<span data-ttu-id="efad9-155">最後に作成されたトークンの有効期限が切れる日時。</span><span class="sxs-lookup"><span data-stu-id="efad9-155">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="efad9-156">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="efad9-156">enrolledDeviceCount</span></span>|<span data-ttu-id="efad9-157">Int32</span><span class="sxs-lookup"><span data-stu-id="efad9-157">Int32</span></span>|<span data-ttu-id="efad9-158">この登録プロファイルを使用して登録した Android デバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="efad9-158">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="efad9-159">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="efad9-159">qrCodeContent</span></span>|<span data-ttu-id="efad9-160">String</span><span class="sxs-lookup"><span data-stu-id="efad9-160">String</span></span>|<span data-ttu-id="efad9-161">トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="efad9-161">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="efad9-162">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="efad9-162">qrCodeImage</span></span>|[<span data-ttu-id="efad9-163">mimeContent</span><span class="sxs-lookup"><span data-stu-id="efad9-163">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="efad9-164">トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="efad9-164">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="efad9-165">応答</span><span class="sxs-lookup"><span data-stu-id="efad9-165">Response</span></span>
<span data-ttu-id="efad9-166">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="efad9-166">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efad9-167">例</span><span class="sxs-lookup"><span data-stu-id="efad9-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="efad9-168">要求</span><span class="sxs-lookup"><span data-stu-id="efad9-168">Request</span></span>
<span data-ttu-id="efad9-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="efad9-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="efad9-170">応答</span><span class="sxs-lookup"><span data-stu-id="efad9-170">Response</span></span>
<span data-ttu-id="efad9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="efad9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





