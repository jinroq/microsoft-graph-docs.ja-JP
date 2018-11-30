---
title: UserPFXCertificate を作成します。
description: 新しい userPFXCertificate オブジェクトを作成します。
ms.openlocfilehash: 3f9ec2d223911191ea9e137bb2d50b5f5d03bb73
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071228"
---
# <a name="create-userpfxcertificate"></a><span data-ttu-id="4545c-103">UserPFXCertificate を作成します。</span><span class="sxs-lookup"><span data-stu-id="4545c-103">Create userPFXCertificate</span></span>

> <span data-ttu-id="4545c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4545c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4545c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4545c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4545c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4545c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4545c-107">新しい[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4545c-107">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4545c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4545c-108">Prerequisites</span></span>
<span data-ttu-id="4545c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4545c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4545c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4545c-111">Permission type</span></span>|<span data-ttu-id="4545c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4545c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4545c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4545c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4545c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4545c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4545c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4545c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4545c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4545c-116">Not supported.</span></span>|
|<span data-ttu-id="4545c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4545c-117">Application</span></span>|<span data-ttu-id="4545c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4545c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4545c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4545c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="4545c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4545c-120">Request headers</span></span>
|<span data-ttu-id="4545c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4545c-121">Header</span></span>|<span data-ttu-id="4545c-122">値</span><span class="sxs-lookup"><span data-stu-id="4545c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4545c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4545c-123">Authorization</span></span>|<span data-ttu-id="4545c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4545c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4545c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4545c-125">Accept</span></span>|<span data-ttu-id="4545c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4545c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4545c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4545c-127">Request body</span></span>
<span data-ttu-id="4545c-128">要求の本文に userPFXCertificate オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="4545c-128">In the request body, supply a JSON representation for the userPFXCertificate object.</span></span>

<span data-ttu-id="4545c-129">次の表は、userPFXCertificate を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4545c-129">The following table shows the properties that are required when you create the userPFXCertificate.</span></span>

|<span data-ttu-id="4545c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4545c-130">Property</span></span>|<span data-ttu-id="4545c-131">型</span><span class="sxs-lookup"><span data-stu-id="4545c-131">Type</span></span>|<span data-ttu-id="4545c-132">説明</span><span class="sxs-lookup"><span data-stu-id="4545c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4545c-133">id</span><span class="sxs-lookup"><span data-stu-id="4545c-133">id</span></span>|<span data-ttu-id="4545c-134">String</span><span class="sxs-lookup"><span data-stu-id="4545c-134">String</span></span>|<span data-ttu-id="4545c-135">PFX 証明書の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="4545c-135">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="4545c-136">拇印</span><span class="sxs-lookup"><span data-stu-id="4545c-136">thumbprint</span></span>|<span data-ttu-id="4545c-137">String</span><span class="sxs-lookup"><span data-stu-id="4545c-137">String</span></span>|<span data-ttu-id="4545c-138">PFX 証明書の拇印を sha-1 です。</span><span class="sxs-lookup"><span data-stu-id="4545c-138">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="4545c-139">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="4545c-139">intendedPurpose</span></span>|[<span data-ttu-id="4545c-140">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="4545c-140">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="4545c-141">証明書からのポイントからのビューの展開の目的のものです。</span><span class="sxs-lookup"><span data-stu-id="4545c-141">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="4545c-142">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="4545c-142">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="4545c-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4545c-143">userPrincipalName</span></span>|<span data-ttu-id="4545c-144">String</span><span class="sxs-lookup"><span data-stu-id="4545c-144">String</span></span>|<span data-ttu-id="4545c-145">PFX 証明書のユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="4545c-145">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="4545c-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4545c-146">startDateTime</span></span>|<span data-ttu-id="4545c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4545c-147">DateTimeOffset</span></span>|<span data-ttu-id="4545c-148">証明書の有効性は、日付と時刻を開始します。</span><span class="sxs-lookup"><span data-stu-id="4545c-148">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="4545c-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4545c-149">expirationDateTime</span></span>|<span data-ttu-id="4545c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4545c-150">DateTimeOffset</span></span>|<span data-ttu-id="4545c-151">証明書の有効期限切れ日時です。</span><span class="sxs-lookup"><span data-stu-id="4545c-151">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="4545c-152">プロバイダー</span><span class="sxs-lookup"><span data-stu-id="4545c-152">providerName</span></span>|<span data-ttu-id="4545c-153">String</span><span class="sxs-lookup"><span data-stu-id="4545c-153">String</span></span>|<span data-ttu-id="4545c-154">暗号サービス プロバイダーがこの blob の暗号化に使用します。</span><span class="sxs-lookup"><span data-stu-id="4545c-154">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="4545c-155">キー名</span><span class="sxs-lookup"><span data-stu-id="4545c-155">keyName</span></span>|<span data-ttu-id="4545c-156">String</span><span class="sxs-lookup"><span data-stu-id="4545c-156">String</span></span>|<span data-ttu-id="4545c-157">(プロバイダー) 内のキーの名前が blob の暗号化に使用します。</span><span class="sxs-lookup"><span data-stu-id="4545c-157">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="4545c-158">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="4545c-158">paddingScheme</span></span>|[<span data-ttu-id="4545c-159">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="4545c-159">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="4545c-160">暗号化/復号化中に、プロバイダーによって使用されるスキームをパディングします。</span><span class="sxs-lookup"><span data-stu-id="4545c-160">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="4545c-161">使用可能な値: `none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。</span><span class="sxs-lookup"><span data-stu-id="4545c-161">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="4545c-162">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="4545c-162">encryptedPfxBlob</span></span>|<span data-ttu-id="4545c-163">バイナリ</span><span class="sxs-lookup"><span data-stu-id="4545c-163">Binary</span></span>|<span data-ttu-id="4545c-164">PFX の暗号化された blob です。</span><span class="sxs-lookup"><span data-stu-id="4545c-164">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="4545c-165">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="4545c-165">encryptedPfxPassword</span></span>|<span data-ttu-id="4545c-166">String</span><span class="sxs-lookup"><span data-stu-id="4545c-166">String</span></span>|<span data-ttu-id="4545c-167">PFX パスワードを暗号化します。</span><span class="sxs-lookup"><span data-stu-id="4545c-167">Encrypted PFX password.</span></span>|
|<span data-ttu-id="4545c-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4545c-168">createdDateTime</span></span>|<span data-ttu-id="4545c-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4545c-169">DateTimeOffset</span></span>|<span data-ttu-id="4545c-170">PFX 証明書がインポートされたときに、日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="4545c-170">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="4545c-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4545c-171">lastModifiedDateTime</span></span>|<span data-ttu-id="4545c-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4545c-172">DateTimeOffset</span></span>|<span data-ttu-id="4545c-173">PFX 証明書が最後に修正された日時です。</span><span class="sxs-lookup"><span data-stu-id="4545c-173">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="4545c-174">応答</span><span class="sxs-lookup"><span data-stu-id="4545c-174">Response</span></span>
<span data-ttu-id="4545c-175">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4545c-175">If successful, this method returns a `201 Created` response code and a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4545c-176">例</span><span class="sxs-lookup"><span data-stu-id="4545c-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="4545c-177">要求</span><span class="sxs-lookup"><span data-stu-id="4545c-177">Request</span></span>
<span data-ttu-id="4545c-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4545c-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
Content-type: application/json
Content-length: 587

{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "thumbprint": "Thumbprint value",
  "intendedPurpose": "smimeEncryption",
  "userPrincipalName": "User Principal Name value",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "providerName": "Provider Name value",
  "keyName": "Key Name value",
  "paddingScheme": "pkcs1",
  "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="4545c-179">応答</span><span class="sxs-lookup"><span data-stu-id="4545c-179">Response</span></span>
<span data-ttu-id="4545c-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4545c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 695

{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "id": "045c159b-159b-045c-9b15-5c049b155c04",
  "thumbprint": "Thumbprint value",
  "intendedPurpose": "smimeEncryption",
  "userPrincipalName": "User Principal Name value",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "providerName": "Provider Name value",
  "keyName": "Key Name value",
  "paddingScheme": "pkcs1",
  "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





