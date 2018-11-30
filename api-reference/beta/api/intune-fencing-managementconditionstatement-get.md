---
title: ManagementConditionStatement を取得します。
description: ManagementConditionStatement オブジェクトのプロパティと関係を参照してください。
ms.openlocfilehash: 8a89c1c83e1d38e061bcb738331f538a93e6c13d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072725"
---
# <a name="get-managementconditionstatement"></a><span data-ttu-id="41e13-103">ManagementConditionStatement を取得します。</span><span class="sxs-lookup"><span data-stu-id="41e13-103">Get managementConditionStatement</span></span>

> <span data-ttu-id="41e13-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="41e13-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41e13-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41e13-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="41e13-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="41e13-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41e13-107">[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41e13-107">Read properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="41e13-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="41e13-108">Prerequisites</span></span>
<span data-ttu-id="41e13-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41e13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41e13-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="41e13-111">Permission type</span></span>|<span data-ttu-id="41e13-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="41e13-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41e13-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="41e13-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41e13-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="41e13-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="41e13-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="41e13-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41e13-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41e13-116">Not supported.</span></span>|
|<span data-ttu-id="41e13-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="41e13-117">Application</span></span>|<span data-ttu-id="41e13-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41e13-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41e13-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="41e13-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/{managementConditionStatementId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41e13-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="41e13-120">Optional query parameters</span></span>
<span data-ttu-id="41e13-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="41e13-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="41e13-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41e13-122">Request headers</span></span>
|<span data-ttu-id="41e13-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41e13-123">Header</span></span>|<span data-ttu-id="41e13-124">値</span><span class="sxs-lookup"><span data-stu-id="41e13-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41e13-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="41e13-125">Authorization</span></span>|<span data-ttu-id="41e13-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="41e13-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41e13-127">Accept</span><span class="sxs-lookup"><span data-stu-id="41e13-127">Accept</span></span>|<span data-ttu-id="41e13-128">application/json</span><span class="sxs-lookup"><span data-stu-id="41e13-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41e13-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="41e13-129">Request body</span></span>
<span data-ttu-id="41e13-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="41e13-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41e13-131">応答</span><span class="sxs-lookup"><span data-stu-id="41e13-131">Response</span></span>
<span data-ttu-id="41e13-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="41e13-132">If successful, this method returns a `200 OK` response code and [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41e13-133">例</span><span class="sxs-lookup"><span data-stu-id="41e13-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="41e13-134">要求</span><span class="sxs-lookup"><span data-stu-id="41e13-134">Request</span></span>
<span data-ttu-id="41e13-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="41e13-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}
```

### <a name="response"></a><span data-ttu-id="41e13-136">応答</span><span class="sxs-lookup"><span data-stu-id="41e13-136">Response</span></span>
<span data-ttu-id="41e13-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="41e13-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 536

{
  "value": {
    "@odata.type": "#microsoft.graph.managementConditionStatement",
    "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "expression": {
      "@odata.type": "microsoft.graph.managementConditionExpression"
    },
    "eTag": "ETag value",
    "applicablePlatforms": [
      "androidForWork"
    ]
  }
}
```





