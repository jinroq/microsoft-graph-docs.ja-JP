---
title: ManagedAllDeviceCertificateState を作成する
description: 新しい managedAllDeviceCertificateState オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 50877255e069c70749ae77b515d7f45a90398a33
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338589"
---
# <a name="create-managedalldevicecertificatestate"></a><span data-ttu-id="9d402-103">ManagedAllDeviceCertificateState を作成する</span><span class="sxs-lookup"><span data-stu-id="9d402-103">Create managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="9d402-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d402-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d402-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9d402-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d402-106">新しい[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9d402-106">Create a new [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d402-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9d402-107">Prerequisites</span></span>
<span data-ttu-id="9d402-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d402-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d402-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9d402-110">Permission type</span></span>|<span data-ttu-id="9d402-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9d402-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d402-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9d402-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9d402-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d402-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9d402-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9d402-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d402-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d402-115">Not supported.</span></span>|
|<span data-ttu-id="9d402-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9d402-116">Application</span></span>|<span data-ttu-id="9d402-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d402-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d402-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9d402-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="9d402-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d402-119">Request headers</span></span>
|<span data-ttu-id="9d402-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d402-120">Header</span></span>|<span data-ttu-id="9d402-121">値</span><span class="sxs-lookup"><span data-stu-id="9d402-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d402-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d402-122">Authorization</span></span>|<span data-ttu-id="9d402-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9d402-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d402-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9d402-124">Accept</span></span>|<span data-ttu-id="9d402-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9d402-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d402-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9d402-126">Request body</span></span>
<span data-ttu-id="9d402-127">要求本文で、managedAllDeviceCertificateState オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9d402-127">In the request body, supply a JSON representation for the managedAllDeviceCertificateState object.</span></span>

<span data-ttu-id="9d402-128">次の表に、managedAllDeviceCertificateState の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9d402-128">The following table shows the properties that are required when you create the managedAllDeviceCertificateState.</span></span>

