---
title: OfficeClientConfigurationAssignment を取得します。
description: OfficeClientConfigurationAssignment オブジェクトのプロパティと関係を参照してください。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 36bb0c9649dea726ea019e24c218e5f3f0b03422
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425359"
---
# <a name="get-officeclientconfigurationassignment"></a><span data-ttu-id="82566-103">OfficeClientConfigurationAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="82566-103">Get officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="82566-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="82566-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="82566-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82566-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82566-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="82566-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82566-107">[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82566-107">Read properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82566-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="82566-108">Prerequisites</span></span>
<span data-ttu-id="82566-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82566-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82566-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="82566-111">Permission type</span></span>|<span data-ttu-id="82566-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="82566-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82566-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="82566-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82566-114">\* \* TODO: スコープを決定する \* \*</span><span class="sxs-lookup"><span data-stu-id="82566-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="82566-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="82566-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82566-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82566-116">Not supported.</span></span>|
|<span data-ttu-id="82566-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="82566-117">Application</span></span>|<span data-ttu-id="82566-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82566-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82566-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="82566-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="82566-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="82566-120">Optional query parameters</span></span>
<span data-ttu-id="82566-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="82566-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="82566-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82566-122">Request headers</span></span>
|<span data-ttu-id="82566-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82566-123">Header</span></span>|<span data-ttu-id="82566-124">値</span><span class="sxs-lookup"><span data-stu-id="82566-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82566-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="82566-125">Authorization</span></span>|<span data-ttu-id="82566-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="82566-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82566-127">Accept</span><span class="sxs-lookup"><span data-stu-id="82566-127">Accept</span></span>|<span data-ttu-id="82566-128">application/json</span><span class="sxs-lookup"><span data-stu-id="82566-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82566-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="82566-129">Request body</span></span>
<span data-ttu-id="82566-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="82566-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82566-131">応答</span><span class="sxs-lookup"><span data-stu-id="82566-131">Response</span></span>
<span data-ttu-id="82566-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="82566-132">If successful, this method returns a `200 OK` response code and [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82566-133">例</span><span class="sxs-lookup"><span data-stu-id="82566-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="82566-134">要求</span><span class="sxs-lookup"><span data-stu-id="82566-134">Request</span></span>
<span data-ttu-id="82566-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="82566-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="82566-136">応答</span><span class="sxs-lookup"><span data-stu-id="82566-136">Response</span></span>
<span data-ttu-id="82566-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="82566-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 250

{
  "value": {
    "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
    "id": "804730f3-30f3-8047-f330-4780f3304780",
    "target": {
      "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
    }
  }
}
```



