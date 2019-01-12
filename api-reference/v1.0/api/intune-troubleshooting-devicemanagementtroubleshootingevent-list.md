---
title: deviceManagementTroubleshootingEvents のリスト
description: deviceManagementTroubleshootingEvent オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b6ab19d049268b0880789b73e9900e3e8ad784a0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986839"
---
# <a name="list-devicemanagementtroubleshootingevents"></a><span data-ttu-id="17897-103">deviceManagementTroubleshootingEvents のリスト</span><span class="sxs-lookup"><span data-stu-id="17897-103">List deviceManagementTroubleshootingEvents</span></span>

> <span data-ttu-id="17897-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="17897-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17897-105">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="17897-105">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="17897-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="17897-106">Prerequisites</span></span>
<span data-ttu-id="17897-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="17897-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17897-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="17897-109">Permission type</span></span>|<span data-ttu-id="17897-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="17897-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17897-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="17897-111">Delegated (work or school account)</span></span>|<span data-ttu-id="17897-112">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="17897-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="17897-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="17897-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17897-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17897-114">Not supported.</span></span>|
|<span data-ttu-id="17897-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="17897-115">Application</span></span>|<span data-ttu-id="17897-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17897-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17897-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="17897-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="17897-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="17897-118">Request headers</span></span>
|<span data-ttu-id="17897-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="17897-119">Header</span></span>|<span data-ttu-id="17897-120">値</span><span class="sxs-lookup"><span data-stu-id="17897-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17897-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="17897-121">Authorization</span></span>|<span data-ttu-id="17897-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="17897-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17897-123">Accept</span><span class="sxs-lookup"><span data-stu-id="17897-123">Accept</span></span>|<span data-ttu-id="17897-124">application/json</span><span class="sxs-lookup"><span data-stu-id="17897-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17897-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="17897-125">Request body</span></span>
<span data-ttu-id="17897-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="17897-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17897-127">応答</span><span class="sxs-lookup"><span data-stu-id="17897-127">Response</span></span>
<span data-ttu-id="17897-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="17897-128">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17897-129">例</span><span class="sxs-lookup"><span data-stu-id="17897-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="17897-130">要求</span><span class="sxs-lookup"><span data-stu-id="17897-130">Request</span></span>
<span data-ttu-id="17897-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="17897-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="17897-132">応答</span><span class="sxs-lookup"><span data-stu-id="17897-132">Response</span></span>
<span data-ttu-id="17897-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="17897-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