|<span data-ttu-id="9d402-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d402-129">Property</span></span>|<span data-ttu-id="9d402-130">型</span><span class="sxs-lookup"><span data-stu-id="9d402-130">Type</span></span>|<span data-ttu-id="9d402-131">説明</span><span class="sxs-lookup"><span data-stu-id="9d402-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d402-132">id</span><span class="sxs-lookup"><span data-stu-id="9d402-132">id</span></span>|<span data-ttu-id="9d402-133">文字列</span><span class="sxs-lookup"><span data-stu-id="9d402-133">String</span></span>|<span data-ttu-id="9d402-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9d402-134">Key of the entity.</span></span>|
|<span data-ttu-id="9d402-135">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="9d402-135">certificateRevokeStatus</span></span>|[<span data-ttu-id="9d402-136">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="9d402-136">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="9d402-137">状態を取り消します。</span><span class="sxs-lookup"><span data-stu-id="9d402-137">Revoke status.</span></span> <span data-ttu-id="9d402-138">可能な値は、`none`、`pending`、`issued`、`failed`、`revoked` です。</span><span class="sxs-lookup"><span data-stu-id="9d402-138">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="9d402-139">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="9d402-139">managedDeviceDisplayName</span></span>|<span data-ttu-id="9d402-140">String</span><span class="sxs-lookup"><span data-stu-id="9d402-140">String</span></span>|<span data-ttu-id="9d402-141">デバイスの表示名</span><span class="sxs-lookup"><span data-stu-id="9d402-141">Device display name</span></span>|
|<span data-ttu-id="9d402-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9d402-142">userPrincipalName</span></span>|<span data-ttu-id="9d402-143">String</span><span class="sxs-lookup"><span data-stu-id="9d402-143">String</span></span>|<span data-ttu-id="9d402-144">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="9d402-144">User principal name</span></span>|
|<span data-ttu-id="9d402-145">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9d402-145">certificateExpirationDateTime</span></span>|<span data-ttu-id="9d402-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d402-146">DateTimeOffset</span></span>|<span data-ttu-id="9d402-147">証明書の有効期限</span><span class="sxs-lookup"><span data-stu-id="9d402-147">Certificate expiry date</span></span>|
|<span data-ttu-id="9d402-148">Certificate/Ername</span><span class="sxs-lookup"><span data-stu-id="9d402-148">certificateIssuerName</span></span>|<span data-ttu-id="9d402-149">String</span><span class="sxs-lookup"><span data-stu-id="9d402-149">String</span></span>|<span data-ttu-id="9d402-150">発行者</span><span class="sxs-lookup"><span data-stu-id="9d402-150">Issuer</span></span>|
|<span data-ttu-id="9d402-151">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="9d402-151">certificateThumbprint</span></span>|<span data-ttu-id="9d402-152">String</span><span class="sxs-lookup"><span data-stu-id="9d402-152">String</span></span>|<span data-ttu-id="9d402-153">拇印</span><span class="sxs-lookup"><span data-stu-id="9d402-153">Thumbprint</span></span>|
|<span data-ttu-id="9d402-154">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="9d402-154">certificateSerialNumber</span></span>|<span data-ttu-id="9d402-155">String</span><span class="sxs-lookup"><span data-stu-id="9d402-155">String</span></span>|<span data-ttu-id="9d402-156">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="9d402-156">Serial number</span></span>|
|<span data-ttu-id="9d402-157">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="9d402-157">certificateSubjectName</span></span>|<span data-ttu-id="9d402-158">String</span><span class="sxs-lookup"><span data-stu-id="9d402-158">String</span></span>|<span data-ttu-id="9d402-159">証明書のサブジェクト名</span><span class="sxs-lookup"><span data-stu-id="9d402-159">Certificate subject name</span></span>|
|<span data-ttu-id="9d402-160">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="9d402-160">certificateKeyUsages</span></span>|<span data-ttu-id="9d402-161">Int32</span><span class="sxs-lookup"><span data-stu-id="9d402-161">Int32</span></span>|<span data-ttu-id="9d402-162">キー使用法</span><span class="sxs-lookup"><span data-stu-id="9d402-162">Key Usage</span></span>|
|<span data-ttu-id="9d402-163">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="9d402-163">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="9d402-164">String</span><span class="sxs-lookup"><span data-stu-id="9d402-164">String</span></span>|<span data-ttu-id="9d402-165">拡張キー使用法</span><span class="sxs-lookup"><span data-stu-id="9d402-165">Enhanced Key Usage</span></span>|
|<span data-ttu-id="9d402-166">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="9d402-166">certificateIssuanceDateTime</span></span>|<span data-ttu-id="9d402-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d402-167">DateTimeOffset</span></span>|<span data-ttu-id="9d402-168">発行日</span><span class="sxs-lookup"><span data-stu-id="9d402-168">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="9d402-169">応答</span><span class="sxs-lookup"><span data-stu-id="9d402-169">Response</span></span>
<span data-ttu-id="9d402-170">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9d402-170">If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d402-171">例</span><span class="sxs-lookup"><span data-stu-id="9d402-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d402-172">要求</span><span class="sxs-lookup"><span data-stu-id="9d402-172">Request</span></span>
<span data-ttu-id="9d402-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9d402-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
Content-type: application/json
Content-length: 735

{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "certificateRevokeStatus": "pending",
  "managedDeviceDisplayName": "Managed Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateIssuerName": "Certificate Issuer Name value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateSubjectName": "Certificate Subject Name value",
  "certificateKeyUsages": 4,
  "certificateExtendedKeyUsages": "Certificate Extended Key Usages value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```

### <a name="response"></a><span data-ttu-id="9d402-174">応答</span><span class="sxs-lookup"><span data-stu-id="9d402-174">Response</span></span>
<span data-ttu-id="9d402-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9d402-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 784

{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "id": "987c6a17-6a17-987c-176a-7c98176a7c98",
  "certificateRevokeStatus": "pending",
  "managedDeviceDisplayName": "Managed Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateIssuerName": "Certificate Issuer Name value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateSubjectName": "Certificate Subject Name value",
  "certificateKeyUsages": 4,
  "certificateExtendedKeyUsages": "Certificate Extended Key Usages value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```






