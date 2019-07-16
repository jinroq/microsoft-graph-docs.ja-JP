---
title: PfxRecryptionRequest の更新
description: PfxRecryptionRequest オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca4addaae01a6fea69d1742338e0452ed7227380
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741436"
---
# <a name="update-pfxrecryptionrequest"></a><span data-ttu-id="e930e-103">PfxRecryptionRequest の更新</span><span class="sxs-lookup"><span data-stu-id="e930e-103">Update pfxRecryptionRequest</span></span>

> <span data-ttu-id="e930e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e930e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e930e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e930e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e930e-106">[PfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e930e-106">Update the properties of a [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e930e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e930e-107">Prerequisites</span></span>
<span data-ttu-id="e930e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e930e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e930e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e930e-110">Permission type</span></span>|<span data-ttu-id="e930e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e930e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e930e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e930e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e930e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e930e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e930e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e930e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e930e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e930e-115">Not supported.</span></span>|
|<span data-ttu-id="e930e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e930e-116">Application</span></span>|<span data-ttu-id="e930e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e930e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e930e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e930e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /pfxRecryptionRequests/{pfxRecryptionRequestsId}
```

## <a name="request-headers"></a><span data-ttu-id="e930e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e930e-119">Request headers</span></span>
|<span data-ttu-id="e930e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e930e-120">Header</span></span>|<span data-ttu-id="e930e-121">値</span><span class="sxs-lookup"><span data-stu-id="e930e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e930e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e930e-122">Authorization</span></span>|<span data-ttu-id="e930e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e930e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e930e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e930e-124">Accept</span></span>|<span data-ttu-id="e930e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e930e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e930e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e930e-126">Request body</span></span>
<span data-ttu-id="e930e-127">要求本文で、 [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e930e-127">In the request body, supply a JSON representation for the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

<span data-ttu-id="e930e-128">次の表に、 [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e930e-128">The following table shows the properties that are required when you create the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md).</span></span>

|<span data-ttu-id="e930e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e930e-129">Property</span></span>|<span data-ttu-id="e930e-130">型</span><span class="sxs-lookup"><span data-stu-id="e930e-130">Type</span></span>|<span data-ttu-id="e930e-131">説明</span><span class="sxs-lookup"><span data-stu-id="e930e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e930e-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="e930e-132">tenantId</span></span>|<span data-ttu-id="e930e-133">Guid</span><span class="sxs-lookup"><span data-stu-id="e930e-133">Guid</span></span>|<span data-ttu-id="e930e-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e930e-134">Not yet documented</span></span>|
|<span data-ttu-id="e930e-135">userId</span><span class="sxs-lookup"><span data-stu-id="e930e-135">userId</span></span>|<span data-ttu-id="e930e-136">Guid</span><span class="sxs-lookup"><span data-stu-id="e930e-136">Guid</span></span>|<span data-ttu-id="e930e-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e930e-137">Not yet documented</span></span>|
|<span data-ttu-id="e930e-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="e930e-138">deviceId</span></span>|<span data-ttu-id="e930e-139">Guid</span><span class="sxs-lookup"><span data-stu-id="e930e-139">Guid</span></span>|<span data-ttu-id="e930e-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e930e-140">Not yet documented</span></span>|
|<span data-ttu-id="e930e-141">profileId</span><span class="sxs-lookup"><span data-stu-id="e930e-141">profileId</span></span>|<span data-ttu-id="e930e-142">Guid</span><span class="sxs-lookup"><span data-stu-id="e930e-142">Guid</span></span>|<span data-ttu-id="e930e-143">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e930e-143">Not yet documented</span></span>|
|<span data-ttu-id="e930e-144">拇印</span><span class="sxs-lookup"><span data-stu-id="e930e-144">thumbprint</span></span>|<span data-ttu-id="e930e-145">String</span><span class="sxs-lookup"><span data-stu-id="e930e-145">String</span></span>|<span data-ttu-id="e930e-146">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e930e-146">Not yet documented</span></span>|
|<span data-ttu-id="e930e-147">deviceKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="e930e-147">deviceKeyThumbprint</span></span>|<span data-ttu-id="e930e-148">String</span><span class="sxs-lookup"><span data-stu-id="e930e-148">String</span></span>|<span data-ttu-id="e930e-149">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e930e-149">Not yet documented</span></span>|
|<span data-ttu-id="e930e-150">status</span><span class="sxs-lookup"><span data-stu-id="e930e-150">status</span></span>|<span data-ttu-id="e930e-151">Int32</span><span class="sxs-lookup"><span data-stu-id="e930e-151">Int32</span></span>|<span data-ttu-id="e930e-152">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e930e-152">Not yet documented</span></span>|
|<span data-ttu-id="e930e-153">sourceType</span><span class="sxs-lookup"><span data-stu-id="e930e-153">sourceType</span></span>|<span data-ttu-id="e930e-154">Int32</span><span class="sxs-lookup"><span data-stu-id="e930e-154">Int32</span></span>|<span data-ttu-id="e930e-155">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e930e-155">Not yet documented</span></span>|
|<span data-ttu-id="e930e-156">createdTime</span><span class="sxs-lookup"><span data-stu-id="e930e-156">createdTime</span></span>|<span data-ttu-id="e930e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e930e-157">DateTimeOffset</span></span>|<span data-ttu-id="e930e-158">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e930e-158">Not yet documented</span></span>|
|<span data-ttu-id="e930e-159">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="e930e-159">lastModifiedTime</span></span>|<span data-ttu-id="e930e-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e930e-160">DateTimeOffset</span></span>|<span data-ttu-id="e930e-161">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e930e-161">Not yet documented</span></span>|
|<span data-ttu-id="e930e-162">isDeleted</span><span class="sxs-lookup"><span data-stu-id="e930e-162">isDeleted</span></span>|<span data-ttu-id="e930e-163">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="e930e-163">Boolean</span></span>|<span data-ttu-id="e930e-164">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e930e-164">Not yet documented</span></span>|
|<span data-ttu-id="e930e-165">eTag</span><span class="sxs-lookup"><span data-stu-id="e930e-165">eTag</span></span>|<span data-ttu-id="e930e-166">String</span><span class="sxs-lookup"><span data-stu-id="e930e-166">String</span></span>|<span data-ttu-id="e930e-167">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e930e-167">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e930e-168">応答</span><span class="sxs-lookup"><span data-stu-id="e930e-168">Response</span></span>
<span data-ttu-id="e930e-169">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e930e-169">If successful, this method returns a `200 OK` response code and an updated [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e930e-170">例</span><span class="sxs-lookup"><span data-stu-id="e930e-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="e930e-171">要求</span><span class="sxs-lookup"><span data-stu-id="e930e-171">Request</span></span>
<span data-ttu-id="e930e-172">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e930e-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/pfxRecryptionRequests/{pfxRecryptionRequestsId}
Content-type: application/json
Content-length: 574

{
  "@odata.type": "#microsoft.graph.pfxRecryptionRequest",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
  "profileId": "6389d896-d896-6389-96d8-896396d88963",
  "thumbprint": "Thumbprint value",
  "deviceKeyThumbprint": "Device Key Thumbprint value",
  "status": 6,
  "sourceType": 10,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "isDeleted": true,
  "eTag": "ETag value"
}
```

### <a name="response"></a><span data-ttu-id="e930e-173">応答</span><span class="sxs-lookup"><span data-stu-id="e930e-173">Response</span></span>
<span data-ttu-id="e930e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e930e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.pfxRecryptionRequest",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
  "profileId": "6389d896-d896-6389-96d8-896396d88963",
  "thumbprint": "Thumbprint value",
  "deviceKeyThumbprint": "Device Key Thumbprint value",
  "status": 6,
  "sourceType": 10,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "isDeleted": true,
  "eTag": "ETag value"
}
```





