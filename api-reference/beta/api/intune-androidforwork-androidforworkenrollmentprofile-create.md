---
title: Create androidForWorkEnrollmentProfile
description: 新しい androidForWorkEnrollmentProfile オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: da20ba9352dd14d1168ac76b4fb4a4f92d8d6726
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938682"
---
# <a name="create-androidforworkenrollmentprofile"></a><span data-ttu-id="0c78a-103">Create androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="0c78a-103">Create androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="0c78a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c78a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c78a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0c78a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c78a-106">新しい [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0c78a-106">Create a new [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c78a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0c78a-107">Prerequisites</span></span>
<span data-ttu-id="0c78a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c78a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c78a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0c78a-110">Permission type</span></span>|<span data-ttu-id="0c78a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0c78a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c78a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0c78a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c78a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c78a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c78a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0c78a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c78a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c78a-115">Not supported.</span></span>|
|<span data-ttu-id="0c78a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0c78a-116">Application</span></span>|<span data-ttu-id="0c78a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c78a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c78a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c78a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="0c78a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c78a-119">Request headers</span></span>
|<span data-ttu-id="0c78a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c78a-120">Header</span></span>|<span data-ttu-id="0c78a-121">値</span><span class="sxs-lookup"><span data-stu-id="0c78a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c78a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c78a-122">Authorization</span></span>|<span data-ttu-id="0c78a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0c78a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c78a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0c78a-124">Accept</span></span>|<span data-ttu-id="0c78a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c78a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c78a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0c78a-126">Request body</span></span>
<span data-ttu-id="0c78a-127">要求本文に、androidForWorkEnrollmentProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0c78a-127">In the request body, supply a JSON representation for the androidForWorkEnrollmentProfile object.</span></span>

<span data-ttu-id="0c78a-128">次の表に、androidForWorkEnrollmentProfile 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0c78a-128">The following table shows the properties that are required when you create the androidForWorkEnrollmentProfile.</span></span>

|<span data-ttu-id="0c78a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c78a-129">Property</span></span>|<span data-ttu-id="0c78a-130">型</span><span class="sxs-lookup"><span data-stu-id="0c78a-130">Type</span></span>|<span data-ttu-id="0c78a-131">説明</span><span class="sxs-lookup"><span data-stu-id="0c78a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c78a-132">accountId</span><span class="sxs-lookup"><span data-stu-id="0c78a-132">accountId</span></span>|<span data-ttu-id="0c78a-133">String</span><span class="sxs-lookup"><span data-stu-id="0c78a-133">String</span></span>|<span data-ttu-id="0c78a-134">登録プロファイルが属するテナント GUID。</span><span class="sxs-lookup"><span data-stu-id="0c78a-134">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="0c78a-135">id</span><span class="sxs-lookup"><span data-stu-id="0c78a-135">id</span></span>|<span data-ttu-id="0c78a-136">文字列</span><span class="sxs-lookup"><span data-stu-id="0c78a-136">String</span></span>|<span data-ttu-id="0c78a-137">登録プロファイルの一意の GUID。</span><span class="sxs-lookup"><span data-stu-id="0c78a-137">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="0c78a-138">displayName</span><span class="sxs-lookup"><span data-stu-id="0c78a-138">displayName</span></span>|<span data-ttu-id="0c78a-139">String</span><span class="sxs-lookup"><span data-stu-id="0c78a-139">String</span></span>|<span data-ttu-id="0c78a-140">登録プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="0c78a-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="0c78a-141">description</span><span class="sxs-lookup"><span data-stu-id="0c78a-141">description</span></span>|<span data-ttu-id="0c78a-142">String</span><span class="sxs-lookup"><span data-stu-id="0c78a-142">String</span></span>|<span data-ttu-id="0c78a-143">登録プロファイルの説明。</span><span class="sxs-lookup"><span data-stu-id="0c78a-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="0c78a-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c78a-144">createdDateTime</span></span>|<span data-ttu-id="0c78a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c78a-145">DateTimeOffset</span></span>|<span data-ttu-id="0c78a-146">登録プロファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="0c78a-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="0c78a-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c78a-147">lastModifiedDateTime</span></span>|<span data-ttu-id="0c78a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c78a-148">DateTimeOffset</span></span>|<span data-ttu-id="0c78a-149">登録プロファイルが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="0c78a-149">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="0c78a-150">tokenValue</span><span class="sxs-lookup"><span data-stu-id="0c78a-150">tokenValue</span></span>|<span data-ttu-id="0c78a-151">String</span><span class="sxs-lookup"><span data-stu-id="0c78a-151">String</span></span>|<span data-ttu-id="0c78a-152">この登録プロファイル用に最後に作成されたトークンの値。</span><span class="sxs-lookup"><span data-stu-id="0c78a-152">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="0c78a-153">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0c78a-153">tokenExpirationDateTime</span></span>|<span data-ttu-id="0c78a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c78a-154">DateTimeOffset</span></span>|<span data-ttu-id="0c78a-155">最後に作成されたトークンの有効期限が切れる日時。</span><span class="sxs-lookup"><span data-stu-id="0c78a-155">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="0c78a-156">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0c78a-156">enrolledDeviceCount</span></span>|<span data-ttu-id="0c78a-157">Int32</span><span class="sxs-lookup"><span data-stu-id="0c78a-157">Int32</span></span>|<span data-ttu-id="0c78a-158">この登録プロファイルを使用して登録した Android デバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="0c78a-158">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="0c78a-159">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="0c78a-159">qrCodeContent</span></span>|<span data-ttu-id="0c78a-160">String</span><span class="sxs-lookup"><span data-stu-id="0c78a-160">String</span></span>|<span data-ttu-id="0c78a-161">トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="0c78a-161">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="0c78a-162">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="0c78a-162">qrCodeImage</span></span>|[<span data-ttu-id="0c78a-163">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0c78a-163">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0c78a-164">トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="0c78a-164">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="0c78a-165">応答</span><span class="sxs-lookup"><span data-stu-id="0c78a-165">Response</span></span>
<span data-ttu-id="0c78a-166">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0c78a-166">If successful, this method returns a `201 Created` response code and a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c78a-167">例</span><span class="sxs-lookup"><span data-stu-id="0c78a-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c78a-168">要求</span><span class="sxs-lookup"><span data-stu-id="0c78a-168">Request</span></span>
<span data-ttu-id="0c78a-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0c78a-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="0c78a-170">応答</span><span class="sxs-lookup"><span data-stu-id="0c78a-170">Response</span></span>
<span data-ttu-id="0c78a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0c78a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




