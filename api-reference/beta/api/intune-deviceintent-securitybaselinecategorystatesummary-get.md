---
title: SecurityBaselineCategoryStateSummary を取得する
description: SecurityBaselineCategoryStateSummary オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 592459b0afb11eb2f0598c9e4fd39d48053840b0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343021"
---
# <a name="get-securitybaselinecategorystatesummary"></a><span data-ttu-id="79da7-103">SecurityBaselineCategoryStateSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="79da7-103">Get securityBaselineCategoryStateSummary</span></span>

> <span data-ttu-id="79da7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79da7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79da7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="79da7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79da7-106">[SecurityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="79da7-106">Read properties and relationships of the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79da7-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="79da7-107">Prerequisites</span></span>
<span data-ttu-id="79da7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79da7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79da7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79da7-110">Permission type</span></span>|<span data-ttu-id="79da7-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="79da7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79da7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79da7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79da7-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79da7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="79da7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79da7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79da7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79da7-115">Not supported.</span></span>|
|<span data-ttu-id="79da7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79da7-116">Application</span></span>|<span data-ttu-id="79da7-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79da7-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79da7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79da7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79da7-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="79da7-119">Optional query parameters</span></span>
<span data-ttu-id="79da7-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="79da7-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79da7-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79da7-121">Request headers</span></span>
|<span data-ttu-id="79da7-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79da7-122">Header</span></span>|<span data-ttu-id="79da7-123">値</span><span class="sxs-lookup"><span data-stu-id="79da7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79da7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="79da7-124">Authorization</span></span>|<span data-ttu-id="79da7-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="79da7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79da7-126">承諾</span><span class="sxs-lookup"><span data-stu-id="79da7-126">Accept</span></span>|<span data-ttu-id="79da7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="79da7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79da7-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="79da7-128">Request body</span></span>
<span data-ttu-id="79da7-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="79da7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79da7-130">応答</span><span class="sxs-lookup"><span data-stu-id="79da7-130">Response</span></span>
<span data-ttu-id="79da7-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="79da7-131">If successful, this method returns a `200 OK` response code and [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79da7-132">例</span><span class="sxs-lookup"><span data-stu-id="79da7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="79da7-133">要求</span><span class="sxs-lookup"><span data-stu-id="79da7-133">Request</span></span>
<span data-ttu-id="79da7-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="79da7-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="79da7-135">応答</span><span class="sxs-lookup"><span data-stu-id="79da7-135">Response</span></span>
<span data-ttu-id="79da7-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79da7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 347

{
  "value": {
    "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
    "id": "7a650997-0997-7a65-9709-657a9709657a",
    "secureCount": 11,
    "notSecureCount": 14,
    "unknownCount": 12,
    "errorCount": 10,
    "conflictCount": 13,
    "notApplicableCount": 2,
    "displayName": "Display Name value"
  }
}
```






