---
title: Get deviceManagementTroubleshootingEvent
description: deviceManagementTroubleshootingEvent オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3a2de223a416964cb4562fae9ec3851ea8fe24c7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025695"
---
# <a name="get-devicemanagementtroubleshootingevent"></a><span data-ttu-id="0d428-103">Get deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="0d428-103">Get deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="0d428-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0d428-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d428-105">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0d428-105">Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d428-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="0d428-106">Prerequisites</span></span>
<span data-ttu-id="0d428-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0d428-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d428-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0d428-109">Permission type</span></span>|<span data-ttu-id="0d428-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0d428-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d428-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0d428-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0d428-112">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d428-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="0d428-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0d428-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d428-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d428-114">Not supported.</span></span>|
|<span data-ttu-id="0d428-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0d428-115">Application</span></span>|<span data-ttu-id="0d428-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d428-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d428-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0d428-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0d428-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0d428-118">Optional query parameters</span></span>
<span data-ttu-id="0d428-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0d428-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d428-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d428-120">Request headers</span></span>
|<span data-ttu-id="0d428-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d428-121">Header</span></span>|<span data-ttu-id="0d428-122">値</span><span class="sxs-lookup"><span data-stu-id="0d428-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d428-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d428-123">Authorization</span></span>|<span data-ttu-id="0d428-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0d428-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d428-125">承諾</span><span class="sxs-lookup"><span data-stu-id="0d428-125">Accept</span></span>|<span data-ttu-id="0d428-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d428-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d428-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0d428-127">Request body</span></span>
<span data-ttu-id="0d428-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0d428-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d428-129">応答</span><span class="sxs-lookup"><span data-stu-id="0d428-129">Response</span></span>
<span data-ttu-id="0d428-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0d428-130">If successful, this method returns a `200 OK` response code and [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d428-131">例</span><span class="sxs-lookup"><span data-stu-id="0d428-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d428-132">要求</span><span class="sxs-lookup"><span data-stu-id="0d428-132">Request</span></span>
<span data-ttu-id="0d428-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0d428-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="0d428-134">応答</span><span class="sxs-lookup"><span data-stu-id="0d428-134">Response</span></span>
<span data-ttu-id="0d428-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0d428-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 255

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
    "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
    "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
    "correlationId": "Correlation Id value"
  }
}
```



