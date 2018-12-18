---
title: getManagementConditionStatementsForPlatform 関数
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 6589cb380f5ea639b27cb4d3e2258b0bc9f1516f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321939"
---
# <a name="getmanagementconditionstatementsforplatform-function"></a><span data-ttu-id="24d8a-103">getManagementConditionStatementsForPlatform 関数</span><span class="sxs-lookup"><span data-stu-id="24d8a-103">getManagementConditionStatementsForPlatform function</span></span>

> <span data-ttu-id="24d8a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="24d8a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24d8a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24d8a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24d8a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="24d8a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24d8a-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="24d8a-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="24d8a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="24d8a-108">Prerequisites</span></span>
<span data-ttu-id="24d8a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24d8a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24d8a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="24d8a-111">Permission type</span></span>|<span data-ttu-id="24d8a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="24d8a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24d8a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="24d8a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24d8a-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="24d8a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="24d8a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="24d8a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24d8a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24d8a-116">Not supported.</span></span>|
|<span data-ttu-id="24d8a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="24d8a-117">Application</span></span>|<span data-ttu-id="24d8a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24d8a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24d8a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="24d8a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/getManagementConditionStatementsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="24d8a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24d8a-120">Request headers</span></span>
|<span data-ttu-id="24d8a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24d8a-121">Header</span></span>|<span data-ttu-id="24d8a-122">値</span><span class="sxs-lookup"><span data-stu-id="24d8a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24d8a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="24d8a-123">Authorization</span></span>|<span data-ttu-id="24d8a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="24d8a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24d8a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="24d8a-125">Accept</span></span>|<span data-ttu-id="24d8a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24d8a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24d8a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="24d8a-127">Request body</span></span>
<span data-ttu-id="24d8a-128">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="24d8a-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="24d8a-129">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="24d8a-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="24d8a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24d8a-130">Property</span></span>|<span data-ttu-id="24d8a-131">種類</span><span class="sxs-lookup"><span data-stu-id="24d8a-131">Type</span></span>|<span data-ttu-id="24d8a-132">説明</span><span class="sxs-lookup"><span data-stu-id="24d8a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24d8a-133">platform</span><span class="sxs-lookup"><span data-stu-id="24d8a-133">platform</span></span>|[<span data-ttu-id="24d8a-134">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="24d8a-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="24d8a-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="24d8a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="24d8a-136">応答</span><span class="sxs-lookup"><span data-stu-id="24d8a-136">Response</span></span>
<span data-ttu-id="24d8a-137">かどうかは成功すると、この関数を返します、`200 OK`応答コードおよび応答の本文に[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="24d8a-137">If successful, this function returns a `200 OK` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24d8a-138">例</span><span class="sxs-lookup"><span data-stu-id="24d8a-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="24d8a-139">要求</span><span class="sxs-lookup"><span data-stu-id="24d8a-139">Request</span></span>
<span data-ttu-id="24d8a-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="24d8a-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="24d8a-141">応答</span><span class="sxs-lookup"><span data-stu-id="24d8a-141">Response</span></span>
<span data-ttu-id="24d8a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="24d8a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

{
  "value": [
    {
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
  ]
}
```





