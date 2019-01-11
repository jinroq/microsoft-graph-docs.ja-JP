---
title: Get deviceAppManagement
description: deviceAppManagement オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f6e862fa3b0e82d70907fbe903c144c4511fb278
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837773"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="65b49-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="65b49-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="65b49-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="65b49-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65b49-105">[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="65b49-105">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65b49-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="65b49-106">Prerequisites</span></span>

<span data-ttu-id="65b49-107">この API を呼び出すには次のアクセス許可のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="65b49-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="65b49-108">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65b49-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="65b49-109">ワークフローに従って、適切なアクセス許可が異なることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="65b49-109">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="65b49-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65b49-110">Permission type</span></span>|<span data-ttu-id="65b49-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="65b49-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65b49-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65b49-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65b49-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="65b49-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="65b49-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65b49-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65b49-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65b49-115">Not supported.</span></span>|
|<span data-ttu-id="65b49-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65b49-116">Application</span></span>|<span data-ttu-id="65b49-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65b49-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65b49-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65b49-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="65b49-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="65b49-119">Optional query parameters</span></span>
<span data-ttu-id="65b49-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="65b49-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65b49-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65b49-121">Request headers</span></span>
|<span data-ttu-id="65b49-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65b49-122">Header</span></span>|<span data-ttu-id="65b49-123">値</span><span class="sxs-lookup"><span data-stu-id="65b49-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65b49-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="65b49-124">Authorization</span></span>|<span data-ttu-id="65b49-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="65b49-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65b49-126">Accept</span><span class="sxs-lookup"><span data-stu-id="65b49-126">Accept</span></span>|<span data-ttu-id="65b49-127">application/json</span><span class="sxs-lookup"><span data-stu-id="65b49-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65b49-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="65b49-128">Request body</span></span>
<span data-ttu-id="65b49-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="65b49-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65b49-130">応答</span><span class="sxs-lookup"><span data-stu-id="65b49-130">Response</span></span>
<span data-ttu-id="65b49-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="65b49-131">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="65b49-132">要求の例</span><span class="sxs-lookup"><span data-stu-id="65b49-132">Example request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

## <a name="example-response"></a><span data-ttu-id="65b49-133">応答の例</span><span class="sxs-lookup"><span data-stu-id="65b49-133">Example response</span></span>
<span data-ttu-id="65b49-134">ここに示す応答オブジェクトは、簡潔にするために切り詰められます。</span><span class="sxs-lookup"><span data-stu-id="65b49-134">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="65b49-135">すべてのプロパティは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="65b49-135">All properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```



