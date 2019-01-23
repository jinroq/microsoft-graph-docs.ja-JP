---
title: GroupPolicyPresentationValueText を取得します。
description: GroupPolicyPresentationValueText オブジェクトのプロパティと関係を参照してください。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a615e8893302bee4ba6cf777ba5255140db65d69
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430472"
---
# <a name="get-grouppolicypresentationvaluetext"></a><span data-ttu-id="ff8e2-103">GroupPolicyPresentationValueText を取得します。</span><span class="sxs-lookup"><span data-stu-id="ff8e2-103">Get groupPolicyPresentationValueText</span></span>

> <span data-ttu-id="ff8e2-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ff8e2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ff8e2-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff8e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff8e2-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ff8e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff8e2-107">[GroupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff8e2-107">Read properties and relationships of the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff8e2-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ff8e2-108">Prerequisites</span></span>
<span data-ttu-id="ff8e2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff8e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ff8e2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff8e2-111">Permission type</span></span>|<span data-ttu-id="ff8e2-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff8e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff8e2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff8e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff8e2-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff8e2-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ff8e2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff8e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff8e2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff8e2-116">Not supported.</span></span>|
|<span data-ttu-id="ff8e2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff8e2-117">Application</span></span>|<span data-ttu-id="ff8e2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff8e2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff8e2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff8e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff8e2-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ff8e2-120">Optional query parameters</span></span>
<span data-ttu-id="ff8e2-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ff8e2-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff8e2-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff8e2-122">Request headers</span></span>
|<span data-ttu-id="ff8e2-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff8e2-123">Header</span></span>|<span data-ttu-id="ff8e2-124">値</span><span class="sxs-lookup"><span data-stu-id="ff8e2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff8e2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff8e2-125">Authorization</span></span>|<span data-ttu-id="ff8e2-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ff8e2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff8e2-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ff8e2-127">Accept</span></span>|<span data-ttu-id="ff8e2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ff8e2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff8e2-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff8e2-129">Request body</span></span>
<span data-ttu-id="ff8e2-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ff8e2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff8e2-131">応答</span><span class="sxs-lookup"><span data-stu-id="ff8e2-131">Response</span></span>
<span data-ttu-id="ff8e2-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ff8e2-132">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff8e2-133">例</span><span class="sxs-lookup"><span data-stu-id="ff8e2-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff8e2-134">要求</span><span class="sxs-lookup"><span data-stu-id="ff8e2-134">Request</span></span>
<span data-ttu-id="ff8e2-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ff8e2-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

### <a name="response"></a><span data-ttu-id="ff8e2-136">応答</span><span class="sxs-lookup"><span data-stu-id="ff8e2-136">Response</span></span>
<span data-ttu-id="ff8e2-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ff8e2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "id": "a3883444-3444-a388-4434-88a3443488a3",
    "value": "Value value"
  }
}
```




