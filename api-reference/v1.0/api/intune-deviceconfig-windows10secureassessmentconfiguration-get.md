---
title: Get windows10SecureAssessmentConfiguration
description: windows10SecureAssessmentConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dc3030116f5c6274dd60dca24d309ca1c759071a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020109"
---
# <a name="get-windows10secureassessmentconfiguration"></a><span data-ttu-id="9bf0a-103">Get windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="9bf0a-103">Get windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="9bf0a-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9bf0a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bf0a-105">[windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9bf0a-105">Read properties and relationships of the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bf0a-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="9bf0a-106">Prerequisites</span></span>
<span data-ttu-id="9bf0a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9bf0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bf0a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9bf0a-109">Permission type</span></span>|<span data-ttu-id="9bf0a-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9bf0a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bf0a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9bf0a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9bf0a-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bf0a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9bf0a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9bf0a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bf0a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9bf0a-114">Not supported.</span></span>|
|<span data-ttu-id="9bf0a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9bf0a-115">Application</span></span>|<span data-ttu-id="9bf0a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9bf0a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bf0a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9bf0a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9bf0a-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9bf0a-118">Optional query parameters</span></span>
<span data-ttu-id="9bf0a-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9bf0a-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9bf0a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9bf0a-120">Request headers</span></span>
|<span data-ttu-id="9bf0a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9bf0a-121">Header</span></span>|<span data-ttu-id="9bf0a-122">値</span><span class="sxs-lookup"><span data-stu-id="9bf0a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bf0a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bf0a-123">Authorization</span></span>|<span data-ttu-id="9bf0a-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9bf0a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bf0a-125">承諾</span><span class="sxs-lookup"><span data-stu-id="9bf0a-125">Accept</span></span>|<span data-ttu-id="9bf0a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9bf0a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bf0a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9bf0a-127">Request body</span></span>
<span data-ttu-id="9bf0a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9bf0a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bf0a-129">応答</span><span class="sxs-lookup"><span data-stu-id="9bf0a-129">Response</span></span>
<span data-ttu-id="9bf0a-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9bf0a-130">If successful, this method returns a `200 OK` response code and [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bf0a-131">例</span><span class="sxs-lookup"><span data-stu-id="9bf0a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bf0a-132">要求</span><span class="sxs-lookup"><span data-stu-id="9bf0a-132">Request</span></span>
<span data-ttu-id="9bf0a-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9bf0a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="9bf0a-134">応答</span><span class="sxs-lookup"><span data-stu-id="9bf0a-134">Response</span></span>
<span data-ttu-id="9bf0a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9bf0a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
    "id": "f60d71be-71be-f60d-be71-0df6be710df6",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "launchUri": "Launch Uri value",
    "configurationAccount": "Configuration Account value",
    "allowPrinting": true,
    "allowScreenCapture": true,
    "allowTextSuggestion": true
  }
}
```



