---
title: PfxUserCertificate を作成する
description: 新しい pfxUserCertificate オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bda1a3e6b5f2296b3b7b1da62335cfdf7a8d10aa
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726088"
---
# <a name="create-pfxusercertificate"></a><span data-ttu-id="36877-103">PfxUserCertificate を作成する</span><span class="sxs-lookup"><span data-stu-id="36877-103">Create pfxUserCertificate</span></span>

> <span data-ttu-id="36877-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36877-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36877-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="36877-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36877-106">新しい[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="36877-106">Create a new [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36877-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="36877-107">Prerequisites</span></span>
<span data-ttu-id="36877-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36877-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36877-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="36877-110">Permission type</span></span>|<span data-ttu-id="36877-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="36877-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36877-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="36877-112">Delegated (work or school account)</span></span>|<span data-ttu-id="36877-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36877-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="36877-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="36877-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36877-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36877-115">Not supported.</span></span>|
|<span data-ttu-id="36877-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="36877-116">Application</span></span>|<span data-ttu-id="36877-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36877-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36877-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="36877-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxUserCertificates
```

## <a name="request-headers"></a><span data-ttu-id="36877-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36877-119">Request headers</span></span>
|<span data-ttu-id="36877-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36877-120">Header</span></span>|<span data-ttu-id="36877-121">値</span><span class="sxs-lookup"><span data-stu-id="36877-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36877-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="36877-122">Authorization</span></span>|<span data-ttu-id="36877-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="36877-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36877-124">承諾</span><span class="sxs-lookup"><span data-stu-id="36877-124">Accept</span></span>|<span data-ttu-id="36877-125">application/json</span><span class="sxs-lookup"><span data-stu-id="36877-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36877-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="36877-126">Request body</span></span>
<span data-ttu-id="36877-127">要求本文で、pfxUserCertificate オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="36877-127">In the request body, supply a JSON representation for the pfxUserCertificate object.</span></span>

<span data-ttu-id="36877-128">次の表に、pfxUserCertificate の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="36877-128">The following table shows the properties that are required when you create the pfxUserCertificate.</span></span>

|<span data-ttu-id="36877-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36877-129">Property</span></span>|<span data-ttu-id="36877-130">型</span><span class="sxs-lookup"><span data-stu-id="36877-130">Type</span></span>|<span data-ttu-id="36877-131">説明</span><span class="sxs-lookup"><span data-stu-id="36877-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36877-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="36877-132">tenantId</span></span>|<span data-ttu-id="36877-133">Guid</span><span class="sxs-lookup"><span data-stu-id="36877-133">Guid</span></span>|<span data-ttu-id="36877-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="36877-134">Not yet documented</span></span>|
|<span data-ttu-id="36877-135">userId</span><span class="sxs-lookup"><span data-stu-id="36877-135">userId</span></span>|<span data-ttu-id="36877-136">Guid</span><span class="sxs-lookup"><span data-stu-id="36877-136">Guid</span></span>|<span data-ttu-id="36877-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="36877-137">Not yet documented</span></span>|
|<span data-ttu-id="36877-138">拇印</span><span class="sxs-lookup"><span data-stu-id="36877-138">thumbprint</span></span>|<span data-ttu-id="36877-139">String</span><span class="sxs-lookup"><span data-stu-id="36877-139">String</span></span>|<span data-ttu-id="36877-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="36877-140">Not yet documented</span></span>|
|<span data-ttu-id="36877-141">userUpn</span><span class="sxs-lookup"><span data-stu-id="36877-141">userUpn</span></span>|<span data-ttu-id="36877-142">String</span><span class="sxs-lookup"><span data-stu-id="36877-142">String</span></span>|<span data-ttu-id="36877-143">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="36877-143">Not yet documented</span></span>|
|<span data-ttu-id="36877-144">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="36877-144">encryptedPfxBlob</span></span>|<span data-ttu-id="36877-145">String</span><span class="sxs-lookup"><span data-stu-id="36877-145">String</span></span>|<span data-ttu-id="36877-146">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="36877-146">Not yet documented</span></span>|
|<span data-ttu-id="36877-147">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="36877-147">encryptedPfxPassword</span></span>|<span data-ttu-id="36877-148">String</span><span class="sxs-lookup"><span data-stu-id="36877-148">String</span></span>|<span data-ttu-id="36877-149">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="36877-149">Not yet documented</span></span>|
|<span data-ttu-id="36877-150">certStartDate</span><span class="sxs-lookup"><span data-stu-id="36877-150">certStartDate</span></span>|<span data-ttu-id="36877-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36877-151">DateTimeOffset</span></span>|<span data-ttu-id="36877-152">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="36877-152">Not yet documented</span></span>|
|<span data-ttu-id="36877-153">certExpirationDate</span><span class="sxs-lookup"><span data-stu-id="36877-153">certExpirationDate</span></span>|<span data-ttu-id="36877-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36877-154">DateTimeOffset</span></span>|<span data-ttu-id="36877-155">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="36877-155">Not yet documented</span></span>|
|<span data-ttu-id="36877-156">プロバイダー</span><span class="sxs-lookup"><span data-stu-id="36877-156">providerName</span></span>|<span data-ttu-id="36877-157">String</span><span class="sxs-lookup"><span data-stu-id="36877-157">String</span></span>|<span data-ttu-id="36877-158">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="36877-158">Not yet documented</span></span>|
|<span data-ttu-id="36877-159">encryptionKeyName</span><span class="sxs-lookup"><span data-stu-id="36877-159">encryptionKeyName</span></span>|<span data-ttu-id="36877-160">String</span><span class="sxs-lookup"><span data-stu-id="36877-160">String</span></span>|<span data-ttu-id="36877-161">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="36877-161">Not yet documented</span></span>|
|<span data-ttu-id="36877-162">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="36877-162">paddingScheme</span></span>|<span data-ttu-id="36877-163">Int32</span><span class="sxs-lookup"><span data-stu-id="36877-163">Int32</span></span>|<span data-ttu-id="36877-164">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="36877-164">Not yet documented</span></span>|
|<span data-ttu-id="36877-165">status</span><span class="sxs-lookup"><span data-stu-id="36877-165">status</span></span>|<span data-ttu-id="36877-166">Int32</span><span class="sxs-lookup"><span data-stu-id="36877-166">Int32</span></span>|<span data-ttu-id="36877-167">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="36877-167">Not yet documented</span></span>|
|<span data-ttu-id="36877-168">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="36877-168">intendedPurpose</span></span>|<span data-ttu-id="36877-169">Int32</span><span class="sxs-lookup"><span data-stu-id="36877-169">Int32</span></span>|<span data-ttu-id="36877-170">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="36877-170">Not yet documented</span></span>|
|<span data-ttu-id="36877-171">createdTime</span><span class="sxs-lookup"><span data-stu-id="36877-171">createdTime</span></span>|<span data-ttu-id="36877-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36877-172">DateTimeOffset</span></span>|<span data-ttu-id="36877-173">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="36877-173">Not yet documented</span></span>|
|<span data-ttu-id="36877-174">isDeleted</span><span class="sxs-lookup"><span data-stu-id="36877-174">isDeleted</span></span>|<span data-ttu-id="36877-175">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="36877-175">Boolean</span></span>|<span data-ttu-id="36877-176">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="36877-176">Not yet documented</span></span>|
|<span data-ttu-id="36877-177">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="36877-177">lastModifiedTime</span></span>|<span data-ttu-id="36877-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36877-178">DateTimeOffset</span></span>|<span data-ttu-id="36877-179">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="36877-179">Not yet documented</span></span>|
|<span data-ttu-id="36877-180">eTag</span><span class="sxs-lookup"><span data-stu-id="36877-180">eTag</span></span>|<span data-ttu-id="36877-181">String</span><span class="sxs-lookup"><span data-stu-id="36877-181">String</span></span>|<span data-ttu-id="36877-182">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="36877-182">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="36877-183">応答</span><span class="sxs-lookup"><span data-stu-id="36877-183">Response</span></span>
<span data-ttu-id="36877-184">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="36877-184">If successful, this method returns a `201 Created` response code and a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36877-185">例</span><span class="sxs-lookup"><span data-stu-id="36877-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="36877-186">要求</span><span class="sxs-lookup"><span data-stu-id="36877-186">Request</span></span>
<span data-ttu-id="36877-187">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="36877-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/pfxUserCertificates
Content-type: application/json
Content-length: 789

{
  "@odata.type": "#microsoft.graph.pfxUserCertificate",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "thumbprint": "Thumbprint value",
  "userUpn": "User Upn value",
  "encryptedPfxBlob": "Encrypted Pfx Blob value",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "certStartDate": "2017-01-01T00:01:48.7697664-08:00",
  "certExpirationDate": "2016-12-31T23:56:39.3841403-08:00",
  "providerName": "Provider Name value",
  "encryptionKeyName": "Encryption Key Name value",
  "paddingScheme": 13,
  "status": 6,
  "intendedPurpose": 15,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "isDeleted": true,
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value"
}
```

### <a name="response"></a><span data-ttu-id="36877-188">応答</span><span class="sxs-lookup"><span data-stu-id="36877-188">Response</span></span>
<span data-ttu-id="36877-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="36877-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 789

{
  "@odata.type": "#microsoft.graph.pfxUserCertificate",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "thumbprint": "Thumbprint value",
  "userUpn": "User Upn value",
  "encryptedPfxBlob": "Encrypted Pfx Blob value",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "certStartDate": "2017-01-01T00:01:48.7697664-08:00",
  "certExpirationDate": "2016-12-31T23:56:39.3841403-08:00",
  "providerName": "Provider Name value",
  "encryptionKeyName": "Encryption Key Name value",
  "paddingScheme": 13,
  "status": 6,
  "intendedPurpose": 15,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "isDeleted": true,
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value"
}
```





