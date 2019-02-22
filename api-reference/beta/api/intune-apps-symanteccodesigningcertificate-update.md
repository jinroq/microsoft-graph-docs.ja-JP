---
title: symantecCodeSigningCertificate の更新
description: symantecCodeSigningCertificate オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 26a56296956c3955808a308989a0ca8ded5d4ae5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168755"
---
# <a name="update-symanteccodesigningcertificate"></a><span data-ttu-id="de7be-103">symantecCodeSigningCertificate の更新</span><span class="sxs-lookup"><span data-stu-id="de7be-103">Update symantecCodeSigningCertificate</span></span>

> <span data-ttu-id="de7be-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de7be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de7be-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="de7be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de7be-106">[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="de7be-106">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de7be-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="de7be-107">Prerequisites</span></span>
<span data-ttu-id="de7be-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="de7be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="de7be-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="de7be-110">Permission type</span></span>|<span data-ttu-id="de7be-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="de7be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de7be-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="de7be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de7be-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de7be-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="de7be-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="de7be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de7be-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de7be-115">Not supported.</span></span>|
|<span data-ttu-id="de7be-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="de7be-116">Application</span></span>|<span data-ttu-id="de7be-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de7be-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de7be-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="de7be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a><span data-ttu-id="de7be-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de7be-119">Request headers</span></span>
|<span data-ttu-id="de7be-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de7be-120">Header</span></span>|<span data-ttu-id="de7be-121">値</span><span class="sxs-lookup"><span data-stu-id="de7be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de7be-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="de7be-122">Authorization</span></span>|<span data-ttu-id="de7be-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="de7be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de7be-124">承諾</span><span class="sxs-lookup"><span data-stu-id="de7be-124">Accept</span></span>|<span data-ttu-id="de7be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de7be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de7be-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="de7be-126">Request body</span></span>
<span data-ttu-id="de7be-127">要求本文で、 [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="de7be-127">In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

<span data-ttu-id="de7be-128">次の表に、 [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="de7be-128">The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span></span>

|<span data-ttu-id="de7be-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de7be-129">Property</span></span>|<span data-ttu-id="de7be-130">型</span><span class="sxs-lookup"><span data-stu-id="de7be-130">Type</span></span>|<span data-ttu-id="de7be-131">説明</span><span class="sxs-lookup"><span data-stu-id="de7be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de7be-132">id</span><span class="sxs-lookup"><span data-stu-id="de7be-132">id</span></span>|<span data-ttu-id="de7be-133">String</span><span class="sxs-lookup"><span data-stu-id="de7be-133">String</span></span>|<span data-ttu-id="de7be-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="de7be-134">The key of the entity.</span></span>|
|<span data-ttu-id="de7be-135">content</span><span class="sxs-lookup"><span data-stu-id="de7be-135">content</span></span>|<span data-ttu-id="de7be-136">Binary</span><span class="sxs-lookup"><span data-stu-id="de7be-136">Binary</span></span>|<span data-ttu-id="de7be-137">Windows Symantec コード署名証明書が生データ形式で表示されます。</span><span class="sxs-lookup"><span data-stu-id="de7be-137">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="de7be-138">status</span><span class="sxs-lookup"><span data-stu-id="de7be-138">status</span></span>|[<span data-ttu-id="de7be-139">certificatestatus</span><span class="sxs-lookup"><span data-stu-id="de7be-139">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="de7be-140">証明書の状態がプロビジョニングされているか、プロビジョニングされていません。</span><span class="sxs-lookup"><span data-stu-id="de7be-140">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="de7be-141">使用可能な値は、`notProvisioned`、`provisioned` です。</span><span class="sxs-lookup"><span data-stu-id="de7be-141">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="de7be-142">password</span><span class="sxs-lookup"><span data-stu-id="de7be-142">password</span></span>|<span data-ttu-id="de7be-143">String</span><span class="sxs-lookup"><span data-stu-id="de7be-143">String</span></span>|<span data-ttu-id="de7be-144">.pfx ファイルに必要なパスワードを指定します。</span><span class="sxs-lookup"><span data-stu-id="de7be-144">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="de7be-145">subjectName</span><span class="sxs-lookup"><span data-stu-id="de7be-145">subjectName</span></span>|<span data-ttu-id="de7be-146">String</span><span class="sxs-lookup"><span data-stu-id="de7be-146">String</span></span>|<span data-ttu-id="de7be-147">証明書のサブジェクト名。</span><span class="sxs-lookup"><span data-stu-id="de7be-147">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="de7be-148">subject</span><span class="sxs-lookup"><span data-stu-id="de7be-148">subject</span></span>|<span data-ttu-id="de7be-149">String</span><span class="sxs-lookup"><span data-stu-id="de7be-149">String</span></span>|<span data-ttu-id="de7be-150">証明書のサブジェクトの値。</span><span class="sxs-lookup"><span data-stu-id="de7be-150">The Subject value for the cert.</span></span>|
|<span data-ttu-id="de7be-151">issuerName</span><span class="sxs-lookup"><span data-stu-id="de7be-151">issuerName</span></span>|<span data-ttu-id="de7be-152">String</span><span class="sxs-lookup"><span data-stu-id="de7be-152">String</span></span>|<span data-ttu-id="de7be-153">証明書の発行者名。</span><span class="sxs-lookup"><span data-stu-id="de7be-153">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="de7be-154">会社</span><span class="sxs-lookup"><span data-stu-id="de7be-154">issuer</span></span>|<span data-ttu-id="de7be-155">String</span><span class="sxs-lookup"><span data-stu-id="de7be-155">String</span></span>|<span data-ttu-id="de7be-156">証明書の発行者の値。</span><span class="sxs-lookup"><span data-stu-id="de7be-156">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="de7be-157">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="de7be-157">expirationDateTime</span></span>|<span data-ttu-id="de7be-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de7be-158">DateTimeOffset</span></span>|<span data-ttu-id="de7be-159">証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="de7be-159">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="de7be-160">uploaddatetime</span><span class="sxs-lookup"><span data-stu-id="de7be-160">uploadDateTime</span></span>|<span data-ttu-id="de7be-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de7be-161">DateTimeOffset</span></span>|<span data-ttu-id="de7be-162">Symantec cert としての CodeSigning cert の種類。</span><span class="sxs-lookup"><span data-stu-id="de7be-162">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|



## <a name="response"></a><span data-ttu-id="de7be-163">応答</span><span class="sxs-lookup"><span data-stu-id="de7be-163">Response</span></span>
<span data-ttu-id="de7be-164">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="de7be-164">If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de7be-165">例</span><span class="sxs-lookup"><span data-stu-id="de7be-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="de7be-166">要求</span><span class="sxs-lookup"><span data-stu-id="de7be-166">Request</span></span>
<span data-ttu-id="de7be-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="de7be-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/symantecCodeSigningCertificate
Content-type: application/json
Content-length: 421

{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "password": "Password value",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```

### <a name="response"></a><span data-ttu-id="de7be-168">応答</span><span class="sxs-lookup"><span data-stu-id="de7be-168">Response</span></span>
<span data-ttu-id="de7be-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="de7be-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 470

{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "00ffe83e-e83e-00ff-3ee8-ff003ee8ff00",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "password": "Password value",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```




