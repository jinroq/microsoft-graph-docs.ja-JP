---
title: deviceManagementTroubleshootingEvent の作成
description: 新しい deviceManagementTroubleshootingEvent オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d03c31c0bc60aa52bdf40db13a6f3e224c5b64c6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990884"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="b6a8e-103">deviceManagementTroubleshootingEvent の作成</span><span class="sxs-lookup"><span data-stu-id="b6a8e-103">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="b6a8e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6a8e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6a8e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b6a8e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6a8e-106">新しい [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b6a8e-106">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6a8e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b6a8e-107">Prerequisites</span></span>
<span data-ttu-id="b6a8e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6a8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6a8e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b6a8e-110">Permission type</span></span>|<span data-ttu-id="b6a8e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b6a8e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6a8e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b6a8e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6a8e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6a8e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b6a8e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b6a8e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6a8e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6a8e-115">Not supported.</span></span>|
|<span data-ttu-id="b6a8e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b6a8e-116">Application</span></span>|<span data-ttu-id="b6a8e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6a8e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6a8e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b6a8e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="b6a8e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6a8e-119">Request headers</span></span>
|<span data-ttu-id="b6a8e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6a8e-120">Header</span></span>|<span data-ttu-id="b6a8e-121">値</span><span class="sxs-lookup"><span data-stu-id="b6a8e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6a8e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6a8e-122">Authorization</span></span>|<span data-ttu-id="b6a8e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b6a8e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6a8e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b6a8e-124">Accept</span></span>|<span data-ttu-id="b6a8e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b6a8e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6a8e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b6a8e-126">Request body</span></span>
<span data-ttu-id="b6a8e-127">要求本文で、deviceManagementTroubleshootingEvent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b6a8e-127">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="b6a8e-128">次の表に、deviceManagementTroubleshootingEvent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b6a8e-128">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="b6a8e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6a8e-129">Property</span></span>|<span data-ttu-id="b6a8e-130">型</span><span class="sxs-lookup"><span data-stu-id="b6a8e-130">Type</span></span>|<span data-ttu-id="b6a8e-131">説明</span><span class="sxs-lookup"><span data-stu-id="b6a8e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6a8e-132">id</span><span class="sxs-lookup"><span data-stu-id="b6a8e-132">id</span></span>|<span data-ttu-id="b6a8e-133">文字列</span><span class="sxs-lookup"><span data-stu-id="b6a8e-133">String</span></span>|<span data-ttu-id="b6a8e-134">オブジェクトの UUID</span><span class="sxs-lookup"><span data-stu-id="b6a8e-134">UUID for the object</span></span>|
|<span data-ttu-id="b6a8e-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="b6a8e-135">eventDateTime</span></span>|<span data-ttu-id="b6a8e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6a8e-136">DateTimeOffset</span></span>|<span data-ttu-id="b6a8e-137">イベントが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="b6a8e-137">Time when the event occurred .</span></span>|
|<span data-ttu-id="b6a8e-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="b6a8e-138">correlationId</span></span>|<span data-ttu-id="b6a8e-139">String</span><span class="sxs-lookup"><span data-stu-id="b6a8e-139">String</span></span>|<span data-ttu-id="b6a8e-140">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="b6a8e-140">Id used for tracing the failure in the service.</span></span>|
|<span data-ttu-id="b6a8e-141">トラブルシューティングのエラーの詳細</span><span class="sxs-lookup"><span data-stu-id="b6a8e-141">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="b6a8e-142">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="b6a8e-142">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="b6a8e-143">エラーとその修復に関する詳細情報を含むオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="b6a8e-143">Object containing detailed information about the error and its remediation.</span></span>|
|<span data-ttu-id="b6a8e-144">eventName</span><span class="sxs-lookup"><span data-stu-id="b6a8e-144">eventName</span></span>|<span data-ttu-id="b6a8e-145">String</span><span class="sxs-lookup"><span data-stu-id="b6a8e-145">String</span></span>|<span data-ttu-id="b6a8e-146">トラブルシューティングイベントに対応するイベント名。</span><span class="sxs-lookup"><span data-stu-id="b6a8e-146">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="b6a8e-147">省略可能なフィールドです。</span><span class="sxs-lookup"><span data-stu-id="b6a8e-147">It is an Optional field</span></span>|
|<span data-ttu-id="b6a8e-148">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="b6a8e-148">additionalInformation</span></span>|<span data-ttu-id="b6a8e-149">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b6a8e-149">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b6a8e-150">トラブルシューティングイベントに関する追加情報を提供する文字列キーと文字列値のペアのセット</span><span class="sxs-lookup"><span data-stu-id="b6a8e-150">A set of string key and string value pairs which provides additional information on the Troubleshooting event</span></span>|



## <a name="response"></a><span data-ttu-id="b6a8e-151">応答</span><span class="sxs-lookup"><span data-stu-id="b6a8e-151">Response</span></span>
<span data-ttu-id="b6a8e-152">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b6a8e-152">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6a8e-153">例</span><span class="sxs-lookup"><span data-stu-id="b6a8e-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6a8e-154">要求</span><span class="sxs-lookup"><span data-stu-id="b6a8e-154">Request</span></span>
<span data-ttu-id="b6a8e-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b6a8e-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 852

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
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
```

### <a name="response"></a><span data-ttu-id="b6a8e-156">応答</span><span class="sxs-lookup"><span data-stu-id="b6a8e-156">Response</span></span>
<span data-ttu-id="b6a8e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b6a8e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 901

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
```





