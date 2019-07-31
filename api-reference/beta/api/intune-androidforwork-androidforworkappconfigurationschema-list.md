---
title: androidForWorkAppConfigurationSchemas のリスト
description: androidForWorkAppConfigurationSchema オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cff24d93eb1f85b1c6694978819c6234ce268480
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35952815"
---
# <a name="list-androidforworkappconfigurationschemas"></a><span data-ttu-id="7943f-103">androidForWorkAppConfigurationSchemas のリスト</span><span class="sxs-lookup"><span data-stu-id="7943f-103">List androidForWorkAppConfigurationSchemas</span></span>

> <span data-ttu-id="7943f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7943f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7943f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7943f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7943f-106">[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7943f-106">List properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7943f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7943f-107">Prerequisites</span></span>
<span data-ttu-id="7943f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7943f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7943f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7943f-110">Permission type</span></span>|<span data-ttu-id="7943f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7943f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7943f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7943f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7943f-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7943f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7943f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7943f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7943f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7943f-115">Not supported.</span></span>|
|<span data-ttu-id="7943f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7943f-116">Application</span></span>|<span data-ttu-id="7943f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7943f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7943f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7943f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="7943f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7943f-119">Request headers</span></span>
|<span data-ttu-id="7943f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7943f-120">Header</span></span>|<span data-ttu-id="7943f-121">値</span><span class="sxs-lookup"><span data-stu-id="7943f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7943f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7943f-122">Authorization</span></span>|<span data-ttu-id="7943f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7943f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7943f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7943f-124">Accept</span></span>|<span data-ttu-id="7943f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7943f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7943f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7943f-126">Request body</span></span>
<span data-ttu-id="7943f-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7943f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7943f-128">応答</span><span class="sxs-lookup"><span data-stu-id="7943f-128">Response</span></span>
<span data-ttu-id="7943f-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7943f-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7943f-130">例</span><span class="sxs-lookup"><span data-stu-id="7943f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7943f-131">要求</span><span class="sxs-lookup"><span data-stu-id="7943f-131">Request</span></span>
<span data-ttu-id="7943f-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7943f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas
```

### <a name="response"></a><span data-ttu-id="7943f-133">応答</span><span class="sxs-lookup"><span data-stu-id="7943f-133">Response</span></span>
<span data-ttu-id="7943f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7943f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 977

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
      "id": "c1230dc6-0dc6-c123-c60d-23c1c60d23c1",
      "exampleJson": "ZXhhbXBsZUpzb24=",
      "schemaItems": [
        {
          "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
          "schemaItemKey": "Schema Item Key value",
          "displayName": "Display Name value",
          "description": "Description value",
          "defaultBoolValue": true,
          "defaultIntValue": 15,
          "defaultStringValue": "Default String Value value",
          "defaultStringArrayValue": [
            "Default String Array Value value"
          ],
          "dataType": "integer",
          "selections": [
            {
              "@odata.type": "microsoft.graph.keyValuePair",
              "name": "Name value",
              "value": "Value value"
            }
          ]
        }
      ]
    }
  ]
}
```





