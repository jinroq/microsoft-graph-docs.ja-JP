---
title: ManagedAllDeviceCertificateState を作成する
description: 新しい managedAllDeviceCertificateState オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 024aaee657dbb8bd67491e793ceb99f82ca6d0fd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726068"
---
# <a name="create-managedalldevicecertificatestate"></a><span data-ttu-id="9a902-103">ManagedAllDeviceCertificateState を作成する</span><span class="sxs-lookup"><span data-stu-id="9a902-103">Create managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="9a902-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a902-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a902-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9a902-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a902-106">新しい[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9a902-106">Create a new [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a902-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9a902-107">Prerequisites</span></span>
<span data-ttu-id="9a902-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a902-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a902-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9a902-110">Permission type</span></span>|<span data-ttu-id="9a902-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9a902-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a902-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9a902-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9a902-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a902-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a902-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a902-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a902-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a902-115">Not supported.</span></span>|
|<span data-ttu-id="9a902-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a902-116">Application</span></span>|<span data-ttu-id="9a902-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a902-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a902-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a902-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="9a902-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a902-119">Request headers</span></span>
|<span data-ttu-id="9a902-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a902-120">Header</span></span>|<span data-ttu-id="9a902-121">値</span><span class="sxs-lookup"><span data-stu-id="9a902-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a902-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a902-122">Authorization</span></span>|<span data-ttu-id="9a902-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9a902-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a902-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9a902-124">Accept</span></span>|<span data-ttu-id="9a902-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9a902-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a902-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9a902-126">Request body</span></span>
<span data-ttu-id="9a902-127">要求本文で、managedAllDeviceCertificateState オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9a902-127">In the request body, supply a JSON representation for the managedAllDeviceCertificateState object.</span></span>

<span data-ttu-id="9a902-128">次の表に、managedAllDeviceCertificateState の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9a902-128">The following table shows the properties that are required when you create the managedAllDeviceCertificateState.</span></span>

|<span data-ttu-id="9a902-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a902-129">Property</span></span>|<span data-ttu-id="9a902-130">型</span><span class="sxs-lookup"><span data-stu-id="9a902-130">Type</span></span>|<span data-ttu-id="9a902-131">説明</span><span class="sxs-lookup"><span data-stu-id="9a902-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a902-132">id</span><span class="sxs-lookup"><span data-stu-id="9a902-132">id</span></span>|<span data-ttu-id="9a902-133">文字列</span><span class="sxs-lookup"><span data-stu-id="9a902-133">String</span></span>|<span data-ttu-id="9a902-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9a902-134">Key of the entity.</span></span>|
|<span data-ttu-id="9a902-135">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="9a902-135">certificateRevokeStatus</span></span>|[<span data-ttu-id="9a902-136">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="9a902-136">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="9a902-137">状態を取り消します。</span><span class="sxs-lookup"><span data-stu-id="9a902-137">Revoke status.</span></span> <span data-ttu-id="9a902-138">可能な値は、`none`、`pending`、`issued`、`failed`、`revoked` です。</span><span class="sxs-lookup"><span data-stu-id="9a902-138">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="9a902-139">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="9a902-139">managedDeviceDisplayName</span></span>|<span data-ttu-id="9a902-140">String</span><span class="sxs-lookup"><span data-stu-id="9a902-140">String</span></span>|<span data-ttu-id="9a902-141">デバイスの表示名</span><span class="sxs-lookup"><span data-stu-id="9a902-141">Device display name</span></span>|
|<span data-ttu-id="9a902-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9a902-142">userPrincipalName</span></span>|<span data-ttu-id="9a902-143">String</span><span class="sxs-lookup"><span data-stu-id="9a902-143">String</span></span>|<span data-ttu-id="9a902-144">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="9a902-144">User principal name</span></span>|
|<span data-ttu-id="9a902-145">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9a902-145">certificateExpirationDateTime</span></span>|<span data-ttu-id="9a902-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a902-146">DateTimeOffset</span></span>|<span data-ttu-id="9a902-147">証明書の有効期限</span><span class="sxs-lookup"><span data-stu-id="9a902-147">Certificate expiry date</span></span>|
|<span data-ttu-id="9a902-148">Certificate/Ername</span><span class="sxs-lookup"><span data-stu-id="9a902-148">certificateIssuerName</span></span>|<span data-ttu-id="9a902-149">String</span><span class="sxs-lookup"><span data-stu-id="9a902-149">String</span></span>|<span data-ttu-id="9a902-150">発行者</span><span class="sxs-lookup"><span data-stu-id="9a902-150">Issuer</span></span>|
|<span data-ttu-id="9a902-151">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="9a902-151">certificateThumbprint</span></span>|<span data-ttu-id="9a902-152">String</span><span class="sxs-lookup"><span data-stu-id="9a902-152">String</span></span>|<span data-ttu-id="9a902-153">拇印</span><span class="sxs-lookup"><span data-stu-id="9a902-153">Thumbprint</span></span>|
|<span data-ttu-id="9a902-154">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="9a902-154">certificateSerialNumber</span></span>|<span data-ttu-id="9a902-155">String</span><span class="sxs-lookup"><span data-stu-id="9a902-155">String</span></span>|<span data-ttu-id="9a902-156">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="9a902-156">Serial number</span></span>|
|<span data-ttu-id="9a902-157">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="9a902-157">certificateSubjectName</span></span>|<span data-ttu-id="9a902-158">String</span><span class="sxs-lookup"><span data-stu-id="9a902-158">String</span></span>|<span data-ttu-id="9a902-159">証明書のサブジェクト名</span><span class="sxs-lookup"><span data-stu-id="9a902-159">Certificate subject name</span></span>|
|<span data-ttu-id="9a902-160">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="9a902-160">certificateKeyUsages</span></span>|<span data-ttu-id="9a902-161">Int32</span><span class="sxs-lookup"><span data-stu-id="9a902-161">Int32</span></span>|<span data-ttu-id="9a902-162">キー使用法</span><span class="sxs-lookup"><span data-stu-id="9a902-162">Key Usage</span></span>|
|<span data-ttu-id="9a902-163">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="9a902-163">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="9a902-164">String</span><span class="sxs-lookup"><span data-stu-id="9a902-164">String</span></span>|<span data-ttu-id="9a902-165">拡張キー使用法</span><span class="sxs-lookup"><span data-stu-id="9a902-165">Enhanced Key Usage</span></span>|
|<span data-ttu-id="9a902-166">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="9a902-166">certificateIssuanceDateTime</span></span>|<span data-ttu-id="9a902-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a902-167">DateTimeOffset</span></span>|<span data-ttu-id="9a902-168">発行日</span><span class="sxs-lookup"><span data-stu-id="9a902-168">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="9a902-169">応答</span><span class="sxs-lookup"><span data-stu-id="9a902-169">Response</span></span>
<span data-ttu-id="9a902-170">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9a902-170">If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a902-171">例</span><span class="sxs-lookup"><span data-stu-id="9a902-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a902-172">要求</span><span class="sxs-lookup"><span data-stu-id="9a902-172">Request</span></span>
<span data-ttu-id="9a902-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9a902-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9a902-174">応答</span><span class="sxs-lookup"><span data-stu-id="9a902-174">Response</span></span>
<span data-ttu-id="9a902-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9a902-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





