---
title: devicemanagementtemplatesettingcategory の取得
description: devicemanagementtemplatesettingcategory オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1e371b9342e2193c530fabb2991fcd13b98adfa2
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522434"
---
# <a name="get-devicemanagementtemplatesettingcategory"></a><span data-ttu-id="dea65-103">devicemanagementtemplatesettingcategory の取得</span><span class="sxs-lookup"><span data-stu-id="dea65-103">Get deviceManagementTemplateSettingCategory</span></span>

> <span data-ttu-id="dea65-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dea65-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dea65-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dea65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dea65-106">[devicemanagementtemplatesettingcategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dea65-106">Read properties and relationships of the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dea65-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="dea65-107">Prerequisites</span></span>
<span data-ttu-id="dea65-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dea65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dea65-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dea65-110">Permission type</span></span>|<span data-ttu-id="dea65-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dea65-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dea65-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dea65-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dea65-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dea65-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dea65-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dea65-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dea65-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dea65-115">Not supported.</span></span>|
|<span data-ttu-id="dea65-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dea65-116">Application</span></span>|<span data-ttu-id="dea65-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dea65-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dea65-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dea65-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dea65-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="dea65-119">Optional query parameters</span></span>
<span data-ttu-id="dea65-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="dea65-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dea65-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dea65-121">Request headers</span></span>
|<span data-ttu-id="dea65-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dea65-122">Header</span></span>|<span data-ttu-id="dea65-123">値</span><span class="sxs-lookup"><span data-stu-id="dea65-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dea65-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dea65-124">Authorization</span></span>|<span data-ttu-id="dea65-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="dea65-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dea65-126">承諾</span><span class="sxs-lookup"><span data-stu-id="dea65-126">Accept</span></span>|<span data-ttu-id="dea65-127">application/json</span><span class="sxs-lookup"><span data-stu-id="dea65-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dea65-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="dea65-128">Request body</span></span>
<span data-ttu-id="dea65-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dea65-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dea65-130">応答</span><span class="sxs-lookup"><span data-stu-id="dea65-130">Response</span></span>
<span data-ttu-id="dea65-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[devicemanagementtemplatesettingcategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dea65-131">If successful, this method returns a `200 OK` response code and [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dea65-132">例</span><span class="sxs-lookup"><span data-stu-id="dea65-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="dea65-133">要求</span><span class="sxs-lookup"><span data-stu-id="dea65-133">Request</span></span>
<span data-ttu-id="dea65-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dea65-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}
```

### <a name="response"></a><span data-ttu-id="dea65-135">応答</span><span class="sxs-lookup"><span data-stu-id="dea65-135">Response</span></span>
<span data-ttu-id="dea65-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dea65-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 195

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
    "id": "cd213562-3562-cd21-6235-21cd623521cd",
    "displayName": "Display Name value"
  }
}
```







