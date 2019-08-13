---
title: 「りんご Evpptokenトラブルシューティングイベントを作成する」
description: 新しいりんご Evpptokenのトラブルシューティングイベントオブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 68155622824893cf9d42fc4862c647119fb804eb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347361"
---
# <a name="create-applevpptokentroubleshootingevent"></a><span data-ttu-id="2f83e-103">「りんご Evpptokenトラブルシューティングイベントを作成する」</span><span class="sxs-lookup"><span data-stu-id="2f83e-103">Create appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="2f83e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f83e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f83e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2f83e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f83e-106">新しい[りんご Evpptokenのトラブルシューティングイベント](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2f83e-106">Create a new [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f83e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2f83e-107">Prerequisites</span></span>
<span data-ttu-id="2f83e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2f83e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f83e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2f83e-110">Permission type</span></span>|<span data-ttu-id="2f83e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2f83e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f83e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2f83e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f83e-113">\* \* TODO: 範囲を決定します \* \*</span><span class="sxs-lookup"><span data-stu-id="2f83e-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="2f83e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2f83e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f83e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f83e-115">Not supported.</span></span>|
|<span data-ttu-id="2f83e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2f83e-116">Application</span></span>|<span data-ttu-id="2f83e-117">\* \* TODO: AppOnly スコープを決定します \* \*</span><span class="sxs-lookup"><span data-stu-id="2f83e-117">\*\*TODO: Determine AppOnly scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f83e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2f83e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="2f83e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f83e-119">Request headers</span></span>
|<span data-ttu-id="2f83e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f83e-120">Header</span></span>|<span data-ttu-id="2f83e-121">値</span><span class="sxs-lookup"><span data-stu-id="2f83e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f83e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f83e-122">Authorization</span></span>|<span data-ttu-id="2f83e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2f83e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f83e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2f83e-124">Accept</span></span>|<span data-ttu-id="2f83e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f83e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f83e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2f83e-126">Request body</span></span>
<span data-ttu-id="2f83e-127">要求本文で、りんご Evpptokenのトラブルシューティングイベントオブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2f83e-127">In the request body, supply a JSON representation for the appleVppTokenTroubleshootingEvent object.</span></span>

<span data-ttu-id="2f83e-128">次の表に、[りんご Evpptokenトラブルシューティング] イベントの作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2f83e-128">The following table shows the properties that are required when you create the appleVppTokenTroubleshootingEvent.</span></span>

|<span data-ttu-id="2f83e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f83e-129">Property</span></span>|<span data-ttu-id="2f83e-130">型</span><span class="sxs-lookup"><span data-stu-id="2f83e-130">Type</span></span>|<span data-ttu-id="2f83e-131">説明</span><span class="sxs-lookup"><span data-stu-id="2f83e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f83e-132">id</span><span class="sxs-lookup"><span data-stu-id="2f83e-132">id</span></span>|<span data-ttu-id="2f83e-133">文字列</span><span class="sxs-lookup"><span data-stu-id="2f83e-133">String</span></span>|<span data-ttu-id="2f83e-134">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="2f83e-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="2f83e-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="2f83e-135">eventDateTime</span></span>|<span data-ttu-id="2f83e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f83e-136">DateTimeOffset</span></span>|<span data-ttu-id="2f83e-137">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="2f83e-137">Time when the event occurred .</span></span> <span data-ttu-id="2f83e-138">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2f83e-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="2f83e-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="2f83e-139">correlationId</span></span>|<span data-ttu-id="2f83e-140">String</span><span class="sxs-lookup"><span data-stu-id="2f83e-140">String</span></span>|<span data-ttu-id="2f83e-141">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="2f83e-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="2f83e-142">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2f83e-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="2f83e-143">トラブルシューティングのエラーの詳細</span><span class="sxs-lookup"><span data-stu-id="2f83e-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="2f83e-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="2f83e-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="2f83e-145">エラーとその修復に関する詳細情報を含むオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="2f83e-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="2f83e-146">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2f83e-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="2f83e-147">eventName</span><span class="sxs-lookup"><span data-stu-id="2f83e-147">eventName</span></span>|<span data-ttu-id="2f83e-148">String</span><span class="sxs-lookup"><span data-stu-id="2f83e-148">String</span></span>|<span data-ttu-id="2f83e-149">トラブルシューティングイベントに対応するイベント名。</span><span class="sxs-lookup"><span data-stu-id="2f83e-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="2f83e-150">[Devicemanagementトラブルシューティングイベント](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されるオプションフィールドです</span><span class="sxs-lookup"><span data-stu-id="2f83e-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="2f83e-151">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="2f83e-151">additionalInformation</span></span>|<span data-ttu-id="2f83e-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2f83e-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="2f83e-153">[Devicemanagementトラブルシューティングイベント](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されたトラブルシューティングイベントに関する追加情報を提供する文字列キーと文字列値のペアのセット。</span><span class="sxs-lookup"><span data-stu-id="2f83e-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="2f83e-154">tokenId</span><span class="sxs-lookup"><span data-stu-id="2f83e-154">tokenId</span></span>|<span data-ttu-id="2f83e-155">String</span><span class="sxs-lookup"><span data-stu-id="2f83e-155">String</span></span>|<span data-ttu-id="2f83e-156">Apple Volume purchase Program のトークン識別子です。</span><span class="sxs-lookup"><span data-stu-id="2f83e-156">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="2f83e-157">応答</span><span class="sxs-lookup"><span data-stu-id="2f83e-157">Response</span></span>
<span data-ttu-id="2f83e-158">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で、 [Sevpptokenイベント](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2f83e-158">If successful, this method returns a `201 Created` response code and a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f83e-159">例</span><span class="sxs-lookup"><span data-stu-id="2f83e-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f83e-160">要求</span><span class="sxs-lookup"><span data-stu-id="2f83e-160">Request</span></span>
<span data-ttu-id="2f83e-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2f83e-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 881

{
  "@odata.type": "#microsoft.graph.appleVppTokenTroubleshootingEvent",
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
  ],
  "tokenId": "Token Id value"
}
```

### <a name="response"></a><span data-ttu-id="2f83e-162">応答</span><span class="sxs-lookup"><span data-stu-id="2f83e-162">Response</span></span>
<span data-ttu-id="2f83e-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2f83e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 930

{
  "@odata.type": "#microsoft.graph.appleVppTokenTroubleshootingEvent",
  "id": "09295f26-5f26-0929-265f-2909265f2909",
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
  ],
  "tokenId": "Token Id value"
}
```






