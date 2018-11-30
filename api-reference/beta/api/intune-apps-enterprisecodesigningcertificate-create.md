---
title: EnterpriseCodeSigningCertificate を作成します。
description: 新しい enterpriseCodeSigningCertificate オブジェクトを作成します。
ms.openlocfilehash: aa5d92c22a1cd4eb91a41b26ed92f76937ce9dcd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066331"
---
# <a name="create-enterprisecodesigningcertificate"></a><span data-ttu-id="13449-103">EnterpriseCodeSigningCertificate を作成します。</span><span class="sxs-lookup"><span data-stu-id="13449-103">Create enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="13449-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="13449-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13449-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13449-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13449-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="13449-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13449-107">新しい[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="13449-107">Create a new [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="13449-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="13449-108">Prerequisites</span></span>
<span data-ttu-id="13449-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13449-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13449-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="13449-111">Permission type</span></span>|<span data-ttu-id="13449-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="13449-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13449-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="13449-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13449-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13449-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="13449-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="13449-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13449-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13449-116">Not supported.</span></span>|
|<span data-ttu-id="13449-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="13449-117">Application</span></span>|<span data-ttu-id="13449-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13449-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13449-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="13449-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="13449-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13449-120">Request headers</span></span>
|<span data-ttu-id="13449-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13449-121">Header</span></span>|<span data-ttu-id="13449-122">値</span><span class="sxs-lookup"><span data-stu-id="13449-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13449-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="13449-123">Authorization</span></span>|<span data-ttu-id="13449-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="13449-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13449-125">Accept</span><span class="sxs-lookup"><span data-stu-id="13449-125">Accept</span></span>|<span data-ttu-id="13449-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13449-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13449-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="13449-127">Request body</span></span>
<span data-ttu-id="13449-128">要求の本文に enterpriseCodeSigningCertificate オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="13449-128">In the request body, supply a JSON representation for the enterpriseCodeSigningCertificate object.</span></span>

<span data-ttu-id="13449-129">次の表は、enterpriseCodeSigningCertificate を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="13449-129">The following table shows the properties that are required when you create the enterpriseCodeSigningCertificate.</span></span>

|<span data-ttu-id="13449-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13449-130">Property</span></span>|<span data-ttu-id="13449-131">型</span><span class="sxs-lookup"><span data-stu-id="13449-131">Type</span></span>|<span data-ttu-id="13449-132">説明</span><span class="sxs-lookup"><span data-stu-id="13449-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13449-133">id</span><span class="sxs-lookup"><span data-stu-id="13449-133">id</span></span>|<span data-ttu-id="13449-134">String</span><span class="sxs-lookup"><span data-stu-id="13449-134">String</span></span>|<span data-ttu-id="13449-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="13449-135">The key of the entity.</span></span>|
|<span data-ttu-id="13449-136">content</span><span class="sxs-lookup"><span data-stu-id="13449-136">content</span></span>|<span data-ttu-id="13449-137">バイナリ</span><span class="sxs-lookup"><span data-stu-id="13449-137">Binary</span></span>|<span data-ttu-id="13449-138">生データの形式で Windows エンタープライズ コード署名証明書。</span><span class="sxs-lookup"><span data-stu-id="13449-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="13449-139">status</span><span class="sxs-lookup"><span data-stu-id="13449-139">status</span></span>|[<span data-ttu-id="13449-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="13449-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="13449-141">証明書の状態は、準備または準備されていません。</span><span class="sxs-lookup"><span data-stu-id="13449-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="13449-142">使用可能な値は、`notProvisioned`、`provisioned` です。</span><span class="sxs-lookup"><span data-stu-id="13449-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="13449-143">subjectName</span><span class="sxs-lookup"><span data-stu-id="13449-143">subjectName</span></span>|<span data-ttu-id="13449-144">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="13449-144">String</span></span>|<span data-ttu-id="13449-145">証明書のサブジェクト名。</span><span class="sxs-lookup"><span data-stu-id="13449-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="13449-146">subject</span><span class="sxs-lookup"><span data-stu-id="13449-146">subject</span></span>|<span data-ttu-id="13449-147">String</span><span class="sxs-lookup"><span data-stu-id="13449-147">String</span></span>|<span data-ttu-id="13449-148">証明書のサブジェクト値。</span><span class="sxs-lookup"><span data-stu-id="13449-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="13449-149">issuerName</span><span class="sxs-lookup"><span data-stu-id="13449-149">issuerName</span></span>|<span data-ttu-id="13449-150">String</span><span class="sxs-lookup"><span data-stu-id="13449-150">String</span></span>|<span data-ttu-id="13449-151">証明書の発行者の名前です。</span><span class="sxs-lookup"><span data-stu-id="13449-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="13449-152">発行者</span><span class="sxs-lookup"><span data-stu-id="13449-152">issuer</span></span>|<span data-ttu-id="13449-153">String</span><span class="sxs-lookup"><span data-stu-id="13449-153">String</span></span>|<span data-ttu-id="13449-154">証明書の発行者の値です。</span><span class="sxs-lookup"><span data-stu-id="13449-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="13449-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="13449-155">expirationDateTime</span></span>|<span data-ttu-id="13449-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13449-156">DateTimeOffset</span></span>|<span data-ttu-id="13449-157">証明書の有効期限日です。</span><span class="sxs-lookup"><span data-stu-id="13449-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="13449-158">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="13449-158">uploadDateTime</span></span>|<span data-ttu-id="13449-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13449-159">DateTimeOffset</span></span>|<span data-ttu-id="13449-160">コード署名証明書のアップロード時の日時です。</span><span class="sxs-lookup"><span data-stu-id="13449-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="13449-161">応答</span><span class="sxs-lookup"><span data-stu-id="13449-161">Response</span></span>
<span data-ttu-id="13449-162">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="13449-162">If successful, this method returns a `201 Created` response code and a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13449-163">例</span><span class="sxs-lookup"><span data-stu-id="13449-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="13449-164">要求</span><span class="sxs-lookup"><span data-stu-id="13449-164">Request</span></span>
<span data-ttu-id="13449-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="13449-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates
Content-type: application/json
Content-length: 390

{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```

### <a name="response"></a><span data-ttu-id="13449-166">応答</span><span class="sxs-lookup"><span data-stu-id="13449-166">Response</span></span>
<span data-ttu-id="13449-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="13449-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "id": "b20d3703-3703-b20d-0337-0db203370db2",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```





