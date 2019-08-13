---
title: GroupPolicyPresentationListBox の取得
description: GroupPolicyPresentationListBox オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8587f9def83a05d39ad89dae695b0f4c7a0a6312
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357797"
---
# <a name="get-grouppolicypresentationlistbox"></a><span data-ttu-id="2ce2d-103">GroupPolicyPresentationListBox の取得</span><span class="sxs-lookup"><span data-stu-id="2ce2d-103">Get groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="2ce2d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ce2d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ce2d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2ce2d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ce2d-106">[Grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2ce2d-106">Read properties and relationships of the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ce2d-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2ce2d-107">Prerequisites</span></span>
<span data-ttu-id="2ce2d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ce2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ce2d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2ce2d-110">Permission type</span></span>|<span data-ttu-id="2ce2d-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2ce2d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ce2d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2ce2d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ce2d-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ce2d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2ce2d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2ce2d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ce2d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ce2d-115">Not supported.</span></span>|
|<span data-ttu-id="2ce2d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2ce2d-116">Application</span></span>|<span data-ttu-id="2ce2d-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ce2d-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ce2d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2ce2d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ce2d-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2ce2d-119">Optional query parameters</span></span>
<span data-ttu-id="2ce2d-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2ce2d-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ce2d-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ce2d-121">Request headers</span></span>
|<span data-ttu-id="2ce2d-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ce2d-122">Header</span></span>|<span data-ttu-id="2ce2d-123">値</span><span class="sxs-lookup"><span data-stu-id="2ce2d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ce2d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ce2d-124">Authorization</span></span>|<span data-ttu-id="2ce2d-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2ce2d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ce2d-126">承諾</span><span class="sxs-lookup"><span data-stu-id="2ce2d-126">Accept</span></span>|<span data-ttu-id="2ce2d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2ce2d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ce2d-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="2ce2d-128">Request body</span></span>
<span data-ttu-id="2ce2d-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2ce2d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ce2d-130">応答</span><span class="sxs-lookup"><span data-stu-id="2ce2d-130">Response</span></span>
<span data-ttu-id="2ce2d-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2ce2d-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ce2d-132">例</span><span class="sxs-lookup"><span data-stu-id="2ce2d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ce2d-133">要求</span><span class="sxs-lookup"><span data-stu-id="2ce2d-133">Request</span></span>
<span data-ttu-id="2ce2d-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2ce2d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="2ce2d-135">応答</span><span class="sxs-lookup"><span data-stu-id="2ce2d-135">Response</span></span>
<span data-ttu-id="2ce2d-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2ce2d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 309

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
    "label": "Label value",
    "id": "2e074c87-4c87-2e07-874c-072e874c072e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "explicitValue": true,
    "valuePrefix": "Value Prefix value"
  }
}
```






