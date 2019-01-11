---
title: AndroidWorkProfileCustomConfiguration を取得します。
description: AndroidWorkProfileCustomConfiguration オブジェクトのプロパティと関係を参照してください。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e966d803a801ff07c91accfea99aac40a99e28c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881110"
---
# <a name="get-androidworkprofilecustomconfiguration"></a><span data-ttu-id="3359b-103">AndroidWorkProfileCustomConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="3359b-103">Get androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="3359b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3359b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3359b-105">[AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3359b-105">Read properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3359b-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="3359b-106">Prerequisites</span></span>
<span data-ttu-id="3359b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3359b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3359b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3359b-109">Permission type</span></span>|<span data-ttu-id="3359b-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3359b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3359b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3359b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3359b-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3359b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3359b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3359b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3359b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3359b-114">Not supported.</span></span>|
|<span data-ttu-id="3359b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3359b-115">Application</span></span>|<span data-ttu-id="3359b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3359b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3359b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3359b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3359b-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3359b-118">Optional query parameters</span></span>
<span data-ttu-id="3359b-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3359b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3359b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3359b-120">Request headers</span></span>
|<span data-ttu-id="3359b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3359b-121">Header</span></span>|<span data-ttu-id="3359b-122">値</span><span class="sxs-lookup"><span data-stu-id="3359b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3359b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3359b-123">Authorization</span></span>|<span data-ttu-id="3359b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3359b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3359b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3359b-125">Accept</span></span>|<span data-ttu-id="3359b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3359b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3359b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3359b-127">Request body</span></span>
<span data-ttu-id="3359b-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3359b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3359b-129">応答</span><span class="sxs-lookup"><span data-stu-id="3359b-129">Response</span></span>
<span data-ttu-id="3359b-130">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="3359b-130">If successful, this method returns a `200 OK` response code and [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3359b-131">例</span><span class="sxs-lookup"><span data-stu-id="3359b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3359b-132">要求</span><span class="sxs-lookup"><span data-stu-id="3359b-132">Request</span></span>
<span data-ttu-id="3359b-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3359b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="3359b-134">応答</span><span class="sxs-lookup"><span data-stu-id="3359b-134">Response</span></span>
<span data-ttu-id="3359b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3359b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 636

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
    "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "omaSettings": [
      {
        "@odata.type": "microsoft.graph.omaSettingInteger",
        "displayName": "Display Name value",
        "description": "Description value",
        "omaUri": "Oma Uri value",
        "value": 5
      }
    ]
  }
}
```



