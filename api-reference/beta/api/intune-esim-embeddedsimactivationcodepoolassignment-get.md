---
title: EmbeddedSIMActivationCodePoolAssignment を取得する
description: EmbeddedSIMActivationCodePoolAssignment オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c6a58d4c276daac470cadc7db831be76132f08fb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34982575"
---
# <a name="get-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="f6c2e-103">EmbeddedSIMActivationCodePoolAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="f6c2e-103">Get embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="f6c2e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6c2e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6c2e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f6c2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6c2e-106">[EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f6c2e-106">Read properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6c2e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f6c2e-107">Prerequisites</span></span>
<span data-ttu-id="f6c2e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f6c2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6c2e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f6c2e-110">Permission type</span></span>|<span data-ttu-id="f6c2e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f6c2e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6c2e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f6c2e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6c2e-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6c2e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f6c2e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f6c2e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6c2e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6c2e-115">Not supported.</span></span>|
|<span data-ttu-id="f6c2e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f6c2e-116">Application</span></span>|<span data-ttu-id="f6c2e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6c2e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6c2e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f6c2e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6c2e-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f6c2e-119">Optional query parameters</span></span>
<span data-ttu-id="f6c2e-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f6c2e-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6c2e-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6c2e-121">Request headers</span></span>
|<span data-ttu-id="f6c2e-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6c2e-122">Header</span></span>|<span data-ttu-id="f6c2e-123">値</span><span class="sxs-lookup"><span data-stu-id="f6c2e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6c2e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6c2e-124">Authorization</span></span>|<span data-ttu-id="f6c2e-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f6c2e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6c2e-126">承諾</span><span class="sxs-lookup"><span data-stu-id="f6c2e-126">Accept</span></span>|<span data-ttu-id="f6c2e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f6c2e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6c2e-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="f6c2e-128">Request body</span></span>
<span data-ttu-id="f6c2e-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f6c2e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6c2e-130">応答</span><span class="sxs-lookup"><span data-stu-id="f6c2e-130">Response</span></span>
<span data-ttu-id="f6c2e-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f6c2e-131">If successful, this method returns a `200 OK` response code and [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6c2e-132">例</span><span class="sxs-lookup"><span data-stu-id="f6c2e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6c2e-133">要求</span><span class="sxs-lookup"><span data-stu-id="f6c2e-133">Request</span></span>
<span data-ttu-id="f6c2e-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f6c2e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

### <a name="response"></a><span data-ttu-id="f6c2e-135">応答</span><span class="sxs-lookup"><span data-stu-id="f6c2e-135">Response</span></span>
<span data-ttu-id="f6c2e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f6c2e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 257

{
  "value": {
    "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
    "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```





