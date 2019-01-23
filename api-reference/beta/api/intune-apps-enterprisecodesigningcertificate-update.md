---
title: EnterpriseCodeSigningCertificate を更新します。
description: EnterpriseCodeSigningCertificate オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7541f75a12dc39dcf80dfcc0df06aef5d2c551a7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406578"
---
# <a name="update-enterprisecodesigningcertificate"></a><span data-ttu-id="f8c69-103">EnterpriseCodeSigningCertificate を更新します。</span><span class="sxs-lookup"><span data-stu-id="f8c69-103">Update enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="f8c69-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f8c69-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f8c69-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8c69-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8c69-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f8c69-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8c69-107">[EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f8c69-107">Update the properties of a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8c69-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f8c69-108">Prerequisites</span></span>
<span data-ttu-id="f8c69-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f8c69-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f8c69-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f8c69-111">Permission type</span></span>|<span data-ttu-id="f8c69-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f8c69-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8c69-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f8c69-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8c69-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8c69-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f8c69-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f8c69-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8c69-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8c69-116">Not supported.</span></span>|
|<span data-ttu-id="f8c69-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f8c69-117">Application</span></span>|<span data-ttu-id="f8c69-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8c69-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8c69-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f8c69-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="f8c69-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f8c69-120">Request headers</span></span>
|<span data-ttu-id="f8c69-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f8c69-121">Header</span></span>|<span data-ttu-id="f8c69-122">値</span><span class="sxs-lookup"><span data-stu-id="f8c69-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8c69-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8c69-123">Authorization</span></span>|<span data-ttu-id="f8c69-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f8c69-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8c69-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f8c69-125">Accept</span></span>|<span data-ttu-id="f8c69-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8c69-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8c69-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f8c69-127">Request body</span></span>
<span data-ttu-id="f8c69-128">要求の本文に[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="f8c69-128">In the request body, supply a JSON representation for the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

<span data-ttu-id="f8c69-129">[EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="f8c69-129">The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).</span></span>

|<span data-ttu-id="f8c69-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8c69-130">Property</span></span>|<span data-ttu-id="f8c69-131">型</span><span class="sxs-lookup"><span data-stu-id="f8c69-131">Type</span></span>|<span data-ttu-id="f8c69-132">説明</span><span class="sxs-lookup"><span data-stu-id="f8c69-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8c69-133">id</span><span class="sxs-lookup"><span data-stu-id="f8c69-133">id</span></span>|<span data-ttu-id="f8c69-134">String</span><span class="sxs-lookup"><span data-stu-id="f8c69-134">String</span></span>|<span data-ttu-id="f8c69-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f8c69-135">The key of the entity.</span></span>|
|<span data-ttu-id="f8c69-136">content</span><span class="sxs-lookup"><span data-stu-id="f8c69-136">content</span></span>|<span data-ttu-id="f8c69-137">Binary</span><span class="sxs-lookup"><span data-stu-id="f8c69-137">Binary</span></span>|<span data-ttu-id="f8c69-138">生データの形式で Windows エンタープライズ コード署名証明書。</span><span class="sxs-lookup"><span data-stu-id="f8c69-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="f8c69-139">status</span><span class="sxs-lookup"><span data-stu-id="f8c69-139">status</span></span>|[<span data-ttu-id="f8c69-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="f8c69-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="f8c69-141">証明書の状態は、準備または準備されていません。</span><span class="sxs-lookup"><span data-stu-id="f8c69-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="f8c69-142">使用可能な値は、`notProvisioned`、`provisioned` です。</span><span class="sxs-lookup"><span data-stu-id="f8c69-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="f8c69-143">subjectName</span><span class="sxs-lookup"><span data-stu-id="f8c69-143">subjectName</span></span>|<span data-ttu-id="f8c69-144">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f8c69-144">String</span></span>|<span data-ttu-id="f8c69-145">証明書のサブジェクト名。</span><span class="sxs-lookup"><span data-stu-id="f8c69-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="f8c69-146">subject</span><span class="sxs-lookup"><span data-stu-id="f8c69-146">subject</span></span>|<span data-ttu-id="f8c69-147">String</span><span class="sxs-lookup"><span data-stu-id="f8c69-147">String</span></span>|<span data-ttu-id="f8c69-148">証明書のサブジェクト値。</span><span class="sxs-lookup"><span data-stu-id="f8c69-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="f8c69-149">issuerName</span><span class="sxs-lookup"><span data-stu-id="f8c69-149">issuerName</span></span>|<span data-ttu-id="f8c69-150">String</span><span class="sxs-lookup"><span data-stu-id="f8c69-150">String</span></span>|<span data-ttu-id="f8c69-151">証明書の発行者の名前です。</span><span class="sxs-lookup"><span data-stu-id="f8c69-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="f8c69-152">発行者</span><span class="sxs-lookup"><span data-stu-id="f8c69-152">issuer</span></span>|<span data-ttu-id="f8c69-153">String</span><span class="sxs-lookup"><span data-stu-id="f8c69-153">String</span></span>|<span data-ttu-id="f8c69-154">証明書の発行者の値です。</span><span class="sxs-lookup"><span data-stu-id="f8c69-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="f8c69-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f8c69-155">expirationDateTime</span></span>|<span data-ttu-id="f8c69-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8c69-156">DateTimeOffset</span></span>|<span data-ttu-id="f8c69-157">証明書の有効期限日です。</span><span class="sxs-lookup"><span data-stu-id="f8c69-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="f8c69-158">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="f8c69-158">uploadDateTime</span></span>|<span data-ttu-id="f8c69-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8c69-159">DateTimeOffset</span></span>|<span data-ttu-id="f8c69-160">コード署名証明書のアップロード時の日時です。</span><span class="sxs-lookup"><span data-stu-id="f8c69-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="f8c69-161">応答</span><span class="sxs-lookup"><span data-stu-id="f8c69-161">Response</span></span>
<span data-ttu-id="f8c69-162">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f8c69-162">If successful, this method returns a `200 OK` response code and an updated [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8c69-163">例</span><span class="sxs-lookup"><span data-stu-id="f8c69-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8c69-164">要求</span><span class="sxs-lookup"><span data-stu-id="f8c69-164">Request</span></span>
<span data-ttu-id="f8c69-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f8c69-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f8c69-166">応答</span><span class="sxs-lookup"><span data-stu-id="f8c69-166">Response</span></span>
<span data-ttu-id="f8c69-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f8c69-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




