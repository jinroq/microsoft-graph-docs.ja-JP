---
title: EnterpriseCodeSigningCertificate の更新
description: EnterpriseCodeSigningCertificate オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 455fdd186b8be297ec4d9d2ed32c6461b34f0748
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35951996"
---
# <a name="update-enterprisecodesigningcertificate"></a><span data-ttu-id="36d2f-103">EnterpriseCodeSigningCertificate の更新</span><span class="sxs-lookup"><span data-stu-id="36d2f-103">Update enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="36d2f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36d2f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36d2f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="36d2f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36d2f-106">[EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="36d2f-106">Update the properties of a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36d2f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="36d2f-107">Prerequisites</span></span>
<span data-ttu-id="36d2f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36d2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36d2f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="36d2f-110">Permission type</span></span>|<span data-ttu-id="36d2f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="36d2f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36d2f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="36d2f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="36d2f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36d2f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="36d2f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="36d2f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36d2f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36d2f-115">Not supported.</span></span>|
|<span data-ttu-id="36d2f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="36d2f-116">Application</span></span>|<span data-ttu-id="36d2f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36d2f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36d2f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="36d2f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="36d2f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36d2f-119">Request headers</span></span>
|<span data-ttu-id="36d2f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36d2f-120">Header</span></span>|<span data-ttu-id="36d2f-121">値</span><span class="sxs-lookup"><span data-stu-id="36d2f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36d2f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="36d2f-122">Authorization</span></span>|<span data-ttu-id="36d2f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="36d2f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36d2f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="36d2f-124">Accept</span></span>|<span data-ttu-id="36d2f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="36d2f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36d2f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="36d2f-126">Request body</span></span>
<span data-ttu-id="36d2f-127">要求本文で、 [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="36d2f-127">In the request body, supply a JSON representation for the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

<span data-ttu-id="36d2f-128">次の表に、 [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="36d2f-128">The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).</span></span>

|<span data-ttu-id="36d2f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36d2f-129">Property</span></span>|<span data-ttu-id="36d2f-130">型</span><span class="sxs-lookup"><span data-stu-id="36d2f-130">Type</span></span>|<span data-ttu-id="36d2f-131">説明</span><span class="sxs-lookup"><span data-stu-id="36d2f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36d2f-132">id</span><span class="sxs-lookup"><span data-stu-id="36d2f-132">id</span></span>|<span data-ttu-id="36d2f-133">文字列</span><span class="sxs-lookup"><span data-stu-id="36d2f-133">String</span></span>|<span data-ttu-id="36d2f-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="36d2f-134">The key of the entity.</span></span>|
|<span data-ttu-id="36d2f-135">content</span><span class="sxs-lookup"><span data-stu-id="36d2f-135">content</span></span>|<span data-ttu-id="36d2f-136">Binary</span><span class="sxs-lookup"><span data-stu-id="36d2f-136">Binary</span></span>|<span data-ttu-id="36d2f-137">未加工のデータ形式の Windows エンタープライズコード署名証明書。</span><span class="sxs-lookup"><span data-stu-id="36d2f-137">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="36d2f-138">status</span><span class="sxs-lookup"><span data-stu-id="36d2f-138">status</span></span>|[<span data-ttu-id="36d2f-139">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="36d2f-139">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="36d2f-140">証明書の状態がプロビジョニングされているか、プロビジョニングされていません。</span><span class="sxs-lookup"><span data-stu-id="36d2f-140">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="36d2f-141">可能な値は、`notProvisioned`、`provisioned` です。</span><span class="sxs-lookup"><span data-stu-id="36d2f-141">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="36d2f-142">subjectName</span><span class="sxs-lookup"><span data-stu-id="36d2f-142">subjectName</span></span>|<span data-ttu-id="36d2f-143">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="36d2f-143">String</span></span>|<span data-ttu-id="36d2f-144">証明書のサブジェクト名。</span><span class="sxs-lookup"><span data-stu-id="36d2f-144">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="36d2f-145">subject</span><span class="sxs-lookup"><span data-stu-id="36d2f-145">subject</span></span>|<span data-ttu-id="36d2f-146">String</span><span class="sxs-lookup"><span data-stu-id="36d2f-146">String</span></span>|<span data-ttu-id="36d2f-147">証明書のサブジェクトの値。</span><span class="sxs-lookup"><span data-stu-id="36d2f-147">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="36d2f-148">issuerName</span><span class="sxs-lookup"><span data-stu-id="36d2f-148">issuerName</span></span>|<span data-ttu-id="36d2f-149">String</span><span class="sxs-lookup"><span data-stu-id="36d2f-149">String</span></span>|<span data-ttu-id="36d2f-150">証明書の発行者名。</span><span class="sxs-lookup"><span data-stu-id="36d2f-150">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="36d2f-151">会社</span><span class="sxs-lookup"><span data-stu-id="36d2f-151">issuer</span></span>|<span data-ttu-id="36d2f-152">String</span><span class="sxs-lookup"><span data-stu-id="36d2f-152">String</span></span>|<span data-ttu-id="36d2f-153">証明書の発行者の値。</span><span class="sxs-lookup"><span data-stu-id="36d2f-153">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="36d2f-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="36d2f-154">expirationDateTime</span></span>|<span data-ttu-id="36d2f-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36d2f-155">DateTimeOffset</span></span>|<span data-ttu-id="36d2f-156">証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="36d2f-156">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="36d2f-157">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="36d2f-157">uploadDateTime</span></span>|<span data-ttu-id="36d2f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36d2f-158">DateTimeOffset</span></span>|<span data-ttu-id="36d2f-159">CodeSigning Cert がアップロードされたときの日付時刻。</span><span class="sxs-lookup"><span data-stu-id="36d2f-159">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="36d2f-160">応答</span><span class="sxs-lookup"><span data-stu-id="36d2f-160">Response</span></span>
<span data-ttu-id="36d2f-161">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="36d2f-161">If successful, this method returns a `200 OK` response code and an updated [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36d2f-162">例</span><span class="sxs-lookup"><span data-stu-id="36d2f-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="36d2f-163">要求</span><span class="sxs-lookup"><span data-stu-id="36d2f-163">Request</span></span>
<span data-ttu-id="36d2f-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="36d2f-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="36d2f-165">応答</span><span class="sxs-lookup"><span data-stu-id="36d2f-165">Response</span></span>
<span data-ttu-id="36d2f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="36d2f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





