---
title: termsAndConditionsAssignment の取得
description: termsAndConditionsAssignment オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 03b8b40d0e756fc20d5a2f876ae61c9084c94248
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020424"
---
# <a name="get-termsandconditionsassignment"></a><span data-ttu-id="d6d7b-103">termsAndConditionsAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="d6d7b-103">Get termsAndConditionsAssignment</span></span>

> <span data-ttu-id="d6d7b-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d6d7b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6d7b-105">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d6d7b-105">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6d7b-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="d6d7b-106">Prerequisites</span></span>
<span data-ttu-id="d6d7b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6d7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6d7b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d6d7b-109">Permission type</span></span>|<span data-ttu-id="d6d7b-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d6d7b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6d7b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d6d7b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d6d7b-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6d7b-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d6d7b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d6d7b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6d7b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6d7b-114">Not supported.</span></span>|
|<span data-ttu-id="d6d7b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d6d7b-115">Application</span></span>|<span data-ttu-id="d6d7b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6d7b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6d7b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d6d7b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6d7b-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d6d7b-118">Optional query parameters</span></span>
<span data-ttu-id="d6d7b-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d6d7b-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6d7b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6d7b-120">Request headers</span></span>
|<span data-ttu-id="d6d7b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6d7b-121">Header</span></span>|<span data-ttu-id="d6d7b-122">値</span><span class="sxs-lookup"><span data-stu-id="d6d7b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6d7b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6d7b-123">Authorization</span></span>|<span data-ttu-id="d6d7b-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d6d7b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6d7b-125">承諾</span><span class="sxs-lookup"><span data-stu-id="d6d7b-125">Accept</span></span>|<span data-ttu-id="d6d7b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6d7b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6d7b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d6d7b-127">Request body</span></span>
<span data-ttu-id="d6d7b-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d6d7b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6d7b-129">応答</span><span class="sxs-lookup"><span data-stu-id="d6d7b-129">Response</span></span>
<span data-ttu-id="d6d7b-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d6d7b-130">If successful, this method returns a `200 OK` response code and [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6d7b-131">例</span><span class="sxs-lookup"><span data-stu-id="d6d7b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6d7b-132">要求</span><span class="sxs-lookup"><span data-stu-id="d6d7b-132">Request</span></span>
<span data-ttu-id="d6d7b-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d6d7b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

### <a name="response"></a><span data-ttu-id="d6d7b-134">応答</span><span class="sxs-lookup"><span data-stu-id="d6d7b-134">Response</span></span>
<span data-ttu-id="d6d7b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d6d7b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 246

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
    "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```



