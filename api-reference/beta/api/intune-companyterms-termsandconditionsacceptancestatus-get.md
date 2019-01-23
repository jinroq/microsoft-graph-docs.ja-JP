---
title: Get termsAndConditionsAcceptanceStatus
description: termsAndConditionsAcceptanceStatus オブジェクトのプロパティとリレーションシップを読み取ります。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bd5f5bd201d4b008e4ad0d0bad7e65e724394eaa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418289"
---
# <a name="get-termsandconditionsacceptancestatus"></a><span data-ttu-id="16e3b-103">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="16e3b-103">Get termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="16e3b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="16e3b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="16e3b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16e3b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16e3b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="16e3b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16e3b-107">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="16e3b-107">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16e3b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="16e3b-108">Prerequisites</span></span>
<span data-ttu-id="16e3b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16e3b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="16e3b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16e3b-111">Permission type</span></span>|<span data-ttu-id="16e3b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="16e3b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16e3b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16e3b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16e3b-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="16e3b-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="16e3b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16e3b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16e3b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16e3b-116">Not supported.</span></span>|
|<span data-ttu-id="16e3b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16e3b-117">Application</span></span>|<span data-ttu-id="16e3b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16e3b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16e3b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16e3b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16e3b-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="16e3b-120">Optional query parameters</span></span>
<span data-ttu-id="16e3b-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="16e3b-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16e3b-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16e3b-122">Request headers</span></span>
|<span data-ttu-id="16e3b-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16e3b-123">Header</span></span>|<span data-ttu-id="16e3b-124">値</span><span class="sxs-lookup"><span data-stu-id="16e3b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16e3b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="16e3b-125">Authorization</span></span>|<span data-ttu-id="16e3b-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="16e3b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16e3b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="16e3b-127">Accept</span></span>|<span data-ttu-id="16e3b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="16e3b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16e3b-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="16e3b-129">Request body</span></span>
<span data-ttu-id="16e3b-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="16e3b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16e3b-131">応答</span><span class="sxs-lookup"><span data-stu-id="16e3b-131">Response</span></span>
<span data-ttu-id="16e3b-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="16e3b-132">If successful, this method returns a `200 OK` response code and [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16e3b-133">例</span><span class="sxs-lookup"><span data-stu-id="16e3b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="16e3b-134">要求</span><span class="sxs-lookup"><span data-stu-id="16e3b-134">Request</span></span>
<span data-ttu-id="16e3b-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="16e3b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

### <a name="response"></a><span data-ttu-id="16e3b-136">応答</span><span class="sxs-lookup"><span data-stu-id="16e3b-136">Response</span></span>
<span data-ttu-id="16e3b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="16e3b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




