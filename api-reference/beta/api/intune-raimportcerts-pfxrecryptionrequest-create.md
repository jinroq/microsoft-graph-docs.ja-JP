---
title: PfxRecryptionRequest を作成する
description: 新しい pfxRecryptionRequest オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 45b201a67892f5bd62e70456616f3ded099df39f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726095"
---
# <a name="create-pfxrecryptionrequest"></a><span data-ttu-id="db671-103">PfxRecryptionRequest を作成する</span><span class="sxs-lookup"><span data-stu-id="db671-103">Create pfxRecryptionRequest</span></span>

> <span data-ttu-id="db671-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db671-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db671-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="db671-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db671-106">新しい[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="db671-106">Create a new [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db671-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="db671-107">Prerequisites</span></span>
<span data-ttu-id="db671-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db671-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db671-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="db671-110">Permission type</span></span>|<span data-ttu-id="db671-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="db671-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db671-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="db671-112">Delegated (work or school account)</span></span>|<span data-ttu-id="db671-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db671-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="db671-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="db671-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db671-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db671-115">Not supported.</span></span>|
|<span data-ttu-id="db671-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="db671-116">Application</span></span>|<span data-ttu-id="db671-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db671-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db671-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="db671-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxRecryptionRequests
```

## <a name="request-headers"></a><span data-ttu-id="db671-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="db671-119">Request headers</span></span>
|<span data-ttu-id="db671-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="db671-120">Header</span></span>|<span data-ttu-id="db671-121">値</span><span class="sxs-lookup"><span data-stu-id="db671-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db671-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db671-122">Authorization</span></span>|<span data-ttu-id="db671-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="db671-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db671-124">承諾</span><span class="sxs-lookup"><span data-stu-id="db671-124">Accept</span></span>|<span data-ttu-id="db671-125">application/json</span><span class="sxs-lookup"><span data-stu-id="db671-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db671-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="db671-126">Request body</span></span>
<span data-ttu-id="db671-127">要求本文で、pfxRecryptionRequest オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="db671-127">In the request body, supply a JSON representation for the pfxRecryptionRequest object.</span></span>

<span data-ttu-id="db671-128">次の表に、pfxRecryptionRequest の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="db671-128">The following table shows the properties that are required when you create the pfxRecryptionRequest.</span></span>

|<span data-ttu-id="db671-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db671-129">Property</span></span>|<span data-ttu-id="db671-130">型</span><span class="sxs-lookup"><span data-stu-id="db671-130">Type</span></span>|<span data-ttu-id="db671-131">説明</span><span class="sxs-lookup"><span data-stu-id="db671-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db671-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="db671-132">tenantId</span></span>|<span data-ttu-id="db671-133">Guid</span><span class="sxs-lookup"><span data-stu-id="db671-133">Guid</span></span>|<span data-ttu-id="db671-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="db671-134">Not yet documented</span></span>|
|<span data-ttu-id="db671-135">userId</span><span class="sxs-lookup"><span data-stu-id="db671-135">userId</span></span>|<span data-ttu-id="db671-136">Guid</span><span class="sxs-lookup"><span data-stu-id="db671-136">Guid</span></span>|<span data-ttu-id="db671-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="db671-137">Not yet documented</span></span>|
|<span data-ttu-id="db671-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="db671-138">deviceId</span></span>|<span data-ttu-id="db671-139">Guid</span><span class="sxs-lookup"><span data-stu-id="db671-139">Guid</span></span>|<span data-ttu-id="db671-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="db671-140">Not yet documented</span></span>|
|<span data-ttu-id="db671-141">profileId</span><span class="sxs-lookup"><span data-stu-id="db671-141">profileId</span></span>|<span data-ttu-id="db671-142">Guid</span><span class="sxs-lookup"><span data-stu-id="db671-142">Guid</span></span>|<span data-ttu-id="db671-143">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="db671-143">Not yet documented</span></span>|
|<span data-ttu-id="db671-144">拇印</span><span class="sxs-lookup"><span data-stu-id="db671-144">thumbprint</span></span>|<span data-ttu-id="db671-145">String</span><span class="sxs-lookup"><span data-stu-id="db671-145">String</span></span>|<span data-ttu-id="db671-146">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="db671-146">Not yet documented</span></span>|
|<span data-ttu-id="db671-147">deviceKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="db671-147">deviceKeyThumbprint</span></span>|<span data-ttu-id="db671-148">String</span><span class="sxs-lookup"><span data-stu-id="db671-148">String</span></span>|<span data-ttu-id="db671-149">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="db671-149">Not yet documented</span></span>|
|<span data-ttu-id="db671-150">status</span><span class="sxs-lookup"><span data-stu-id="db671-150">status</span></span>|<span data-ttu-id="db671-151">Int32</span><span class="sxs-lookup"><span data-stu-id="db671-151">Int32</span></span>|<span data-ttu-id="db671-152">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="db671-152">Not yet documented</span></span>|
|<span data-ttu-id="db671-153">sourceType</span><span class="sxs-lookup"><span data-stu-id="db671-153">sourceType</span></span>|<span data-ttu-id="db671-154">Int32</span><span class="sxs-lookup"><span data-stu-id="db671-154">Int32</span></span>|<span data-ttu-id="db671-155">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="db671-155">Not yet documented</span></span>|
|<span data-ttu-id="db671-156">createdTime</span><span class="sxs-lookup"><span data-stu-id="db671-156">createdTime</span></span>|<span data-ttu-id="db671-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db671-157">DateTimeOffset</span></span>|<span data-ttu-id="db671-158">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="db671-158">Not yet documented</span></span>|
|<span data-ttu-id="db671-159">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="db671-159">lastModifiedTime</span></span>|<span data-ttu-id="db671-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db671-160">DateTimeOffset</span></span>|<span data-ttu-id="db671-161">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="db671-161">Not yet documented</span></span>|
|<span data-ttu-id="db671-162">isDeleted</span><span class="sxs-lookup"><span data-stu-id="db671-162">isDeleted</span></span>|<span data-ttu-id="db671-163">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="db671-163">Boolean</span></span>|<span data-ttu-id="db671-164">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="db671-164">Not yet documented</span></span>|
|<span data-ttu-id="db671-165">eTag</span><span class="sxs-lookup"><span data-stu-id="db671-165">eTag</span></span>|<span data-ttu-id="db671-166">String</span><span class="sxs-lookup"><span data-stu-id="db671-166">String</span></span>|<span data-ttu-id="db671-167">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="db671-167">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="db671-168">応答</span><span class="sxs-lookup"><span data-stu-id="db671-168">Response</span></span>
<span data-ttu-id="db671-169">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="db671-169">If successful, this method returns a `201 Created` response code and a [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db671-170">例</span><span class="sxs-lookup"><span data-stu-id="db671-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="db671-171">要求</span><span class="sxs-lookup"><span data-stu-id="db671-171">Request</span></span>
<span data-ttu-id="db671-172">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="db671-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/pfxRecryptionRequests
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

### <a name="response"></a><span data-ttu-id="db671-173">応答</span><span class="sxs-lookup"><span data-stu-id="db671-173">Response</span></span>
<span data-ttu-id="db671-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="db671-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





