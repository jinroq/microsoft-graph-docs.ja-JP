---
title: deviceManagementTroubleshootingEvents のリスト
description: deviceManagementTroubleshootingEvent オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37ffbb1d049f3a675c115e15a1784baf200866ed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507778"
---
# <a name="list-devicemanagementtroubleshootingevents"></a><span data-ttu-id="06550-103">deviceManagementTroubleshootingEvents のリスト</span><span class="sxs-lookup"><span data-stu-id="06550-103">List deviceManagementTroubleshootingEvents</span></span>

> <span data-ttu-id="06550-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06550-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06550-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="06550-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06550-106">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="06550-106">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06550-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="06550-107">Prerequisites</span></span>
<span data-ttu-id="06550-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06550-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06550-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="06550-110">Permission type</span></span>|<span data-ttu-id="06550-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="06550-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06550-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="06550-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06550-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="06550-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="06550-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="06550-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06550-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06550-115">Not supported.</span></span>|
|<span data-ttu-id="06550-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="06550-116">Application</span></span>|<span data-ttu-id="06550-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06550-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06550-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="06550-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="06550-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="06550-119">Request headers</span></span>
|<span data-ttu-id="06550-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="06550-120">Header</span></span>|<span data-ttu-id="06550-121">値</span><span class="sxs-lookup"><span data-stu-id="06550-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06550-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="06550-122">Authorization</span></span>|<span data-ttu-id="06550-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="06550-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06550-124">承諾</span><span class="sxs-lookup"><span data-stu-id="06550-124">Accept</span></span>|<span data-ttu-id="06550-125">application/json</span><span class="sxs-lookup"><span data-stu-id="06550-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06550-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="06550-126">Request body</span></span>
<span data-ttu-id="06550-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="06550-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06550-128">応答</span><span class="sxs-lookup"><span data-stu-id="06550-128">Response</span></span>
<span data-ttu-id="06550-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="06550-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06550-130">例</span><span class="sxs-lookup"><span data-stu-id="06550-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="06550-131">要求</span><span class="sxs-lookup"><span data-stu-id="06550-131">Request</span></span>
<span data-ttu-id="06550-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="06550-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="06550-133">応答</span><span class="sxs-lookup"><span data-stu-id="06550-133">Response</span></span>
<span data-ttu-id="06550-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="06550-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1038

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
      "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "correlationId": "Correlation Id value",
      "troubleshootingErrorDetails": {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
        "context": "Context value",
        "failure": "Failure value",
        "failureDetails": "Failure Details value",
        "remediation": "Remediation value",
        "resources": [
          {
            "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
            "text": "Text value",
            "link": "Link value"
          }
        ]
      },
      "eventName": "Event Name value",
      "additionalInformation": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```



