---
title: groupPolicyPresentationLongDecimalTextBox を取得する
description: groupPolicyPresentationLongDecimalTextBox オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 13c4cc97c2ebcceb58494f85584ef3f56aed6ac4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32530964"
---
# <a name="get-grouppolicypresentationlongdecimaltextbox"></a><span data-ttu-id="79ae9-103">groupPolicyPresentationLongDecimalTextBox を取得する</span><span class="sxs-lookup"><span data-stu-id="79ae9-103">Get groupPolicyPresentationLongDecimalTextBox</span></span>

> <span data-ttu-id="79ae9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79ae9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79ae9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="79ae9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79ae9-106">[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="79ae9-106">Read properties and relationships of the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79ae9-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="79ae9-107">Prerequisites</span></span>
<span data-ttu-id="79ae9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79ae9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79ae9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79ae9-110">Permission type</span></span>|<span data-ttu-id="79ae9-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="79ae9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79ae9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79ae9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79ae9-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="79ae9-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="79ae9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79ae9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79ae9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79ae9-115">Not supported.</span></span>|
|<span data-ttu-id="79ae9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79ae9-116">Application</span></span>|<span data-ttu-id="79ae9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79ae9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79ae9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79ae9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79ae9-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="79ae9-119">Optional query parameters</span></span>
<span data-ttu-id="79ae9-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="79ae9-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79ae9-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79ae9-121">Request headers</span></span>
|<span data-ttu-id="79ae9-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79ae9-122">Header</span></span>|<span data-ttu-id="79ae9-123">値</span><span class="sxs-lookup"><span data-stu-id="79ae9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79ae9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="79ae9-124">Authorization</span></span>|<span data-ttu-id="79ae9-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="79ae9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79ae9-126">承諾</span><span class="sxs-lookup"><span data-stu-id="79ae9-126">Accept</span></span>|<span data-ttu-id="79ae9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="79ae9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79ae9-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="79ae9-128">Request body</span></span>
<span data-ttu-id="79ae9-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="79ae9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79ae9-130">応答</span><span class="sxs-lookup"><span data-stu-id="79ae9-130">Response</span></span>
<span data-ttu-id="79ae9-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="79ae9-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79ae9-132">例</span><span class="sxs-lookup"><span data-stu-id="79ae9-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="79ae9-133">要求</span><span class="sxs-lookup"><span data-stu-id="79ae9-133">Request</span></span>
<span data-ttu-id="79ae9-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="79ae9-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="79ae9-135">応答</span><span class="sxs-lookup"><span data-stu-id="79ae9-135">Response</span></span>
<span data-ttu-id="79ae9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79ae9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 377

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
    "label": "Label value",
    "id": "754d8495-8495-754d-9584-4d7595844d75",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "defaultValue": 12,
    "spin": true,
    "spinStep": 8,
    "required": true,
    "minValue": 8,
    "maxValue": 8
  }
}
```





