---
title: OnPremEncryptedPayload の更新
description: OnPremEncryptedPayload オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a50048080072c8bcc7feb08cac69d74a18460c19
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741455"
---
# <a name="update-onpremencryptedpayload"></a><span data-ttu-id="e2704-103">OnPremEncryptedPayload の更新</span><span class="sxs-lookup"><span data-stu-id="e2704-103">Update onPremEncryptedPayload</span></span>

> <span data-ttu-id="e2704-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2704-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2704-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e2704-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2704-106">[OnPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e2704-106">Update the properties of a [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2704-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e2704-107">Prerequisites</span></span>
<span data-ttu-id="e2704-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2704-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2704-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e2704-110">Permission type</span></span>|<span data-ttu-id="e2704-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e2704-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2704-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e2704-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e2704-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2704-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e2704-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e2704-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2704-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2704-115">Not supported.</span></span>|
|<span data-ttu-id="e2704-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e2704-116">Application</span></span>|<span data-ttu-id="e2704-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2704-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2704-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2704-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
```

## <a name="request-headers"></a><span data-ttu-id="e2704-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2704-119">Request headers</span></span>
|<span data-ttu-id="e2704-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2704-120">Header</span></span>|<span data-ttu-id="e2704-121">値</span><span class="sxs-lookup"><span data-stu-id="e2704-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2704-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2704-122">Authorization</span></span>|<span data-ttu-id="e2704-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e2704-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2704-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e2704-124">Accept</span></span>|<span data-ttu-id="e2704-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e2704-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2704-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e2704-126">Request body</span></span>
<span data-ttu-id="e2704-127">要求本文で、 [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e2704-127">In the request body, supply a JSON representation for the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

<span data-ttu-id="e2704-128">次の表に、 [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e2704-128">The following table shows the properties that are required when you create the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md).</span></span>

|<span data-ttu-id="e2704-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2704-129">Property</span></span>|<span data-ttu-id="e2704-130">型</span><span class="sxs-lookup"><span data-stu-id="e2704-130">Type</span></span>|<span data-ttu-id="e2704-131">説明</span><span class="sxs-lookup"><span data-stu-id="e2704-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2704-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="e2704-132">tenantId</span></span>|<span data-ttu-id="e2704-133">Guid</span><span class="sxs-lookup"><span data-stu-id="e2704-133">Guid</span></span>|<span data-ttu-id="e2704-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e2704-134">Not yet documented</span></span>|
|<span data-ttu-id="e2704-135">userId</span><span class="sxs-lookup"><span data-stu-id="e2704-135">userId</span></span>|<span data-ttu-id="e2704-136">Guid</span><span class="sxs-lookup"><span data-stu-id="e2704-136">Guid</span></span>|<span data-ttu-id="e2704-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e2704-137">Not yet documented</span></span>|
|<span data-ttu-id="e2704-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="e2704-138">deviceId</span></span>|<span data-ttu-id="e2704-139">Guid</span><span class="sxs-lookup"><span data-stu-id="e2704-139">Guid</span></span>|<span data-ttu-id="e2704-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e2704-140">Not yet documented</span></span>|
|<span data-ttu-id="e2704-141">payloadId</span><span class="sxs-lookup"><span data-stu-id="e2704-141">payloadId</span></span>|<span data-ttu-id="e2704-142">Guid</span><span class="sxs-lookup"><span data-stu-id="e2704-142">Guid</span></span>|<span data-ttu-id="e2704-143">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e2704-143">Not yet documented</span></span>|
|<span data-ttu-id="e2704-144">deviceKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="e2704-144">deviceKeyThumbprint</span></span>|<span data-ttu-id="e2704-145">String</span><span class="sxs-lookup"><span data-stu-id="e2704-145">String</span></span>|<span data-ttu-id="e2704-146">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e2704-146">Not yet documented</span></span>|
|<span data-ttu-id="e2704-147">cert1PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="e2704-147">cert1PayloadUUID</span></span>|<span data-ttu-id="e2704-148">String</span><span class="sxs-lookup"><span data-stu-id="e2704-148">String</span></span>|<span data-ttu-id="e2704-149">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e2704-149">Not yet documented</span></span>|
|<span data-ttu-id="e2704-150">cert2PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="e2704-150">cert2PayloadUUID</span></span>|<span data-ttu-id="e2704-151">String</span><span class="sxs-lookup"><span data-stu-id="e2704-151">String</span></span>|<span data-ttu-id="e2704-152">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e2704-152">Not yet documented</span></span>|
|<span data-ttu-id="e2704-153">cert3PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="e2704-153">cert3PayloadUUID</span></span>|<span data-ttu-id="e2704-154">String</span><span class="sxs-lookup"><span data-stu-id="e2704-154">String</span></span>|<span data-ttu-id="e2704-155">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e2704-155">Not yet documented</span></span>|
|<span data-ttu-id="e2704-156">plistTemplate</span><span class="sxs-lookup"><span data-stu-id="e2704-156">plistTemplate</span></span>|<span data-ttu-id="e2704-157">String</span><span class="sxs-lookup"><span data-stu-id="e2704-157">String</span></span>|<span data-ttu-id="e2704-158">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e2704-158">Not yet documented</span></span>|
|<span data-ttu-id="e2704-159">encryptedBlob</span><span class="sxs-lookup"><span data-stu-id="e2704-159">encryptedBlob</span></span>|<span data-ttu-id="e2704-160">Binary</span><span class="sxs-lookup"><span data-stu-id="e2704-160">Binary</span></span>|<span data-ttu-id="e2704-161">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e2704-161">Not yet documented</span></span>|
|<span data-ttu-id="e2704-162">payloadVersion</span><span class="sxs-lookup"><span data-stu-id="e2704-162">payloadVersion</span></span>|<span data-ttu-id="e2704-163">Int32</span><span class="sxs-lookup"><span data-stu-id="e2704-163">Int32</span></span>|<span data-ttu-id="e2704-164">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e2704-164">Not yet documented</span></span>|
|<span data-ttu-id="e2704-165">status</span><span class="sxs-lookup"><span data-stu-id="e2704-165">status</span></span>|<span data-ttu-id="e2704-166">Int32</span><span class="sxs-lookup"><span data-stu-id="e2704-166">Int32</span></span>|<span data-ttu-id="e2704-167">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e2704-167">Not yet documented</span></span>|
|<span data-ttu-id="e2704-168">createdTime</span><span class="sxs-lookup"><span data-stu-id="e2704-168">createdTime</span></span>|<span data-ttu-id="e2704-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2704-169">DateTimeOffset</span></span>|<span data-ttu-id="e2704-170">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e2704-170">Not yet documented</span></span>|
|<span data-ttu-id="e2704-171">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="e2704-171">lastModifiedTime</span></span>|<span data-ttu-id="e2704-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2704-172">DateTimeOffset</span></span>|<span data-ttu-id="e2704-173">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e2704-173">Not yet documented</span></span>|
|<span data-ttu-id="e2704-174">eTag</span><span class="sxs-lookup"><span data-stu-id="e2704-174">eTag</span></span>|<span data-ttu-id="e2704-175">String</span><span class="sxs-lookup"><span data-stu-id="e2704-175">String</span></span>|<span data-ttu-id="e2704-176">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e2704-176">Not yet documented</span></span>|
|<span data-ttu-id="e2704-177">isDeleted</span><span class="sxs-lookup"><span data-stu-id="e2704-177">isDeleted</span></span>|<span data-ttu-id="e2704-178">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="e2704-178">Boolean</span></span>|<span data-ttu-id="e2704-179">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e2704-179">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e2704-180">応答</span><span class="sxs-lookup"><span data-stu-id="e2704-180">Response</span></span>
<span data-ttu-id="e2704-181">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e2704-181">If successful, this method returns a `200 OK` response code and an updated [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2704-182">例</span><span class="sxs-lookup"><span data-stu-id="e2704-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2704-183">要求</span><span class="sxs-lookup"><span data-stu-id="e2704-183">Request</span></span>
<span data-ttu-id="e2704-184">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e2704-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
Content-type: application/json
Content-length: 781

{
  "@odata.type": "#microsoft.graph.onPremEncryptedPayload",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
  "payloadId": "f12f6c03-6c03-f12f-036c-2ff1036c2ff1",
  "deviceKeyThumbprint": "Device Key Thumbprint value",
  "cert1PayloadUUID": "Cert1Payload UUID value",
  "cert2PayloadUUID": "Cert2Payload UUID value",
  "cert3PayloadUUID": "Cert3Payload UUID value",
  "plistTemplate": "Plist Template value",
  "encryptedBlob": "ZW5jcnlwdGVkQmxvYg==",
  "payloadVersion": 14,
  "status": 6,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value",
  "isDeleted": true
}
```

### <a name="response"></a><span data-ttu-id="e2704-185">応答</span><span class="sxs-lookup"><span data-stu-id="e2704-185">Response</span></span>
<span data-ttu-id="e2704-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e2704-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 781

{
  "@odata.type": "#microsoft.graph.onPremEncryptedPayload",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
  "payloadId": "f12f6c03-6c03-f12f-036c-2ff1036c2ff1",
  "deviceKeyThumbprint": "Device Key Thumbprint value",
  "cert1PayloadUUID": "Cert1Payload UUID value",
  "cert2PayloadUUID": "Cert2Payload UUID value",
  "cert3PayloadUUID": "Cert3Payload UUID value",
  "plistTemplate": "Plist Template value",
  "encryptedBlob": "ZW5jcnlwdGVkQmxvYg==",
  "payloadVersion": 14,
  "status": 6,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value",
  "isDeleted": true
}
```





