---
title: deviceManagementExchangeOnPremisesPolicy を取得する
description: deviceManagementExchangeOnPremisesPolicy オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29d8bc5184c492238da55f0af19a1cc74f6b81bc
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984227"
---
# <a name="get-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="f6496-103">deviceManagementExchangeOnPremisesPolicy を取得する</span><span class="sxs-lookup"><span data-stu-id="f6496-103">Get deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="f6496-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6496-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6496-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f6496-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6496-106">[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f6496-106">Read properties and relationships of the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6496-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f6496-107">Prerequisites</span></span>
<span data-ttu-id="f6496-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f6496-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6496-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f6496-110">Permission type</span></span>|<span data-ttu-id="f6496-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f6496-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6496-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f6496-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6496-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6496-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f6496-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f6496-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6496-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6496-115">Not supported.</span></span>|
|<span data-ttu-id="f6496-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f6496-116">Application</span></span>|<span data-ttu-id="f6496-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6496-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6496-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f6496-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeOnPremisesPolicy
GET /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6496-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f6496-119">Optional query parameters</span></span>
<span data-ttu-id="f6496-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f6496-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6496-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6496-121">Request headers</span></span>
|<span data-ttu-id="f6496-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6496-122">Header</span></span>|<span data-ttu-id="f6496-123">値</span><span class="sxs-lookup"><span data-stu-id="f6496-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6496-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6496-124">Authorization</span></span>|<span data-ttu-id="f6496-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f6496-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6496-126">承諾</span><span class="sxs-lookup"><span data-stu-id="f6496-126">Accept</span></span>|<span data-ttu-id="f6496-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f6496-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6496-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="f6496-128">Request body</span></span>
<span data-ttu-id="f6496-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f6496-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6496-130">応答</span><span class="sxs-lookup"><span data-stu-id="f6496-130">Response</span></span>
<span data-ttu-id="f6496-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f6496-131">If successful, this method returns a `200 OK` response code and [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6496-132">例</span><span class="sxs-lookup"><span data-stu-id="f6496-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6496-133">要求</span><span class="sxs-lookup"><span data-stu-id="f6496-133">Request</span></span>
<span data-ttu-id="f6496-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f6496-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
```

### <a name="response"></a><span data-ttu-id="f6496-135">応答</span><span class="sxs-lookup"><span data-stu-id="f6496-135">Response</span></span>
<span data-ttu-id="f6496-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f6496-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 777

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
    "id": "16e76336-6336-16e7-3663-e7163663e716",
    "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
    "defaultAccessLevel": "allow",
    "accessRules": [
      {
        "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
        "deviceClass": {
          "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
          "name": "Name value",
          "type": "model"
        },
        "accessLevel": "allow"
      }
    ],
    "knownDeviceClasses": [
      {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      }
    ]
  }
}
```




