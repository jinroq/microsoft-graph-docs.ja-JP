---
title: NetworkIPv4ConfigurationManagementCondition を取得する
description: NetworkIPv4ConfigurationManagementCondition オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e6511ba5c57dbdd7ad02b632a5bcd17b59071385
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990240"
---
# <a name="get-networkipv4configurationmanagementcondition"></a><span data-ttu-id="e5f12-103">NetworkIPv4ConfigurationManagementCondition を取得する</span><span class="sxs-lookup"><span data-stu-id="e5f12-103">Get networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="e5f12-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5f12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5f12-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5f12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5f12-106">[NetworkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e5f12-106">Read properties and relationships of the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5f12-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e5f12-107">Prerequisites</span></span>
<span data-ttu-id="e5f12-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5f12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5f12-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e5f12-110">Permission type</span></span>|<span data-ttu-id="e5f12-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e5f12-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5f12-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e5f12-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5f12-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5f12-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e5f12-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e5f12-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5f12-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5f12-115">Not supported.</span></span>|
|<span data-ttu-id="e5f12-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e5f12-116">Application</span></span>|<span data-ttu-id="e5f12-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5f12-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5f12-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e5f12-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5f12-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e5f12-119">Optional query parameters</span></span>
<span data-ttu-id="e5f12-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e5f12-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5f12-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5f12-121">Request headers</span></span>
|<span data-ttu-id="e5f12-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5f12-122">Header</span></span>|<span data-ttu-id="e5f12-123">値</span><span class="sxs-lookup"><span data-stu-id="e5f12-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5f12-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5f12-124">Authorization</span></span>|<span data-ttu-id="e5f12-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5f12-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5f12-126">承諾</span><span class="sxs-lookup"><span data-stu-id="e5f12-126">Accept</span></span>|<span data-ttu-id="e5f12-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e5f12-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5f12-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e5f12-128">Request body</span></span>
<span data-ttu-id="e5f12-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e5f12-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5f12-130">応答</span><span class="sxs-lookup"><span data-stu-id="e5f12-130">Response</span></span>
<span data-ttu-id="e5f12-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e5f12-131">If successful, this method returns a `200 OK` response code and [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5f12-132">例</span><span class="sxs-lookup"><span data-stu-id="e5f12-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5f12-133">要求</span><span class="sxs-lookup"><span data-stu-id="e5f12-133">Request</span></span>
<span data-ttu-id="e5f12-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e5f12-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="e5f12-135">応答</span><span class="sxs-lookup"><span data-stu-id="e5f12-135">Response</span></span>
<span data-ttu-id="e5f12-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e5f12-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "value": {
    "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
    "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
    "uniqueName": "Unique Name value",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "eTag": "ETag value",
    "applicablePlatforms": [
      "androidForWork"
    ],
    "ipV4Prefix": "Ip V4Prefix value",
    "ipV4Gateway": "Ip V4Gateway value",
    "ipV4DHCPServer": "Ip V4DHCPServer value",
    "ipV4DNSServerList": [
      "Ip V4DNSServer List value"
    ],
    "dnsSuffixList": [
      "Dns Suffix List value"
    ]
  }
}
```





