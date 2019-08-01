---
title: Get termsAndConditionsAcceptanceStatus
description: termsAndConditionsAcceptanceStatus オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3b75725b109b2b68eae72679a17c46537b01fa07
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019843"
---
# <a name="get-termsandconditionsacceptancestatus"></a><span data-ttu-id="00da8-103">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="00da8-103">Get termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="00da8-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="00da8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00da8-105">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="00da8-105">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00da8-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="00da8-106">Prerequisites</span></span>
<span data-ttu-id="00da8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00da8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00da8-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="00da8-109">Permission type</span></span>|<span data-ttu-id="00da8-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="00da8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00da8-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="00da8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="00da8-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="00da8-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="00da8-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="00da8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00da8-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00da8-114">Not supported.</span></span>|
|<span data-ttu-id="00da8-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="00da8-115">Application</span></span>|<span data-ttu-id="00da8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00da8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00da8-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="00da8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00da8-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="00da8-118">Optional query parameters</span></span>
<span data-ttu-id="00da8-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="00da8-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="00da8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00da8-120">Request headers</span></span>
|<span data-ttu-id="00da8-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00da8-121">Header</span></span>|<span data-ttu-id="00da8-122">値</span><span class="sxs-lookup"><span data-stu-id="00da8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00da8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="00da8-123">Authorization</span></span>|<span data-ttu-id="00da8-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="00da8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00da8-125">承諾</span><span class="sxs-lookup"><span data-stu-id="00da8-125">Accept</span></span>|<span data-ttu-id="00da8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00da8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00da8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="00da8-127">Request body</span></span>
<span data-ttu-id="00da8-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="00da8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00da8-129">応答</span><span class="sxs-lookup"><span data-stu-id="00da8-129">Response</span></span>
<span data-ttu-id="00da8-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="00da8-130">If successful, this method returns a `200 OK` response code and [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00da8-131">例</span><span class="sxs-lookup"><span data-stu-id="00da8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="00da8-132">要求</span><span class="sxs-lookup"><span data-stu-id="00da8-132">Request</span></span>
<span data-ttu-id="00da8-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="00da8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

### <a name="response"></a><span data-ttu-id="00da8-134">応答</span><span class="sxs-lookup"><span data-stu-id="00da8-134">Response</span></span>
<span data-ttu-id="00da8-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="00da8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 289

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
    "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
    "userDisplayName": "User Display Name value",
    "acceptedVersion": 15,
    "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
  }
}
```



