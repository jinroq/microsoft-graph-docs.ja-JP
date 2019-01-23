---
title: EnterpriseCodeSigningCertificate を作成します。
description: 新しい enterpriseCodeSigningCertificate オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e5ba50739903fce6e462f5c1a2602a4a61221eb3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402553"
---
# <a name="create-enterprisecodesigningcertificate"></a><span data-ttu-id="8bcf9-103">EnterpriseCodeSigningCertificate を作成します。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-103">Create enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="8bcf9-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8bcf9-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8bcf9-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bcf9-107">新しい[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-107">Create a new [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bcf9-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="8bcf9-108">Prerequisites</span></span>
<span data-ttu-id="8bcf9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8bcf9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8bcf9-111">Permission type</span></span>|<span data-ttu-id="8bcf9-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8bcf9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bcf9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8bcf9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8bcf9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bcf9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8bcf9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8bcf9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bcf9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-116">Not supported.</span></span>|
|<span data-ttu-id="8bcf9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8bcf9-117">Application</span></span>|<span data-ttu-id="8bcf9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bcf9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8bcf9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="8bcf9-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8bcf9-120">Request headers</span></span>
|<span data-ttu-id="8bcf9-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8bcf9-121">Header</span></span>|<span data-ttu-id="8bcf9-122">値</span><span class="sxs-lookup"><span data-stu-id="8bcf9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bcf9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bcf9-123">Authorization</span></span>|<span data-ttu-id="8bcf9-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bcf9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8bcf9-125">Accept</span></span>|<span data-ttu-id="8bcf9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8bcf9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bcf9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8bcf9-127">Request body</span></span>
<span data-ttu-id="8bcf9-128">要求の本文に enterpriseCodeSigningCertificate オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-128">In the request body, supply a JSON representation for the enterpriseCodeSigningCertificate object.</span></span>

<span data-ttu-id="8bcf9-129">次の表は、enterpriseCodeSigningCertificate を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-129">The following table shows the properties that are required when you create the enterpriseCodeSigningCertificate.</span></span>

|<span data-ttu-id="8bcf9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8bcf9-130">Property</span></span>|<span data-ttu-id="8bcf9-131">型</span><span class="sxs-lookup"><span data-stu-id="8bcf9-131">Type</span></span>|<span data-ttu-id="8bcf9-132">説明</span><span class="sxs-lookup"><span data-stu-id="8bcf9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bcf9-133">id</span><span class="sxs-lookup"><span data-stu-id="8bcf9-133">id</span></span>|<span data-ttu-id="8bcf9-134">String</span><span class="sxs-lookup"><span data-stu-id="8bcf9-134">String</span></span>|<span data-ttu-id="8bcf9-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-135">The key of the entity.</span></span>|
|<span data-ttu-id="8bcf9-136">content</span><span class="sxs-lookup"><span data-stu-id="8bcf9-136">content</span></span>|<span data-ttu-id="8bcf9-137">Binary</span><span class="sxs-lookup"><span data-stu-id="8bcf9-137">Binary</span></span>|<span data-ttu-id="8bcf9-138">生データの形式で Windows エンタープライズ コード署名証明書。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="8bcf9-139">status</span><span class="sxs-lookup"><span data-stu-id="8bcf9-139">status</span></span>|[<span data-ttu-id="8bcf9-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="8bcf9-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="8bcf9-141">証明書の状態は、準備または準備されていません。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="8bcf9-142">使用可能な値は、`notProvisioned`、`provisioned` です。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="8bcf9-143">subjectName</span><span class="sxs-lookup"><span data-stu-id="8bcf9-143">subjectName</span></span>|<span data-ttu-id="8bcf9-144">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8bcf9-144">String</span></span>|<span data-ttu-id="8bcf9-145">証明書のサブジェクト名。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="8bcf9-146">subject</span><span class="sxs-lookup"><span data-stu-id="8bcf9-146">subject</span></span>|<span data-ttu-id="8bcf9-147">String</span><span class="sxs-lookup"><span data-stu-id="8bcf9-147">String</span></span>|<span data-ttu-id="8bcf9-148">証明書のサブジェクト値。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="8bcf9-149">issuerName</span><span class="sxs-lookup"><span data-stu-id="8bcf9-149">issuerName</span></span>|<span data-ttu-id="8bcf9-150">String</span><span class="sxs-lookup"><span data-stu-id="8bcf9-150">String</span></span>|<span data-ttu-id="8bcf9-151">証明書の発行者の名前です。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="8bcf9-152">発行者</span><span class="sxs-lookup"><span data-stu-id="8bcf9-152">issuer</span></span>|<span data-ttu-id="8bcf9-153">String</span><span class="sxs-lookup"><span data-stu-id="8bcf9-153">String</span></span>|<span data-ttu-id="8bcf9-154">証明書の発行者の値です。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="8bcf9-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8bcf9-155">expirationDateTime</span></span>|<span data-ttu-id="8bcf9-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bcf9-156">DateTimeOffset</span></span>|<span data-ttu-id="8bcf9-157">証明書の有効期限日です。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="8bcf9-158">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="8bcf9-158">uploadDateTime</span></span>|<span data-ttu-id="8bcf9-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bcf9-159">DateTimeOffset</span></span>|<span data-ttu-id="8bcf9-160">コード署名証明書のアップロード時の日時です。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="8bcf9-161">応答</span><span class="sxs-lookup"><span data-stu-id="8bcf9-161">Response</span></span>
<span data-ttu-id="8bcf9-162">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-162">If successful, this method returns a `201 Created` response code and a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bcf9-163">例</span><span class="sxs-lookup"><span data-stu-id="8bcf9-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bcf9-164">要求</span><span class="sxs-lookup"><span data-stu-id="8bcf9-164">Request</span></span>
<span data-ttu-id="8bcf9-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8bcf9-166">応答</span><span class="sxs-lookup"><span data-stu-id="8bcf9-166">Response</span></span>
<span data-ttu-id="8bcf9-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8bcf9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




