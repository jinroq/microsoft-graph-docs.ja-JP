---
title: enterpriseCodeSigningCertificate を作成する
description: 新しい enterpriseCodeSigningCertificate オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6cd85a33da06395314fc30836ba6f28de00c98ba
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802080"
---
# <a name="create-enterprisecodesigningcertificate"></a><span data-ttu-id="cbcbe-103">enterpriseCodeSigningCertificate を作成する</span><span class="sxs-lookup"><span data-stu-id="cbcbe-103">Create enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="cbcbe-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbcbe-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbcbe-106">新しい[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-106">Create a new [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbcbe-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="cbcbe-107">Prerequisites</span></span>
<span data-ttu-id="cbcbe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbcbe-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cbcbe-110">Permission type</span></span>|<span data-ttu-id="cbcbe-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cbcbe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbcbe-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cbcbe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cbcbe-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbcbe-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cbcbe-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cbcbe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbcbe-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-115">Not supported.</span></span>|
|<span data-ttu-id="cbcbe-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cbcbe-116">Application</span></span>|<span data-ttu-id="cbcbe-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbcbe-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cbcbe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="cbcbe-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cbcbe-119">Request headers</span></span>
|<span data-ttu-id="cbcbe-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cbcbe-120">Header</span></span>|<span data-ttu-id="cbcbe-121">値</span><span class="sxs-lookup"><span data-stu-id="cbcbe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbcbe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbcbe-122">Authorization</span></span>|<span data-ttu-id="cbcbe-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbcbe-124">承諾</span><span class="sxs-lookup"><span data-stu-id="cbcbe-124">Accept</span></span>|<span data-ttu-id="cbcbe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cbcbe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbcbe-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cbcbe-126">Request body</span></span>
<span data-ttu-id="cbcbe-127">要求本文で、enterpriseCodeSigningCertificate オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-127">In the request body, supply a JSON representation for the enterpriseCodeSigningCertificate object.</span></span>

<span data-ttu-id="cbcbe-128">次の表に、enterpriseCodeSigningCertificate の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-128">The following table shows the properties that are required when you create the enterpriseCodeSigningCertificate.</span></span>

|<span data-ttu-id="cbcbe-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbcbe-129">Property</span></span>|<span data-ttu-id="cbcbe-130">型</span><span class="sxs-lookup"><span data-stu-id="cbcbe-130">Type</span></span>|<span data-ttu-id="cbcbe-131">説明</span><span class="sxs-lookup"><span data-stu-id="cbcbe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbcbe-132">id</span><span class="sxs-lookup"><span data-stu-id="cbcbe-132">id</span></span>|<span data-ttu-id="cbcbe-133">String</span><span class="sxs-lookup"><span data-stu-id="cbcbe-133">String</span></span>|<span data-ttu-id="cbcbe-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-134">The key of the entity.</span></span>|
|<span data-ttu-id="cbcbe-135">content</span><span class="sxs-lookup"><span data-stu-id="cbcbe-135">content</span></span>|<span data-ttu-id="cbcbe-136">Binary</span><span class="sxs-lookup"><span data-stu-id="cbcbe-136">Binary</span></span>|<span data-ttu-id="cbcbe-137">未加工のデータ形式の Windows エンタープライズコード署名証明書。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-137">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="cbcbe-138">status</span><span class="sxs-lookup"><span data-stu-id="cbcbe-138">status</span></span>|[<span data-ttu-id="cbcbe-139">certificatestatus</span><span class="sxs-lookup"><span data-stu-id="cbcbe-139">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="cbcbe-140">証明書の状態がプロビジョニングされているか、プロビジョニングされていません。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-140">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="cbcbe-141">可能な値は、`notProvisioned`、`provisioned` です。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-141">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="cbcbe-142">subjectName</span><span class="sxs-lookup"><span data-stu-id="cbcbe-142">subjectName</span></span>|<span data-ttu-id="cbcbe-143">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="cbcbe-143">String</span></span>|<span data-ttu-id="cbcbe-144">証明書のサブジェクト名。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-144">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="cbcbe-145">subject</span><span class="sxs-lookup"><span data-stu-id="cbcbe-145">subject</span></span>|<span data-ttu-id="cbcbe-146">String</span><span class="sxs-lookup"><span data-stu-id="cbcbe-146">String</span></span>|<span data-ttu-id="cbcbe-147">証明書のサブジェクトの値。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-147">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="cbcbe-148">issuerName</span><span class="sxs-lookup"><span data-stu-id="cbcbe-148">issuerName</span></span>|<span data-ttu-id="cbcbe-149">文字列</span><span class="sxs-lookup"><span data-stu-id="cbcbe-149">String</span></span>|<span data-ttu-id="cbcbe-150">証明書の発行者名。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-150">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="cbcbe-151">会社</span><span class="sxs-lookup"><span data-stu-id="cbcbe-151">issuer</span></span>|<span data-ttu-id="cbcbe-152">文字列</span><span class="sxs-lookup"><span data-stu-id="cbcbe-152">String</span></span>|<span data-ttu-id="cbcbe-153">証明書の発行者の値。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-153">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="cbcbe-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cbcbe-154">expirationDateTime</span></span>|<span data-ttu-id="cbcbe-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbcbe-155">DateTimeOffset</span></span>|<span data-ttu-id="cbcbe-156">証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-156">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="cbcbe-157">uploaddatetime</span><span class="sxs-lookup"><span data-stu-id="cbcbe-157">uploadDateTime</span></span>|<span data-ttu-id="cbcbe-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbcbe-158">DateTimeOffset</span></span>|<span data-ttu-id="cbcbe-159">CodeSigning Cert がアップロードされたときの日付時刻。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-159">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="cbcbe-160">応答</span><span class="sxs-lookup"><span data-stu-id="cbcbe-160">Response</span></span>
<span data-ttu-id="cbcbe-161">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-161">If successful, this method returns a `201 Created` response code and a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbcbe-162">例</span><span class="sxs-lookup"><span data-stu-id="cbcbe-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbcbe-163">要求</span><span class="sxs-lookup"><span data-stu-id="cbcbe-163">Request</span></span>
<span data-ttu-id="cbcbe-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cbcbe-165">応答</span><span class="sxs-lookup"><span data-stu-id="cbcbe-165">Response</span></span>
<span data-ttu-id="cbcbe-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cbcbe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





