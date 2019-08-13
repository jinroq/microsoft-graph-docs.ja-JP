---
title: ManagedAllDeviceCertificateState の更新
description: ManagedAllDeviceCertificateState オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 520afd6fb7b2980b8c263dff2f44b52ac2c2f610
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345618"
---
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="1fd64-103">ManagedAllDeviceCertificateState の更新</span><span class="sxs-lookup"><span data-stu-id="1fd64-103">Update managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="1fd64-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1fd64-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fd64-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1fd64-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fd64-106">[ManagedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1fd64-106">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fd64-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1fd64-107">Prerequisites</span></span>
<span data-ttu-id="1fd64-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1fd64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fd64-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1fd64-110">Permission type</span></span>|<span data-ttu-id="1fd64-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1fd64-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fd64-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1fd64-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1fd64-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fd64-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1fd64-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1fd64-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fd64-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1fd64-115">Not supported.</span></span>|
|<span data-ttu-id="1fd64-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1fd64-116">Application</span></span>|<span data-ttu-id="1fd64-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fd64-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fd64-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1fd64-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="1fd64-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1fd64-119">Request headers</span></span>
|<span data-ttu-id="1fd64-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1fd64-120">Header</span></span>|<span data-ttu-id="1fd64-121">値</span><span class="sxs-lookup"><span data-stu-id="1fd64-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fd64-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fd64-122">Authorization</span></span>|<span data-ttu-id="1fd64-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1fd64-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fd64-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1fd64-124">Accept</span></span>|<span data-ttu-id="1fd64-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1fd64-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fd64-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1fd64-126">Request body</span></span>
<span data-ttu-id="1fd64-127">要求本文で、 [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1fd64-127">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="1fd64-128">次の表に、 [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1fd64-128">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="1fd64-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1fd64-129">Property</span></span>|<span data-ttu-id="1fd64-130">型</span><span class="sxs-lookup"><span data-stu-id="1fd64-130">Type</span></span>|<span data-ttu-id="1fd64-131">説明</span><span class="sxs-lookup"><span data-stu-id="1fd64-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fd64-132">id</span><span class="sxs-lookup"><span data-stu-id="1fd64-132">id</span></span>|<span data-ttu-id="1fd64-133">文字列</span><span class="sxs-lookup"><span data-stu-id="1fd64-133">String</span></span>|<span data-ttu-id="1fd64-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1fd64-134">Key of the entity.</span></span>|
|<span data-ttu-id="1fd64-135">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="1fd64-135">certificateRevokeStatus</span></span>|[<span data-ttu-id="1fd64-136">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="1fd64-136">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="1fd64-137">状態を取り消します。</span><span class="sxs-lookup"><span data-stu-id="1fd64-137">Revoke status.</span></span> <span data-ttu-id="1fd64-138">可能な値は、`none`、`pending`、`issued`、`failed`、`revoked` です。</span><span class="sxs-lookup"><span data-stu-id="1fd64-138">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="1fd64-139">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="1fd64-139">managedDeviceDisplayName</span></span>|<span data-ttu-id="1fd64-140">String</span><span class="sxs-lookup"><span data-stu-id="1fd64-140">String</span></span>|<span data-ttu-id="1fd64-141">デバイスの表示名</span><span class="sxs-lookup"><span data-stu-id="1fd64-141">Device display name</span></span>|
|<span data-ttu-id="1fd64-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1fd64-142">userPrincipalName</span></span>|<span data-ttu-id="1fd64-143">String</span><span class="sxs-lookup"><span data-stu-id="1fd64-143">String</span></span>|<span data-ttu-id="1fd64-144">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="1fd64-144">User principal name</span></span>|
|<span data-ttu-id="1fd64-145">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1fd64-145">certificateExpirationDateTime</span></span>|<span data-ttu-id="1fd64-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fd64-146">DateTimeOffset</span></span>|<span data-ttu-id="1fd64-147">証明書の有効期限</span><span class="sxs-lookup"><span data-stu-id="1fd64-147">Certificate expiry date</span></span>|
|<span data-ttu-id="1fd64-148">Certificate/Ername</span><span class="sxs-lookup"><span data-stu-id="1fd64-148">certificateIssuerName</span></span>|<span data-ttu-id="1fd64-149">String</span><span class="sxs-lookup"><span data-stu-id="1fd64-149">String</span></span>|<span data-ttu-id="1fd64-150">発行者</span><span class="sxs-lookup"><span data-stu-id="1fd64-150">Issuer</span></span>|
|<span data-ttu-id="1fd64-151">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="1fd64-151">certificateThumbprint</span></span>|<span data-ttu-id="1fd64-152">String</span><span class="sxs-lookup"><span data-stu-id="1fd64-152">String</span></span>|<span data-ttu-id="1fd64-153">拇印</span><span class="sxs-lookup"><span data-stu-id="1fd64-153">Thumbprint</span></span>|
|<span data-ttu-id="1fd64-154">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="1fd64-154">certificateSerialNumber</span></span>|<span data-ttu-id="1fd64-155">String</span><span class="sxs-lookup"><span data-stu-id="1fd64-155">String</span></span>|<span data-ttu-id="1fd64-156">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="1fd64-156">Serial number</span></span>|
|<span data-ttu-id="1fd64-157">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="1fd64-157">certificateSubjectName</span></span>|<span data-ttu-id="1fd64-158">String</span><span class="sxs-lookup"><span data-stu-id="1fd64-158">String</span></span>|<span data-ttu-id="1fd64-159">証明書のサブジェクト名</span><span class="sxs-lookup"><span data-stu-id="1fd64-159">Certificate subject name</span></span>|
|<span data-ttu-id="1fd64-160">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="1fd64-160">certificateKeyUsages</span></span>|<span data-ttu-id="1fd64-161">Int32</span><span class="sxs-lookup"><span data-stu-id="1fd64-161">Int32</span></span>|<span data-ttu-id="1fd64-162">キー使用法</span><span class="sxs-lookup"><span data-stu-id="1fd64-162">Key Usage</span></span>|
|<span data-ttu-id="1fd64-163">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="1fd64-163">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="1fd64-164">String</span><span class="sxs-lookup"><span data-stu-id="1fd64-164">String</span></span>|<span data-ttu-id="1fd64-165">拡張キー使用法</span><span class="sxs-lookup"><span data-stu-id="1fd64-165">Enhanced Key Usage</span></span>|
|<span data-ttu-id="1fd64-166">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="1fd64-166">certificateIssuanceDateTime</span></span>|<span data-ttu-id="1fd64-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fd64-167">DateTimeOffset</span></span>|<span data-ttu-id="1fd64-168">発行日</span><span class="sxs-lookup"><span data-stu-id="1fd64-168">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="1fd64-169">応答</span><span class="sxs-lookup"><span data-stu-id="1fd64-169">Response</span></span>
<span data-ttu-id="1fd64-170">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1fd64-170">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fd64-171">例</span><span class="sxs-lookup"><span data-stu-id="1fd64-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fd64-172">要求</span><span class="sxs-lookup"><span data-stu-id="1fd64-172">Request</span></span>
<span data-ttu-id="1fd64-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1fd64-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
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

### <a name="response"></a><span data-ttu-id="1fd64-174">応答</span><span class="sxs-lookup"><span data-stu-id="1fd64-174">Response</span></span>
<span data-ttu-id="1fd64-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1fd64-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






