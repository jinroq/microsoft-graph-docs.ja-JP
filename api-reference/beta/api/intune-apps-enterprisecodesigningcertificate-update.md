---
title: EnterpriseCodeSigningCertificate を更新します。
description: EnterpriseCodeSigningCertificate オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5133f5dffa98834ce44849c6b18c73cc19732756
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955115"
---
# <a name="update-enterprisecodesigningcertificate"></a><span data-ttu-id="04453-103">EnterpriseCodeSigningCertificate を更新します。</span><span class="sxs-lookup"><span data-stu-id="04453-103">Update enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="04453-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="04453-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04453-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04453-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04453-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="04453-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04453-107">[EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="04453-107">Update the properties of a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="04453-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="04453-108">Prerequisites</span></span>
<span data-ttu-id="04453-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04453-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04453-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04453-111">Permission type</span></span>|<span data-ttu-id="04453-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="04453-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04453-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04453-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04453-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04453-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04453-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04453-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04453-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04453-116">Not supported.</span></span>|
|<span data-ttu-id="04453-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04453-117">Application</span></span>|<span data-ttu-id="04453-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04453-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04453-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04453-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="04453-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04453-120">Request headers</span></span>
|<span data-ttu-id="04453-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04453-121">Header</span></span>|<span data-ttu-id="04453-122">値</span><span class="sxs-lookup"><span data-stu-id="04453-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04453-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="04453-123">Authorization</span></span>|<span data-ttu-id="04453-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="04453-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04453-125">Accept</span><span class="sxs-lookup"><span data-stu-id="04453-125">Accept</span></span>|<span data-ttu-id="04453-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04453-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04453-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="04453-127">Request body</span></span>
<span data-ttu-id="04453-128">要求の本文に[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="04453-128">In the request body, supply a JSON representation for the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

<span data-ttu-id="04453-129">[EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="04453-129">The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).</span></span>

|<span data-ttu-id="04453-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04453-130">Property</span></span>|<span data-ttu-id="04453-131">種類</span><span class="sxs-lookup"><span data-stu-id="04453-131">Type</span></span>|<span data-ttu-id="04453-132">説明</span><span class="sxs-lookup"><span data-stu-id="04453-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04453-133">ID</span><span class="sxs-lookup"><span data-stu-id="04453-133">id</span></span>|<span data-ttu-id="04453-134">String</span><span class="sxs-lookup"><span data-stu-id="04453-134">String</span></span>|<span data-ttu-id="04453-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="04453-135">The key of the entity.</span></span>|
|<span data-ttu-id="04453-136">content</span><span class="sxs-lookup"><span data-stu-id="04453-136">content</span></span>|<span data-ttu-id="04453-137">Binary</span><span class="sxs-lookup"><span data-stu-id="04453-137">Binary</span></span>|<span data-ttu-id="04453-138">生データの形式で Windows エンタープライズ コード署名証明書。</span><span class="sxs-lookup"><span data-stu-id="04453-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="04453-139">status</span><span class="sxs-lookup"><span data-stu-id="04453-139">status</span></span>|[<span data-ttu-id="04453-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="04453-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="04453-141">証明書の状態は、準備または準備されていません。</span><span class="sxs-lookup"><span data-stu-id="04453-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="04453-142">使用可能な値は、`notProvisioned`、`provisioned` です。</span><span class="sxs-lookup"><span data-stu-id="04453-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="04453-143">subjectName</span><span class="sxs-lookup"><span data-stu-id="04453-143">subjectName</span></span>|<span data-ttu-id="04453-144">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="04453-144">String</span></span>|<span data-ttu-id="04453-145">証明書のサブジェクト名。</span><span class="sxs-lookup"><span data-stu-id="04453-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="04453-146">subject</span><span class="sxs-lookup"><span data-stu-id="04453-146">subject</span></span>|<span data-ttu-id="04453-147">String</span><span class="sxs-lookup"><span data-stu-id="04453-147">String</span></span>|<span data-ttu-id="04453-148">証明書のサブジェクト値。</span><span class="sxs-lookup"><span data-stu-id="04453-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="04453-149">issuerName</span><span class="sxs-lookup"><span data-stu-id="04453-149">issuerName</span></span>|<span data-ttu-id="04453-150">String</span><span class="sxs-lookup"><span data-stu-id="04453-150">String</span></span>|<span data-ttu-id="04453-151">証明書の発行者の名前です。</span><span class="sxs-lookup"><span data-stu-id="04453-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="04453-152">発行者</span><span class="sxs-lookup"><span data-stu-id="04453-152">issuer</span></span>|<span data-ttu-id="04453-153">String</span><span class="sxs-lookup"><span data-stu-id="04453-153">String</span></span>|<span data-ttu-id="04453-154">証明書の発行者の値です。</span><span class="sxs-lookup"><span data-stu-id="04453-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="04453-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="04453-155">expirationDateTime</span></span>|<span data-ttu-id="04453-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04453-156">DateTimeOffset</span></span>|<span data-ttu-id="04453-157">証明書の有効期限日です。</span><span class="sxs-lookup"><span data-stu-id="04453-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="04453-158">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="04453-158">uploadDateTime</span></span>|<span data-ttu-id="04453-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04453-159">DateTimeOffset</span></span>|<span data-ttu-id="04453-160">コード署名証明書のアップロード時の日時です。</span><span class="sxs-lookup"><span data-stu-id="04453-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="04453-161">応答</span><span class="sxs-lookup"><span data-stu-id="04453-161">Response</span></span>
<span data-ttu-id="04453-162">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="04453-162">If successful, this method returns a `200 OK` response code and an updated [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04453-163">例</span><span class="sxs-lookup"><span data-stu-id="04453-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="04453-164">要求</span><span class="sxs-lookup"><span data-stu-id="04453-164">Request</span></span>
<span data-ttu-id="04453-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04453-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="04453-166">応答</span><span class="sxs-lookup"><span data-stu-id="04453-166">Response</span></span>
<span data-ttu-id="04453-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="04453-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





