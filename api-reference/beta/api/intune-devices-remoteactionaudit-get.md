---
title: RemoteActionAudit の取得
description: RemoteActionAudit オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d625faceac71275140fc61ebcc072fe2c016823
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958068"
---
# <a name="get-remoteactionaudit"></a><span data-ttu-id="9e9fb-103">RemoteActionAudit の取得</span><span class="sxs-lookup"><span data-stu-id="9e9fb-103">Get remoteActionAudit</span></span>

> <span data-ttu-id="9e9fb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e9fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e9fb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9e9fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e9fb-106">[Remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9e9fb-106">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e9fb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9e9fb-107">Prerequisites</span></span>
<span data-ttu-id="9e9fb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9e9fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e9fb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9e9fb-110">Permission type</span></span>|<span data-ttu-id="9e9fb-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9e9fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e9fb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9e9fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e9fb-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e9fb-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9e9fb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9e9fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e9fb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e9fb-115">Not supported.</span></span>|
|<span data-ttu-id="9e9fb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9e9fb-116">Application</span></span>|<span data-ttu-id="9e9fb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e9fb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e9fb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9e9fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9e9fb-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9e9fb-119">Optional query parameters</span></span>
<span data-ttu-id="9e9fb-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9e9fb-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e9fb-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e9fb-121">Request headers</span></span>
|<span data-ttu-id="9e9fb-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e9fb-122">Header</span></span>|<span data-ttu-id="9e9fb-123">値</span><span class="sxs-lookup"><span data-stu-id="9e9fb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e9fb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e9fb-124">Authorization</span></span>|<span data-ttu-id="9e9fb-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9e9fb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e9fb-126">承諾</span><span class="sxs-lookup"><span data-stu-id="9e9fb-126">Accept</span></span>|<span data-ttu-id="9e9fb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9e9fb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e9fb-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="9e9fb-128">Request body</span></span>
<span data-ttu-id="9e9fb-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9e9fb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e9fb-130">応答</span><span class="sxs-lookup"><span data-stu-id="9e9fb-130">Response</span></span>
<span data-ttu-id="9e9fb-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[remoteactionaudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9e9fb-131">If successful, this method returns a `200 OK` response code and [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e9fb-132">例</span><span class="sxs-lookup"><span data-stu-id="9e9fb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e9fb-133">要求</span><span class="sxs-lookup"><span data-stu-id="9e9fb-133">Request</span></span>
<span data-ttu-id="9e9fb-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9e9fb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

### <a name="response"></a><span data-ttu-id="9e9fb-135">応答</span><span class="sxs-lookup"><span data-stu-id="9e9fb-135">Response</span></span>
<span data-ttu-id="9e9fb-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9e9fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

{
  "value": {
    "@odata.type": "#microsoft.graph.remoteActionAudit",
    "id": "477f8d24-8d24-477f-248d-7f47248d7f47",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
    "action": "factoryReset",
    "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
    "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
    "deviceIMEI": "Device IMEI value",
    "actionState": "pending"
  }
}
```





