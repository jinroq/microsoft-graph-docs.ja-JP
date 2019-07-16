---
title: PfxUserCertificate の更新
description: PfxUserCertificate オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6756a6c35818426790e24d7f348ca760355ffec6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726087"
---
# <a name="update-pfxusercertificate"></a><span data-ttu-id="0c343-103">PfxUserCertificate の更新</span><span class="sxs-lookup"><span data-stu-id="0c343-103">Update pfxUserCertificate</span></span>

> <span data-ttu-id="0c343-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c343-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c343-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0c343-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c343-106">[PfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0c343-106">Update the properties of a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c343-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0c343-107">Prerequisites</span></span>
<span data-ttu-id="0c343-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c343-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c343-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0c343-110">Permission type</span></span>|<span data-ttu-id="0c343-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0c343-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c343-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0c343-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c343-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c343-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c343-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0c343-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c343-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c343-115">Not supported.</span></span>|
|<span data-ttu-id="0c343-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0c343-116">Application</span></span>|<span data-ttu-id="0c343-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c343-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c343-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c343-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /pfxUserCertificates/{pfxUserCertificatesId}
```

## <a name="request-headers"></a><span data-ttu-id="0c343-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c343-119">Request headers</span></span>
|<span data-ttu-id="0c343-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c343-120">Header</span></span>|<span data-ttu-id="0c343-121">値</span><span class="sxs-lookup"><span data-stu-id="0c343-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c343-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c343-122">Authorization</span></span>|<span data-ttu-id="0c343-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0c343-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c343-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0c343-124">Accept</span></span>|<span data-ttu-id="0c343-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c343-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c343-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0c343-126">Request body</span></span>
<span data-ttu-id="0c343-127">要求本文で、 [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0c343-127">In the request body, supply a JSON representation for the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

<span data-ttu-id="0c343-128">次の表に、 [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0c343-128">The following table shows the properties that are required when you create the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md).</span></span>

|<span data-ttu-id="0c343-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c343-129">Property</span></span>|<span data-ttu-id="0c343-130">型</span><span class="sxs-lookup"><span data-stu-id="0c343-130">Type</span></span>|<span data-ttu-id="0c343-131">説明</span><span class="sxs-lookup"><span data-stu-id="0c343-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c343-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="0c343-132">tenantId</span></span>|<span data-ttu-id="0c343-133">Guid</span><span class="sxs-lookup"><span data-stu-id="0c343-133">Guid</span></span>|<span data-ttu-id="0c343-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0c343-134">Not yet documented</span></span>|
|<span data-ttu-id="0c343-135">userId</span><span class="sxs-lookup"><span data-stu-id="0c343-135">userId</span></span>|<span data-ttu-id="0c343-136">Guid</span><span class="sxs-lookup"><span data-stu-id="0c343-136">Guid</span></span>|<span data-ttu-id="0c343-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0c343-137">Not yet documented</span></span>|
|<span data-ttu-id="0c343-138">拇印</span><span class="sxs-lookup"><span data-stu-id="0c343-138">thumbprint</span></span>|<span data-ttu-id="0c343-139">String</span><span class="sxs-lookup"><span data-stu-id="0c343-139">String</span></span>|<span data-ttu-id="0c343-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0c343-140">Not yet documented</span></span>|
|<span data-ttu-id="0c343-141">userUpn</span><span class="sxs-lookup"><span data-stu-id="0c343-141">userUpn</span></span>|<span data-ttu-id="0c343-142">String</span><span class="sxs-lookup"><span data-stu-id="0c343-142">String</span></span>|<span data-ttu-id="0c343-143">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0c343-143">Not yet documented</span></span>|
|<span data-ttu-id="0c343-144">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="0c343-144">encryptedPfxBlob</span></span>|<span data-ttu-id="0c343-145">String</span><span class="sxs-lookup"><span data-stu-id="0c343-145">String</span></span>|<span data-ttu-id="0c343-146">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0c343-146">Not yet documented</span></span>|
|<span data-ttu-id="0c343-147">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="0c343-147">encryptedPfxPassword</span></span>|<span data-ttu-id="0c343-148">String</span><span class="sxs-lookup"><span data-stu-id="0c343-148">String</span></span>|<span data-ttu-id="0c343-149">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0c343-149">Not yet documented</span></span>|
|<span data-ttu-id="0c343-150">certStartDate</span><span class="sxs-lookup"><span data-stu-id="0c343-150">certStartDate</span></span>|<span data-ttu-id="0c343-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c343-151">DateTimeOffset</span></span>|<span data-ttu-id="0c343-152">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0c343-152">Not yet documented</span></span>|
|<span data-ttu-id="0c343-153">certExpirationDate</span><span class="sxs-lookup"><span data-stu-id="0c343-153">certExpirationDate</span></span>|<span data-ttu-id="0c343-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c343-154">DateTimeOffset</span></span>|<span data-ttu-id="0c343-155">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0c343-155">Not yet documented</span></span>|
|<span data-ttu-id="0c343-156">プロバイダー</span><span class="sxs-lookup"><span data-stu-id="0c343-156">providerName</span></span>|<span data-ttu-id="0c343-157">String</span><span class="sxs-lookup"><span data-stu-id="0c343-157">String</span></span>|<span data-ttu-id="0c343-158">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0c343-158">Not yet documented</span></span>|
|<span data-ttu-id="0c343-159">encryptionKeyName</span><span class="sxs-lookup"><span data-stu-id="0c343-159">encryptionKeyName</span></span>|<span data-ttu-id="0c343-160">String</span><span class="sxs-lookup"><span data-stu-id="0c343-160">String</span></span>|<span data-ttu-id="0c343-161">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0c343-161">Not yet documented</span></span>|
|<span data-ttu-id="0c343-162">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="0c343-162">paddingScheme</span></span>|<span data-ttu-id="0c343-163">Int32</span><span class="sxs-lookup"><span data-stu-id="0c343-163">Int32</span></span>|<span data-ttu-id="0c343-164">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0c343-164">Not yet documented</span></span>|
|<span data-ttu-id="0c343-165">status</span><span class="sxs-lookup"><span data-stu-id="0c343-165">status</span></span>|<span data-ttu-id="0c343-166">Int32</span><span class="sxs-lookup"><span data-stu-id="0c343-166">Int32</span></span>|<span data-ttu-id="0c343-167">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0c343-167">Not yet documented</span></span>|
|<span data-ttu-id="0c343-168">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="0c343-168">intendedPurpose</span></span>|<span data-ttu-id="0c343-169">Int32</span><span class="sxs-lookup"><span data-stu-id="0c343-169">Int32</span></span>|<span data-ttu-id="0c343-170">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0c343-170">Not yet documented</span></span>|
|<span data-ttu-id="0c343-171">createdTime</span><span class="sxs-lookup"><span data-stu-id="0c343-171">createdTime</span></span>|<span data-ttu-id="0c343-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c343-172">DateTimeOffset</span></span>|<span data-ttu-id="0c343-173">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0c343-173">Not yet documented</span></span>|
|<span data-ttu-id="0c343-174">isDeleted</span><span class="sxs-lookup"><span data-stu-id="0c343-174">isDeleted</span></span>|<span data-ttu-id="0c343-175">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="0c343-175">Boolean</span></span>|<span data-ttu-id="0c343-176">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0c343-176">Not yet documented</span></span>|
|<span data-ttu-id="0c343-177">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="0c343-177">lastModifiedTime</span></span>|<span data-ttu-id="0c343-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c343-178">DateTimeOffset</span></span>|<span data-ttu-id="0c343-179">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0c343-179">Not yet documented</span></span>|
|<span data-ttu-id="0c343-180">eTag</span><span class="sxs-lookup"><span data-stu-id="0c343-180">eTag</span></span>|<span data-ttu-id="0c343-181">String</span><span class="sxs-lookup"><span data-stu-id="0c343-181">String</span></span>|<span data-ttu-id="0c343-182">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0c343-182">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0c343-183">応答</span><span class="sxs-lookup"><span data-stu-id="0c343-183">Response</span></span>
<span data-ttu-id="0c343-184">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0c343-184">If successful, this method returns a `200 OK` response code and an updated [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c343-185">例</span><span class="sxs-lookup"><span data-stu-id="0c343-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c343-186">要求</span><span class="sxs-lookup"><span data-stu-id="0c343-186">Request</span></span>
<span data-ttu-id="0c343-187">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0c343-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/pfxUserCertificates/{pfxUserCertificatesId}
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

### <a name="response"></a><span data-ttu-id="0c343-188">応答</span><span class="sxs-lookup"><span data-stu-id="0c343-188">Response</span></span>
<span data-ttu-id="0c343-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0c343-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





