---
title: deviceManagementTroubleshootingEvents のリスト
description: deviceManagementTroubleshootingEvent オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 11f8b55dff577f1f8f33a62ec0d2d20db3fc666f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828428"
---
# <a name="list-devicemanagementtroubleshootingevents"></a><span data-ttu-id="40ace-103">deviceManagementTroubleshootingEvents のリスト</span><span class="sxs-lookup"><span data-stu-id="40ace-103">List deviceManagementTroubleshootingEvents</span></span>

> <span data-ttu-id="40ace-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="40ace-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40ace-105">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="40ace-105">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40ace-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="40ace-106">Prerequisites</span></span>
<span data-ttu-id="40ace-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40ace-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40ace-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="40ace-109">Permission type</span></span>|<span data-ttu-id="40ace-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="40ace-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40ace-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="40ace-111">Delegated (work or school account)</span></span>|<span data-ttu-id="40ace-112">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="40ace-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="40ace-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="40ace-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40ace-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40ace-114">Not supported.</span></span>|
|<span data-ttu-id="40ace-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="40ace-115">Application</span></span>|<span data-ttu-id="40ace-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40ace-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40ace-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="40ace-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="40ace-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40ace-118">Request headers</span></span>
|<span data-ttu-id="40ace-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40ace-119">Header</span></span>|<span data-ttu-id="40ace-120">値</span><span class="sxs-lookup"><span data-stu-id="40ace-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40ace-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="40ace-121">Authorization</span></span>|<span data-ttu-id="40ace-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="40ace-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40ace-123">Accept</span><span class="sxs-lookup"><span data-stu-id="40ace-123">Accept</span></span>|<span data-ttu-id="40ace-124">application/json</span><span class="sxs-lookup"><span data-stu-id="40ace-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40ace-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="40ace-125">Request body</span></span>
<span data-ttu-id="40ace-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="40ace-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40ace-127">応答</span><span class="sxs-lookup"><span data-stu-id="40ace-127">Response</span></span>
<span data-ttu-id="40ace-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="40ace-128">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40ace-129">例</span><span class="sxs-lookup"><span data-stu-id="40ace-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="40ace-130">要求</span><span class="sxs-lookup"><span data-stu-id="40ace-130">Request</span></span>
<span data-ttu-id="40ace-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="40ace-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="40ace-132">応答</span><span class="sxs-lookup"><span data-stu-id="40ace-132">Response</span></span>
<span data-ttu-id="40ace-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="40ace-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 277

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
      "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "correlationId": "Correlation Id value"
    }
  ]
}
```



