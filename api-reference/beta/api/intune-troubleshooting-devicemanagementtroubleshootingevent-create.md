---
title: deviceManagementTroubleshootingEvent の作成
description: 新しい deviceManagementTroubleshootingEvent オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f8b88d0474c7b332b91d447c963fa2a983b64035
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404429"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="95529-103">deviceManagementTroubleshootingEvent の作成</span><span class="sxs-lookup"><span data-stu-id="95529-103">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="95529-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="95529-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="95529-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95529-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95529-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="95529-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95529-107">新しい [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="95529-107">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95529-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="95529-108">Prerequisites</span></span>
<span data-ttu-id="95529-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95529-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="95529-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95529-111">Permission type</span></span>|<span data-ttu-id="95529-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="95529-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95529-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95529-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95529-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95529-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="95529-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95529-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95529-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95529-116">Not supported.</span></span>|
|<span data-ttu-id="95529-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95529-117">Application</span></span>|<span data-ttu-id="95529-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95529-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95529-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95529-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="95529-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95529-120">Request headers</span></span>
|<span data-ttu-id="95529-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95529-121">Header</span></span>|<span data-ttu-id="95529-122">値</span><span class="sxs-lookup"><span data-stu-id="95529-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95529-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="95529-123">Authorization</span></span>|<span data-ttu-id="95529-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="95529-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95529-125">Accept</span><span class="sxs-lookup"><span data-stu-id="95529-125">Accept</span></span>|<span data-ttu-id="95529-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95529-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95529-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="95529-127">Request body</span></span>
<span data-ttu-id="95529-128">要求本文で、deviceManagementTroubleshootingEvent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="95529-128">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="95529-129">次の表に、deviceManagementTroubleshootingEvent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="95529-129">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="95529-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95529-130">Property</span></span>|<span data-ttu-id="95529-131">型</span><span class="sxs-lookup"><span data-stu-id="95529-131">Type</span></span>|<span data-ttu-id="95529-132">説明</span><span class="sxs-lookup"><span data-stu-id="95529-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95529-133">id</span><span class="sxs-lookup"><span data-stu-id="95529-133">id</span></span>|<span data-ttu-id="95529-134">String</span><span class="sxs-lookup"><span data-stu-id="95529-134">String</span></span>|<span data-ttu-id="95529-135">オブジェクトの UUID</span><span class="sxs-lookup"><span data-stu-id="95529-135">UUID for the object</span></span>|
|<span data-ttu-id="95529-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="95529-136">eventDateTime</span></span>|<span data-ttu-id="95529-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95529-137">DateTimeOffset</span></span>|<span data-ttu-id="95529-138">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="95529-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="95529-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="95529-139">correlationId</span></span>|<span data-ttu-id="95529-140">String</span><span class="sxs-lookup"><span data-stu-id="95529-140">String</span></span>|<span data-ttu-id="95529-141">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="95529-141">Id used for tracing the failure in the service.</span></span>|
|<span data-ttu-id="95529-142">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="95529-142">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="95529-143">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="95529-143">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="95529-144">エラーとその修復に関する詳細情報を含むオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="95529-144">Object containing detailed information about the error and its remediation.</span></span>|
|<span data-ttu-id="95529-145">eventName</span><span class="sxs-lookup"><span data-stu-id="95529-145">eventName</span></span>|<span data-ttu-id="95529-146">String</span><span class="sxs-lookup"><span data-stu-id="95529-146">String</span></span>|<span data-ttu-id="95529-147">トラブルシューティング イベントに対応するイベントの名前です。</span><span class="sxs-lookup"><span data-stu-id="95529-147">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="95529-148">省略可能なフィールドします。</span><span class="sxs-lookup"><span data-stu-id="95529-148">It is an Optional field</span></span>|
|<span data-ttu-id="95529-149">について</span><span class="sxs-lookup"><span data-stu-id="95529-149">additionalInformation</span></span>|<span data-ttu-id="95529-150">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="95529-150">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="95529-151">トラブルシューティング イベントに関する追加情報を提供する文字列キーと文字列値のペアのセット</span><span class="sxs-lookup"><span data-stu-id="95529-151">A set of string key and string value pairs which provides additional information on the Troubleshooting event</span></span>|



## <a name="response"></a><span data-ttu-id="95529-152">応答</span><span class="sxs-lookup"><span data-stu-id="95529-152">Response</span></span>
<span data-ttu-id="95529-153">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="95529-153">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95529-154">例</span><span class="sxs-lookup"><span data-stu-id="95529-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="95529-155">要求</span><span class="sxs-lookup"><span data-stu-id="95529-155">Request</span></span>
<span data-ttu-id="95529-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="95529-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="95529-157">応答</span><span class="sxs-lookup"><span data-stu-id="95529-157">Response</span></span>
<span data-ttu-id="95529-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="95529-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




