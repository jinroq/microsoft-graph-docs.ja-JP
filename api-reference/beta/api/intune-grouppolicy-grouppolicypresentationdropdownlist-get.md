---
title: GroupPolicyPresentationDropdownList の取得
description: GroupPolicyPresentationDropdownList オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d13884a30bbe63da3dca2bc0499f0dfb50802878
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35989575"
---
# <a name="get-grouppolicypresentationdropdownlist"></a><span data-ttu-id="bdfc2-103">GroupPolicyPresentationDropdownList の取得</span><span class="sxs-lookup"><span data-stu-id="bdfc2-103">Get groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="bdfc2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bdfc2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdfc2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bdfc2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdfc2-106">[Grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bdfc2-106">Read properties and relationships of the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bdfc2-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="bdfc2-107">Prerequisites</span></span>
<span data-ttu-id="bdfc2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bdfc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdfc2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bdfc2-110">Permission type</span></span>|<span data-ttu-id="bdfc2-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bdfc2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdfc2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bdfc2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bdfc2-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdfc2-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="bdfc2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bdfc2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdfc2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bdfc2-115">Not supported.</span></span>|
|<span data-ttu-id="bdfc2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bdfc2-116">Application</span></span>|<span data-ttu-id="bdfc2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bdfc2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdfc2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bdfc2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bdfc2-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bdfc2-119">Optional query parameters</span></span>
<span data-ttu-id="bdfc2-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bdfc2-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bdfc2-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bdfc2-121">Request headers</span></span>
|<span data-ttu-id="bdfc2-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bdfc2-122">Header</span></span>|<span data-ttu-id="bdfc2-123">値</span><span class="sxs-lookup"><span data-stu-id="bdfc2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdfc2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdfc2-124">Authorization</span></span>|<span data-ttu-id="bdfc2-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="bdfc2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdfc2-126">承諾</span><span class="sxs-lookup"><span data-stu-id="bdfc2-126">Accept</span></span>|<span data-ttu-id="bdfc2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bdfc2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdfc2-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="bdfc2-128">Request body</span></span>
<span data-ttu-id="bdfc2-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bdfc2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdfc2-130">応答</span><span class="sxs-lookup"><span data-stu-id="bdfc2-130">Response</span></span>
<span data-ttu-id="bdfc2-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bdfc2-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdfc2-132">例</span><span class="sxs-lookup"><span data-stu-id="bdfc2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdfc2-133">要求</span><span class="sxs-lookup"><span data-stu-id="bdfc2-133">Request</span></span>
<span data-ttu-id="bdfc2-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bdfc2-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="bdfc2-135">応答</span><span class="sxs-lookup"><span data-stu-id="bdfc2-135">Response</span></span>
<span data-ttu-id="bdfc2-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bdfc2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 655

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
    "label": "Label value",
    "id": "ba3ff7c9-f7c9-ba3f-c9f7-3fbac9f73fba",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "defaultItem": {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "Display Name value",
      "value": "Value value"
    },
    "items": [
      {
        "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
        "displayName": "Display Name value",
        "value": "Value value"
      }
    ],
    "required": true
  }
}
```





