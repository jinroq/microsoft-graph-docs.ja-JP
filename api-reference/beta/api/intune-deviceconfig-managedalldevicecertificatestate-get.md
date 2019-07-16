---
title: ManagedAllDeviceCertificateState を取得する
description: ManagedAllDeviceCertificateState オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 879c030e3668c25aef1a18d011c87a22c70f0134
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726065"
---
# <a name="get-managedalldevicecertificatestate"></a><span data-ttu-id="9830d-103">ManagedAllDeviceCertificateState を取得する</span><span class="sxs-lookup"><span data-stu-id="9830d-103">Get managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="9830d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9830d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9830d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9830d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9830d-106">[ManagedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9830d-106">Read properties and relationships of the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9830d-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9830d-107">Prerequisites</span></span>
<span data-ttu-id="9830d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9830d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9830d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9830d-110">Permission type</span></span>|<span data-ttu-id="9830d-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9830d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9830d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9830d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9830d-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9830d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9830d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9830d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9830d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9830d-115">Not supported.</span></span>|
|<span data-ttu-id="9830d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9830d-116">Application</span></span>|<span data-ttu-id="9830d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9830d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9830d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9830d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9830d-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9830d-119">Optional query parameters</span></span>
<span data-ttu-id="9830d-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9830d-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9830d-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9830d-121">Request headers</span></span>
|<span data-ttu-id="9830d-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9830d-122">Header</span></span>|<span data-ttu-id="9830d-123">値</span><span class="sxs-lookup"><span data-stu-id="9830d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9830d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9830d-124">Authorization</span></span>|<span data-ttu-id="9830d-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9830d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9830d-126">承諾</span><span class="sxs-lookup"><span data-stu-id="9830d-126">Accept</span></span>|<span data-ttu-id="9830d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9830d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9830d-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="9830d-128">Request body</span></span>
<span data-ttu-id="9830d-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9830d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9830d-130">応答</span><span class="sxs-lookup"><span data-stu-id="9830d-130">Response</span></span>
<span data-ttu-id="9830d-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9830d-131">If successful, this method returns a `200 OK` response code and [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9830d-132">例</span><span class="sxs-lookup"><span data-stu-id="9830d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9830d-133">要求</span><span class="sxs-lookup"><span data-stu-id="9830d-133">Request</span></span>
<span data-ttu-id="9830d-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9830d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="9830d-135">応答</span><span class="sxs-lookup"><span data-stu-id="9830d-135">Response</span></span>
<span data-ttu-id="9830d-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9830d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 829

{
  "value": {
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
}
```





