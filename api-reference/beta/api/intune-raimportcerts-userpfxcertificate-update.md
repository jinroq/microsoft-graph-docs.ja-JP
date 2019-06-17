---
title: UserPFXCertificate の更新
description: UserPFXCertificate オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ce7aa967f62010f335c75b0211794f733de8e1f5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988756"
---
# <a name="update-userpfxcertificate"></a><span data-ttu-id="bc274-103">UserPFXCertificate の更新</span><span class="sxs-lookup"><span data-stu-id="bc274-103">Update userPFXCertificate</span></span>

> <span data-ttu-id="bc274-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc274-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc274-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bc274-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc274-106">[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bc274-106">Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc274-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="bc274-107">Prerequisites</span></span>
<span data-ttu-id="bc274-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bc274-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc274-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bc274-110">Permission type</span></span>|<span data-ttu-id="bc274-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bc274-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc274-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bc274-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bc274-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc274-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc274-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bc274-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc274-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc274-115">Not supported.</span></span>|
|<span data-ttu-id="bc274-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bc274-116">Application</span></span>|<span data-ttu-id="bc274-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc274-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc274-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bc274-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="bc274-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bc274-119">Request headers</span></span>
|<span data-ttu-id="bc274-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bc274-120">Header</span></span>|<span data-ttu-id="bc274-121">値</span><span class="sxs-lookup"><span data-stu-id="bc274-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc274-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc274-122">Authorization</span></span>|<span data-ttu-id="bc274-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="bc274-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc274-124">承諾</span><span class="sxs-lookup"><span data-stu-id="bc274-124">Accept</span></span>|<span data-ttu-id="bc274-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bc274-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc274-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bc274-126">Request body</span></span>
<span data-ttu-id="bc274-127">要求本文で、 [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bc274-127">In the request body, supply a JSON representation for the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

<span data-ttu-id="bc274-128">次の表に、 [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bc274-128">The following table shows the properties that are required when you create the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>

|<span data-ttu-id="bc274-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc274-129">Property</span></span>|<span data-ttu-id="bc274-130">型</span><span class="sxs-lookup"><span data-stu-id="bc274-130">Type</span></span>|<span data-ttu-id="bc274-131">説明</span><span class="sxs-lookup"><span data-stu-id="bc274-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc274-132">id</span><span class="sxs-lookup"><span data-stu-id="bc274-132">id</span></span>|<span data-ttu-id="bc274-133">文字列</span><span class="sxs-lookup"><span data-stu-id="bc274-133">String</span></span>|<span data-ttu-id="bc274-134">PFX 証明書の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="bc274-134">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="bc274-135">拇印</span><span class="sxs-lookup"><span data-stu-id="bc274-135">thumbprint</span></span>|<span data-ttu-id="bc274-136">String</span><span class="sxs-lookup"><span data-stu-id="bc274-136">String</span></span>|<span data-ttu-id="bc274-137">PFX 証明書の SHA-1 拇印。</span><span class="sxs-lookup"><span data-stu-id="bc274-137">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="bc274-138">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="bc274-138">intendedPurpose</span></span>|[<span data-ttu-id="bc274-139">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="bc274-139">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="bc274-140">展開の観点から見た証明書の目的。</span><span class="sxs-lookup"><span data-stu-id="bc274-140">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="bc274-141">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="bc274-141">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="bc274-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bc274-142">userPrincipalName</span></span>|<span data-ttu-id="bc274-143">String</span><span class="sxs-lookup"><span data-stu-id="bc274-143">String</span></span>|<span data-ttu-id="bc274-144">PFX 証明書のユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="bc274-144">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="bc274-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bc274-145">startDateTime</span></span>|<span data-ttu-id="bc274-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc274-146">DateTimeOffset</span></span>|<span data-ttu-id="bc274-147">証明書の有効期間の開始日/時刻。</span><span class="sxs-lookup"><span data-stu-id="bc274-147">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="bc274-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bc274-148">expirationDateTime</span></span>|<span data-ttu-id="bc274-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc274-149">DateTimeOffset</span></span>|<span data-ttu-id="bc274-150">証明書の有効期限の日付/時刻。</span><span class="sxs-lookup"><span data-stu-id="bc274-150">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="bc274-151">プロバイダー</span><span class="sxs-lookup"><span data-stu-id="bc274-151">providerName</span></span>|<span data-ttu-id="bc274-152">String</span><span class="sxs-lookup"><span data-stu-id="bc274-152">String</span></span>|<span data-ttu-id="bc274-153">この blob を暗号化するために使用される暗号化プロバイダー。</span><span class="sxs-lookup"><span data-stu-id="bc274-153">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="bc274-154">keyName</span><span class="sxs-lookup"><span data-stu-id="bc274-154">keyName</span></span>|<span data-ttu-id="bc274-155">String</span><span class="sxs-lookup"><span data-stu-id="bc274-155">String</span></span>|<span data-ttu-id="bc274-156">Blob の暗号化に使用された (プロバイダー内の) キーの名前。</span><span class="sxs-lookup"><span data-stu-id="bc274-156">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="bc274-157">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="bc274-157">paddingScheme</span></span>|[<span data-ttu-id="bc274-158">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="bc274-158">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="bc274-159">暗号化/復号化時にプロバイダーによって使用されるパディング方式。</span><span class="sxs-lookup"><span data-stu-id="bc274-159">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="bc274-160">使用可能な値: `none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。</span><span class="sxs-lookup"><span data-stu-id="bc274-160">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="bc274-161">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="bc274-161">encryptedPfxBlob</span></span>|<span data-ttu-id="bc274-162">Binary</span><span class="sxs-lookup"><span data-stu-id="bc274-162">Binary</span></span>|<span data-ttu-id="bc274-163">暗号化された PFX blob。</span><span class="sxs-lookup"><span data-stu-id="bc274-163">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="bc274-164">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="bc274-164">encryptedPfxPassword</span></span>|<span data-ttu-id="bc274-165">String</span><span class="sxs-lookup"><span data-stu-id="bc274-165">String</span></span>|<span data-ttu-id="bc274-166">暗号化された PFX パスワード。</span><span class="sxs-lookup"><span data-stu-id="bc274-166">Encrypted PFX password.</span></span>|
|<span data-ttu-id="bc274-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc274-167">createdDateTime</span></span>|<span data-ttu-id="bc274-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc274-168">DateTimeOffset</span></span>|<span data-ttu-id="bc274-169">この PFX 証明書がインポートされた日付/時刻です。</span><span class="sxs-lookup"><span data-stu-id="bc274-169">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="bc274-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc274-170">lastModifiedDateTime</span></span>|<span data-ttu-id="bc274-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc274-171">DateTimeOffset</span></span>|<span data-ttu-id="bc274-172">この PFX 証明書が最後に変更された日付/時刻。</span><span class="sxs-lookup"><span data-stu-id="bc274-172">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="bc274-173">応答</span><span class="sxs-lookup"><span data-stu-id="bc274-173">Response</span></span>
<span data-ttu-id="bc274-174">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bc274-174">If successful, this method returns a `200 OK` response code and an updated [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc274-175">例</span><span class="sxs-lookup"><span data-stu-id="bc274-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc274-176">要求</span><span class="sxs-lookup"><span data-stu-id="bc274-176">Request</span></span>
<span data-ttu-id="bc274-177">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bc274-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates/{userPFXCertificateId}
Content-type: application/json
Content-length: 523

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
  "encryptedPfxPassword": "Encrypted Pfx Password value"
}
```

### <a name="response"></a><span data-ttu-id="bc274-178">応答</span><span class="sxs-lookup"><span data-stu-id="bc274-178">Response</span></span>
<span data-ttu-id="bc274-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bc274-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





