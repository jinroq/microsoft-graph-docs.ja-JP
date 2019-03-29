---
title: grouppolicypresentationtextbox の取得
description: grouppolicypresentationtextbox オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2894e7852802b0d6b1b560ae09bceb51dce37231
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971095"
---
# <a name="get-grouppolicypresentationtextbox"></a><span data-ttu-id="8eddb-103">grouppolicypresentationtextbox の取得</span><span class="sxs-lookup"><span data-stu-id="8eddb-103">Get groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="8eddb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8eddb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8eddb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8eddb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8eddb-106">[grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8eddb-106">Read properties and relationships of the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8eddb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8eddb-107">Prerequisites</span></span>
<span data-ttu-id="8eddb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8eddb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8eddb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8eddb-110">Permission type</span></span>|<span data-ttu-id="8eddb-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8eddb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8eddb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8eddb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8eddb-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8eddb-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8eddb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8eddb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8eddb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8eddb-115">Not supported.</span></span>|
|<span data-ttu-id="8eddb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8eddb-116">Application</span></span>|<span data-ttu-id="8eddb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8eddb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8eddb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8eddb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8eddb-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8eddb-119">Optional query parameters</span></span>
<span data-ttu-id="8eddb-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8eddb-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8eddb-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8eddb-121">Request headers</span></span>
|<span data-ttu-id="8eddb-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8eddb-122">Header</span></span>|<span data-ttu-id="8eddb-123">値</span><span class="sxs-lookup"><span data-stu-id="8eddb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8eddb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8eddb-124">Authorization</span></span>|<span data-ttu-id="8eddb-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8eddb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8eddb-126">承諾</span><span class="sxs-lookup"><span data-stu-id="8eddb-126">Accept</span></span>|<span data-ttu-id="8eddb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8eddb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8eddb-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="8eddb-128">Request body</span></span>
<span data-ttu-id="8eddb-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8eddb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8eddb-130">応答</span><span class="sxs-lookup"><span data-stu-id="8eddb-130">Response</span></span>
<span data-ttu-id="8eddb-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8eddb-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8eddb-132">例</span><span class="sxs-lookup"><span data-stu-id="8eddb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8eddb-133">要求</span><span class="sxs-lookup"><span data-stu-id="8eddb-133">Request</span></span>
<span data-ttu-id="8eddb-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8eddb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="8eddb-135">応答</span><span class="sxs-lookup"><span data-stu-id="8eddb-135">Response</span></span>
<span data-ttu-id="8eddb-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8eddb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 327

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
    "label": "Label value",
    "id": "ec80633e-633e-ec80-3e63-80ec3e6380ec",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "defaultValue": "Default Value value",
    "required": true,
    "maxLength": 9
  }
}
```




