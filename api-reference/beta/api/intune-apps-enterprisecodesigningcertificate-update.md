---
title: EnterpriseCodeSigningCertificate を更新します。
description: EnterpriseCodeSigningCertificate オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5272c0ff0e18fd7200e85ff51575c10825dbf7f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829317"
---
# <a name="update-enterprisecodesigningcertificate"></a><span data-ttu-id="c0b61-103">EnterpriseCodeSigningCertificate を更新します。</span><span class="sxs-lookup"><span data-stu-id="c0b61-103">Update enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="c0b61-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c0b61-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0b61-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0b61-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0b61-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0b61-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0b61-107">[EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c0b61-107">Update the properties of a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c0b61-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c0b61-108">Prerequisites</span></span>
<span data-ttu-id="c0b61-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0b61-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0b61-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c0b61-111">Permission type</span></span>|<span data-ttu-id="c0b61-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c0b61-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0b61-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c0b61-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0b61-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0b61-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c0b61-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c0b61-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0b61-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0b61-116">Not supported.</span></span>|
|<span data-ttu-id="c0b61-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c0b61-117">Application</span></span>|<span data-ttu-id="c0b61-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0b61-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0b61-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c0b61-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="c0b61-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0b61-120">Request headers</span></span>
|<span data-ttu-id="c0b61-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0b61-121">Header</span></span>|<span data-ttu-id="c0b61-122">値</span><span class="sxs-lookup"><span data-stu-id="c0b61-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0b61-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0b61-123">Authorization</span></span>|<span data-ttu-id="c0b61-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c0b61-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0b61-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c0b61-125">Accept</span></span>|<span data-ttu-id="c0b61-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0b61-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0b61-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c0b61-127">Request body</span></span>
<span data-ttu-id="c0b61-128">要求の本文に[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0b61-128">In the request body, supply a JSON representation for the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

<span data-ttu-id="c0b61-129">[EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="c0b61-129">The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).</span></span>

|<span data-ttu-id="c0b61-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0b61-130">Property</span></span>|<span data-ttu-id="c0b61-131">種類</span><span class="sxs-lookup"><span data-stu-id="c0b61-131">Type</span></span>|<span data-ttu-id="c0b61-132">説明</span><span class="sxs-lookup"><span data-stu-id="c0b61-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0b61-133">ID</span><span class="sxs-lookup"><span data-stu-id="c0b61-133">id</span></span>|<span data-ttu-id="c0b61-134">String</span><span class="sxs-lookup"><span data-stu-id="c0b61-134">String</span></span>|<span data-ttu-id="c0b61-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c0b61-135">The key of the entity.</span></span>|
|<span data-ttu-id="c0b61-136">content</span><span class="sxs-lookup"><span data-stu-id="c0b61-136">content</span></span>|<span data-ttu-id="c0b61-137">Binary</span><span class="sxs-lookup"><span data-stu-id="c0b61-137">Binary</span></span>|<span data-ttu-id="c0b61-138">生データの形式で Windows エンタープライズ コード署名証明書。</span><span class="sxs-lookup"><span data-stu-id="c0b61-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="c0b61-139">status</span><span class="sxs-lookup"><span data-stu-id="c0b61-139">status</span></span>|[<span data-ttu-id="c0b61-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="c0b61-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="c0b61-141">証明書の状態は、準備または準備されていません。</span><span class="sxs-lookup"><span data-stu-id="c0b61-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="c0b61-142">使用可能な値は、`notProvisioned`、`provisioned` です。</span><span class="sxs-lookup"><span data-stu-id="c0b61-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="c0b61-143">subjectName</span><span class="sxs-lookup"><span data-stu-id="c0b61-143">subjectName</span></span>|<span data-ttu-id="c0b61-144">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c0b61-144">String</span></span>|<span data-ttu-id="c0b61-145">証明書のサブジェクト名。</span><span class="sxs-lookup"><span data-stu-id="c0b61-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="c0b61-146">subject</span><span class="sxs-lookup"><span data-stu-id="c0b61-146">subject</span></span>|<span data-ttu-id="c0b61-147">String</span><span class="sxs-lookup"><span data-stu-id="c0b61-147">String</span></span>|<span data-ttu-id="c0b61-148">証明書のサブジェクト値。</span><span class="sxs-lookup"><span data-stu-id="c0b61-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="c0b61-149">issuerName</span><span class="sxs-lookup"><span data-stu-id="c0b61-149">issuerName</span></span>|<span data-ttu-id="c0b61-150">String</span><span class="sxs-lookup"><span data-stu-id="c0b61-150">String</span></span>|<span data-ttu-id="c0b61-151">証明書の発行者の名前です。</span><span class="sxs-lookup"><span data-stu-id="c0b61-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="c0b61-152">発行者</span><span class="sxs-lookup"><span data-stu-id="c0b61-152">issuer</span></span>|<span data-ttu-id="c0b61-153">String</span><span class="sxs-lookup"><span data-stu-id="c0b61-153">String</span></span>|<span data-ttu-id="c0b61-154">証明書の発行者の値です。</span><span class="sxs-lookup"><span data-stu-id="c0b61-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="c0b61-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c0b61-155">expirationDateTime</span></span>|<span data-ttu-id="c0b61-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0b61-156">DateTimeOffset</span></span>|<span data-ttu-id="c0b61-157">証明書の有効期限日です。</span><span class="sxs-lookup"><span data-stu-id="c0b61-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="c0b61-158">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="c0b61-158">uploadDateTime</span></span>|<span data-ttu-id="c0b61-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0b61-159">DateTimeOffset</span></span>|<span data-ttu-id="c0b61-160">コード署名証明書のアップロード時の日時です。</span><span class="sxs-lookup"><span data-stu-id="c0b61-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="c0b61-161">応答</span><span class="sxs-lookup"><span data-stu-id="c0b61-161">Response</span></span>
<span data-ttu-id="c0b61-162">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c0b61-162">If successful, this method returns a `200 OK` response code and an updated [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0b61-163">例</span><span class="sxs-lookup"><span data-stu-id="c0b61-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="c0b61-164">要求</span><span class="sxs-lookup"><span data-stu-id="c0b61-164">Request</span></span>
<span data-ttu-id="c0b61-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c0b61-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
Content-type: application/json
Content-length: 319

{
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

### <a name="response"></a><span data-ttu-id="c0b61-166">応答</span><span class="sxs-lookup"><span data-stu-id="c0b61-166">Response</span></span>
<span data-ttu-id="c0b61-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c0b61-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





