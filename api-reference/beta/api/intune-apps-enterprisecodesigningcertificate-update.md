---
title: EnterpriseCodeSigningCertificate の更新
description: EnterpriseCodeSigningCertificate オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c2bbc568330386553c855f94498fb410c08d296
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36330931"
---
# <a name="update-enterprisecodesigningcertificate"></a><span data-ttu-id="c1959-103">EnterpriseCodeSigningCertificate の更新</span><span class="sxs-lookup"><span data-stu-id="c1959-103">Update enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="c1959-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1959-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1959-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c1959-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1959-106">[EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c1959-106">Update the properties of a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1959-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c1959-107">Prerequisites</span></span>
<span data-ttu-id="c1959-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c1959-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1959-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c1959-110">Permission type</span></span>|<span data-ttu-id="c1959-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c1959-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1959-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c1959-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1959-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1959-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c1959-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c1959-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1959-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1959-115">Not supported.</span></span>|
|<span data-ttu-id="c1959-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c1959-116">Application</span></span>|<span data-ttu-id="c1959-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1959-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1959-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c1959-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="c1959-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c1959-119">Request headers</span></span>
|<span data-ttu-id="c1959-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c1959-120">Header</span></span>|<span data-ttu-id="c1959-121">値</span><span class="sxs-lookup"><span data-stu-id="c1959-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1959-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1959-122">Authorization</span></span>|<span data-ttu-id="c1959-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c1959-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1959-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c1959-124">Accept</span></span>|<span data-ttu-id="c1959-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1959-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1959-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c1959-126">Request body</span></span>
<span data-ttu-id="c1959-127">要求本文で、 [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c1959-127">In the request body, supply a JSON representation for the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

<span data-ttu-id="c1959-128">次の表に、 [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c1959-128">The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).</span></span>

|<span data-ttu-id="c1959-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1959-129">Property</span></span>|<span data-ttu-id="c1959-130">型</span><span class="sxs-lookup"><span data-stu-id="c1959-130">Type</span></span>|<span data-ttu-id="c1959-131">説明</span><span class="sxs-lookup"><span data-stu-id="c1959-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1959-132">id</span><span class="sxs-lookup"><span data-stu-id="c1959-132">id</span></span>|<span data-ttu-id="c1959-133">文字列</span><span class="sxs-lookup"><span data-stu-id="c1959-133">String</span></span>|<span data-ttu-id="c1959-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c1959-134">The key of the entity.</span></span>|
|<span data-ttu-id="c1959-135">content</span><span class="sxs-lookup"><span data-stu-id="c1959-135">content</span></span>|<span data-ttu-id="c1959-136">Binary</span><span class="sxs-lookup"><span data-stu-id="c1959-136">Binary</span></span>|<span data-ttu-id="c1959-137">未加工のデータ形式の Windows エンタープライズコード署名証明書。</span><span class="sxs-lookup"><span data-stu-id="c1959-137">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="c1959-138">status</span><span class="sxs-lookup"><span data-stu-id="c1959-138">status</span></span>|[<span data-ttu-id="c1959-139">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="c1959-139">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="c1959-140">証明書の状態がプロビジョニングされているか、プロビジョニングされていません。</span><span class="sxs-lookup"><span data-stu-id="c1959-140">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="c1959-141">可能な値は、`notProvisioned`、`provisioned` です。</span><span class="sxs-lookup"><span data-stu-id="c1959-141">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="c1959-142">subjectName</span><span class="sxs-lookup"><span data-stu-id="c1959-142">subjectName</span></span>|<span data-ttu-id="c1959-143">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c1959-143">String</span></span>|<span data-ttu-id="c1959-144">証明書のサブジェクト名。</span><span class="sxs-lookup"><span data-stu-id="c1959-144">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="c1959-145">subject</span><span class="sxs-lookup"><span data-stu-id="c1959-145">subject</span></span>|<span data-ttu-id="c1959-146">String</span><span class="sxs-lookup"><span data-stu-id="c1959-146">String</span></span>|<span data-ttu-id="c1959-147">証明書のサブジェクトの値。</span><span class="sxs-lookup"><span data-stu-id="c1959-147">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="c1959-148">issuerName</span><span class="sxs-lookup"><span data-stu-id="c1959-148">issuerName</span></span>|<span data-ttu-id="c1959-149">String</span><span class="sxs-lookup"><span data-stu-id="c1959-149">String</span></span>|<span data-ttu-id="c1959-150">証明書の発行者名。</span><span class="sxs-lookup"><span data-stu-id="c1959-150">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="c1959-151">会社</span><span class="sxs-lookup"><span data-stu-id="c1959-151">issuer</span></span>|<span data-ttu-id="c1959-152">String</span><span class="sxs-lookup"><span data-stu-id="c1959-152">String</span></span>|<span data-ttu-id="c1959-153">証明書の発行者の値。</span><span class="sxs-lookup"><span data-stu-id="c1959-153">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="c1959-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c1959-154">expirationDateTime</span></span>|<span data-ttu-id="c1959-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1959-155">DateTimeOffset</span></span>|<span data-ttu-id="c1959-156">証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="c1959-156">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="c1959-157">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="c1959-157">uploadDateTime</span></span>|<span data-ttu-id="c1959-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1959-158">DateTimeOffset</span></span>|<span data-ttu-id="c1959-159">CodeSigning Cert がアップロードされたときの日付時刻。</span><span class="sxs-lookup"><span data-stu-id="c1959-159">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="c1959-160">応答</span><span class="sxs-lookup"><span data-stu-id="c1959-160">Response</span></span>
<span data-ttu-id="c1959-161">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c1959-161">If successful, this method returns a `200 OK` response code and an updated [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1959-162">例</span><span class="sxs-lookup"><span data-stu-id="c1959-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1959-163">要求</span><span class="sxs-lookup"><span data-stu-id="c1959-163">Request</span></span>
<span data-ttu-id="c1959-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c1959-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
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

### <a name="response"></a><span data-ttu-id="c1959-165">応答</span><span class="sxs-lookup"><span data-stu-id="c1959-165">Response</span></span>
<span data-ttu-id="c1959-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c1959-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






