---
title: deviceManagementTroubleshootingEvent の作成
description: 新しい deviceManagementTroubleshootingEvent オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c63b34a0e8a29e7ead8491b2bf28402bc25a7d47
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350284"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="4fc81-103">deviceManagementTroubleshootingEvent の作成</span><span class="sxs-lookup"><span data-stu-id="4fc81-103">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="4fc81-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fc81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fc81-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4fc81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fc81-106">新しい [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4fc81-106">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fc81-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4fc81-107">Prerequisites</span></span>
<span data-ttu-id="4fc81-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4fc81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fc81-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4fc81-110">Permission type</span></span>|<span data-ttu-id="4fc81-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4fc81-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fc81-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4fc81-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4fc81-113">\* \* TODO: 範囲を決定します \* \*</span><span class="sxs-lookup"><span data-stu-id="4fc81-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="4fc81-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4fc81-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fc81-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fc81-115">Not supported.</span></span>|
|<span data-ttu-id="4fc81-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4fc81-116">Application</span></span>|<span data-ttu-id="4fc81-117">\* \* TODO: AppOnly スコープを決定します \* \*</span><span class="sxs-lookup"><span data-stu-id="4fc81-117">\*\*TODO: Determine AppOnly scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fc81-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4fc81-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="4fc81-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4fc81-119">Request headers</span></span>
|<span data-ttu-id="4fc81-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4fc81-120">Header</span></span>|<span data-ttu-id="4fc81-121">値</span><span class="sxs-lookup"><span data-stu-id="4fc81-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fc81-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fc81-122">Authorization</span></span>|<span data-ttu-id="4fc81-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4fc81-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fc81-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4fc81-124">Accept</span></span>|<span data-ttu-id="4fc81-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4fc81-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fc81-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4fc81-126">Request body</span></span>
<span data-ttu-id="4fc81-127">要求本文で、deviceManagementTroubleshootingEvent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4fc81-127">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="4fc81-128">次の表に、deviceManagementTroubleshootingEvent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4fc81-128">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="4fc81-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fc81-129">Property</span></span>|<span data-ttu-id="4fc81-130">型</span><span class="sxs-lookup"><span data-stu-id="4fc81-130">Type</span></span>|<span data-ttu-id="4fc81-131">説明</span><span class="sxs-lookup"><span data-stu-id="4fc81-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fc81-132">id</span><span class="sxs-lookup"><span data-stu-id="4fc81-132">id</span></span>|<span data-ttu-id="4fc81-133">文字列</span><span class="sxs-lookup"><span data-stu-id="4fc81-133">String</span></span>|<span data-ttu-id="4fc81-134">オブジェクトの UUID</span><span class="sxs-lookup"><span data-stu-id="4fc81-134">UUID for the object</span></span>|
|<span data-ttu-id="4fc81-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="4fc81-135">eventDateTime</span></span>|<span data-ttu-id="4fc81-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fc81-136">DateTimeOffset</span></span>|<span data-ttu-id="4fc81-137">イベントが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="4fc81-137">Time when the event occurred .</span></span>|
|<span data-ttu-id="4fc81-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="4fc81-138">correlationId</span></span>|<span data-ttu-id="4fc81-139">String</span><span class="sxs-lookup"><span data-stu-id="4fc81-139">String</span></span>|<span data-ttu-id="4fc81-140">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="4fc81-140">Id used for tracing the failure in the service.</span></span>|
|<span data-ttu-id="4fc81-141">トラブルシューティングのエラーの詳細</span><span class="sxs-lookup"><span data-stu-id="4fc81-141">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="4fc81-142">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="4fc81-142">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="4fc81-143">エラーとその修復に関する詳細情報を含むオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="4fc81-143">Object containing detailed information about the error and its remediation.</span></span>|
|<span data-ttu-id="4fc81-144">eventName</span><span class="sxs-lookup"><span data-stu-id="4fc81-144">eventName</span></span>|<span data-ttu-id="4fc81-145">String</span><span class="sxs-lookup"><span data-stu-id="4fc81-145">String</span></span>|<span data-ttu-id="4fc81-146">トラブルシューティングイベントに対応するイベント名。</span><span class="sxs-lookup"><span data-stu-id="4fc81-146">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="4fc81-147">省略可能なフィールドです。</span><span class="sxs-lookup"><span data-stu-id="4fc81-147">It is an Optional field</span></span>|
|<span data-ttu-id="4fc81-148">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="4fc81-148">additionalInformation</span></span>|<span data-ttu-id="4fc81-149">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4fc81-149">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="4fc81-150">トラブルシューティングイベントに関する追加情報を提供する文字列キーと文字列値のペアのセット</span><span class="sxs-lookup"><span data-stu-id="4fc81-150">A set of string key and string value pairs which provides additional information on the Troubleshooting event</span></span>|



## <a name="response"></a><span data-ttu-id="4fc81-151">応答</span><span class="sxs-lookup"><span data-stu-id="4fc81-151">Response</span></span>
<span data-ttu-id="4fc81-152">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4fc81-152">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fc81-153">例</span><span class="sxs-lookup"><span data-stu-id="4fc81-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fc81-154">要求</span><span class="sxs-lookup"><span data-stu-id="4fc81-154">Request</span></span>
<span data-ttu-id="4fc81-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4fc81-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4fc81-156">応答</span><span class="sxs-lookup"><span data-stu-id="4fc81-156">Response</span></span>
<span data-ttu-id="4fc81-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4fc81-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






