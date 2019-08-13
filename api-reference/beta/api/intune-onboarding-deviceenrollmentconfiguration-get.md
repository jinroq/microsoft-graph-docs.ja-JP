---
title: deviceEnrollmentConfiguration の取得
description: deviceEnrollmentConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5257331b2d39397389e9f8ea53206ef34adec136
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36353065"
---
# <a name="get-deviceenrollmentconfiguration"></a><span data-ttu-id="e1689-103">deviceEnrollmentConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="e1689-103">Get deviceEnrollmentConfiguration</span></span>

> <span data-ttu-id="e1689-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1689-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1689-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e1689-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1689-106">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e1689-106">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1689-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e1689-107">Prerequisites</span></span>
<span data-ttu-id="e1689-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1689-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1689-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e1689-110">Permission type</span></span>|<span data-ttu-id="e1689-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e1689-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1689-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e1689-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1689-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1689-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e1689-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e1689-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1689-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1689-115">Not supported.</span></span>|
|<span data-ttu-id="e1689-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e1689-116">Application</span></span>|<span data-ttu-id="e1689-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1689-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1689-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e1689-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1689-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e1689-119">Optional query parameters</span></span>
<span data-ttu-id="e1689-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e1689-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1689-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1689-121">Request headers</span></span>
|<span data-ttu-id="e1689-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1689-122">Header</span></span>|<span data-ttu-id="e1689-123">値</span><span class="sxs-lookup"><span data-stu-id="e1689-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1689-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1689-124">Authorization</span></span>|<span data-ttu-id="e1689-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e1689-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1689-126">承諾</span><span class="sxs-lookup"><span data-stu-id="e1689-126">Accept</span></span>|<span data-ttu-id="e1689-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e1689-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1689-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e1689-128">Request body</span></span>
<span data-ttu-id="e1689-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e1689-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1689-130">応答</span><span class="sxs-lookup"><span data-stu-id="e1689-130">Response</span></span>
<span data-ttu-id="e1689-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e1689-131">If successful, this method returns a `200 OK` response code and [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1689-132">例</span><span class="sxs-lookup"><span data-stu-id="e1689-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1689-133">要求</span><span class="sxs-lookup"><span data-stu-id="e1689-133">Request</span></span>
<span data-ttu-id="e1689-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e1689-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e1689-135">応答</span><span class="sxs-lookup"><span data-stu-id="e1689-135">Response</span></span>
<span data-ttu-id="e1689-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e1689-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 392

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
    "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
    "displayName": "Display Name value",
    "description": "Description value",
    "priority": 8,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7
  }
}
```






