---
title: deviceManagementTroubleshootingEvent の更新
description: deviceManagementTroubleshootingEvent オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2374a8a749acf0bb8f1082a2b7f8083736a14e46
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31798139"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="47994-103">deviceManagementTroubleshootingEvent の更新</span><span class="sxs-lookup"><span data-stu-id="47994-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="47994-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47994-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47994-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="47994-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47994-106">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="47994-106">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47994-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="47994-107">Prerequisites</span></span>
<span data-ttu-id="47994-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="47994-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47994-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="47994-110">Permission type</span></span>|<span data-ttu-id="47994-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="47994-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47994-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="47994-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47994-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47994-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="47994-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="47994-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47994-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47994-115">Not supported.</span></span>|
|<span data-ttu-id="47994-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="47994-116">Application</span></span>|<span data-ttu-id="47994-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47994-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47994-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="47994-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="47994-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="47994-119">Request headers</span></span>
|<span data-ttu-id="47994-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="47994-120">Header</span></span>|<span data-ttu-id="47994-121">値</span><span class="sxs-lookup"><span data-stu-id="47994-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47994-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="47994-122">Authorization</span></span>|<span data-ttu-id="47994-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="47994-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47994-124">承諾</span><span class="sxs-lookup"><span data-stu-id="47994-124">Accept</span></span>|<span data-ttu-id="47994-125">application/json</span><span class="sxs-lookup"><span data-stu-id="47994-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47994-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="47994-126">Request body</span></span>
<span data-ttu-id="47994-127">要求本文で、[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="47994-127">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="47994-128">次の表に、[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="47994-128">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="47994-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47994-129">Property</span></span>|<span data-ttu-id="47994-130">型</span><span class="sxs-lookup"><span data-stu-id="47994-130">Type</span></span>|<span data-ttu-id="47994-131">説明</span><span class="sxs-lookup"><span data-stu-id="47994-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47994-132">id</span><span class="sxs-lookup"><span data-stu-id="47994-132">id</span></span>|<span data-ttu-id="47994-133">String</span><span class="sxs-lookup"><span data-stu-id="47994-133">String</span></span>|<span data-ttu-id="47994-134">オブジェクトの UUID</span><span class="sxs-lookup"><span data-stu-id="47994-134">UUID for the object</span></span>|
|<span data-ttu-id="47994-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="47994-135">eventDateTime</span></span>|<span data-ttu-id="47994-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47994-136">DateTimeOffset</span></span>|<span data-ttu-id="47994-137">イベントが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="47994-137">Time when the event occurred .</span></span>|
|<span data-ttu-id="47994-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="47994-138">correlationId</span></span>|<span data-ttu-id="47994-139">String</span><span class="sxs-lookup"><span data-stu-id="47994-139">String</span></span>|<span data-ttu-id="47994-140">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="47994-140">Id used for tracing the failure in the service.</span></span>|
|<span data-ttu-id="47994-141">トラブルシューティングのエラーの詳細</span><span class="sxs-lookup"><span data-stu-id="47994-141">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="47994-142">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="47994-142">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="47994-143">エラーとその修復に関する詳細情報を含むオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="47994-143">Object containing detailed information about the error and its remediation.</span></span>|
|<span data-ttu-id="47994-144">eventName</span><span class="sxs-lookup"><span data-stu-id="47994-144">eventName</span></span>|<span data-ttu-id="47994-145">文字列</span><span class="sxs-lookup"><span data-stu-id="47994-145">String</span></span>|<span data-ttu-id="47994-146">トラブルシューティングイベントに対応するイベント名。</span><span class="sxs-lookup"><span data-stu-id="47994-146">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="47994-147">省略可能なフィールドです。</span><span class="sxs-lookup"><span data-stu-id="47994-147">It is an Optional field</span></span>|
|<span data-ttu-id="47994-148">additionalinformation</span><span class="sxs-lookup"><span data-stu-id="47994-148">additionalInformation</span></span>|<span data-ttu-id="47994-149">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="47994-149">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="47994-150">トラブルシューティングイベントに関する追加情報を提供する文字列キーと文字列値のペアのセット</span><span class="sxs-lookup"><span data-stu-id="47994-150">A set of string key and string value pairs which provides additional information on the Troubleshooting event</span></span>|



## <a name="response"></a><span data-ttu-id="47994-151">応答</span><span class="sxs-lookup"><span data-stu-id="47994-151">Response</span></span>
<span data-ttu-id="47994-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="47994-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47994-153">例</span><span class="sxs-lookup"><span data-stu-id="47994-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="47994-154">要求</span><span class="sxs-lookup"><span data-stu-id="47994-154">Request</span></span>
<span data-ttu-id="47994-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="47994-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
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

### <a name="response"></a><span data-ttu-id="47994-156">応答</span><span class="sxs-lookup"><span data-stu-id="47994-156">Response</span></span>
<span data-ttu-id="47994-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="47994-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



