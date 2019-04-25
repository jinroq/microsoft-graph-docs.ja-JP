---
title: groupPolicyPresentationValueLongDecimal を取得する
description: groupPolicyPresentationValueLongDecimal オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 55ba50d6d2848fcf9d3d019dad522667642ccb4e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32530677"
---
# <a name="get-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="3e738-103">groupPolicyPresentationValueLongDecimal を取得する</span><span class="sxs-lookup"><span data-stu-id="3e738-103">Get groupPolicyPresentationValueLongDecimal</span></span>

> <span data-ttu-id="3e738-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e738-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e738-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3e738-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e738-106">[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3e738-106">Read properties and relationships of the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e738-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3e738-107">Prerequisites</span></span>
<span data-ttu-id="3e738-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3e738-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e738-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3e738-110">Permission type</span></span>|<span data-ttu-id="3e738-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3e738-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e738-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3e738-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3e738-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e738-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3e738-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3e738-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e738-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e738-115">Not supported.</span></span>|
|<span data-ttu-id="3e738-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3e738-116">Application</span></span>|<span data-ttu-id="3e738-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e738-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e738-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3e738-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e738-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3e738-119">Optional query parameters</span></span>
<span data-ttu-id="3e738-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3e738-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e738-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3e738-121">Request headers</span></span>
|<span data-ttu-id="3e738-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3e738-122">Header</span></span>|<span data-ttu-id="3e738-123">値</span><span class="sxs-lookup"><span data-stu-id="3e738-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e738-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e738-124">Authorization</span></span>|<span data-ttu-id="3e738-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3e738-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e738-126">承諾</span><span class="sxs-lookup"><span data-stu-id="3e738-126">Accept</span></span>|<span data-ttu-id="3e738-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3e738-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e738-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="3e738-128">Request body</span></span>
<span data-ttu-id="3e738-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3e738-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e738-130">応答</span><span class="sxs-lookup"><span data-stu-id="3e738-130">Response</span></span>
<span data-ttu-id="3e738-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3e738-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e738-132">例</span><span class="sxs-lookup"><span data-stu-id="3e738-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e738-133">要求</span><span class="sxs-lookup"><span data-stu-id="3e738-133">Request</span></span>
<span data-ttu-id="3e738-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3e738-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

### <a name="response"></a><span data-ttu-id="3e738-135">応答</span><span class="sxs-lookup"><span data-stu-id="3e738-135">Response</span></span>
<span data-ttu-id="3e738-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3e738-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 297

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "id": "210f7078-7078-210f-7870-0f2178700f21",
    "value": 5
  }
}
```





