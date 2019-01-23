---
title: AppleVppTokenTroubleshootingEvent を更新します。
description: AppleVppTokenTroubleshootingEvent オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3382eb7069be27fb47bf094d4a0688d7cd128de6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430360"
---
# <a name="update-applevpptokentroubleshootingevent"></a><span data-ttu-id="540d2-103">AppleVppTokenTroubleshootingEvent を更新します。</span><span class="sxs-lookup"><span data-stu-id="540d2-103">Update appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="540d2-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="540d2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="540d2-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="540d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="540d2-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="540d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="540d2-107">[AppleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="540d2-107">Update the properties of a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="540d2-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="540d2-108">Prerequisites</span></span>
<span data-ttu-id="540d2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="540d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="540d2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="540d2-111">Permission type</span></span>|<span data-ttu-id="540d2-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="540d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="540d2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="540d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="540d2-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="540d2-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="540d2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="540d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="540d2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="540d2-116">Not supported.</span></span>|
|<span data-ttu-id="540d2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="540d2-117">Application</span></span>|<span data-ttu-id="540d2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="540d2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="540d2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="540d2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="540d2-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="540d2-120">Request headers</span></span>
|<span data-ttu-id="540d2-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="540d2-121">Header</span></span>|<span data-ttu-id="540d2-122">値</span><span class="sxs-lookup"><span data-stu-id="540d2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="540d2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="540d2-123">Authorization</span></span>|<span data-ttu-id="540d2-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="540d2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="540d2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="540d2-125">Accept</span></span>|<span data-ttu-id="540d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="540d2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="540d2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="540d2-127">Request body</span></span>
<span data-ttu-id="540d2-128">要求の本文に[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="540d2-128">In the request body, supply a JSON representation for the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

<span data-ttu-id="540d2-129">[AppleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="540d2-129">The following table shows the properties that are required when you create the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).</span></span>

|<span data-ttu-id="540d2-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="540d2-130">Property</span></span>|<span data-ttu-id="540d2-131">型</span><span class="sxs-lookup"><span data-stu-id="540d2-131">Type</span></span>|<span data-ttu-id="540d2-132">説明</span><span class="sxs-lookup"><span data-stu-id="540d2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="540d2-133">id</span><span class="sxs-lookup"><span data-stu-id="540d2-133">id</span></span>|<span data-ttu-id="540d2-134">String</span><span class="sxs-lookup"><span data-stu-id="540d2-134">String</span></span>|<span data-ttu-id="540d2-135">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="540d2-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="540d2-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="540d2-136">eventDateTime</span></span>|<span data-ttu-id="540d2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="540d2-137">DateTimeOffset</span></span>|<span data-ttu-id="540d2-138">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="540d2-138">Time when the event occurred .</span></span> <span data-ttu-id="540d2-139">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="540d2-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="540d2-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="540d2-140">correlationId</span></span>|<span data-ttu-id="540d2-141">String</span><span class="sxs-lookup"><span data-stu-id="540d2-141">String</span></span>|<span data-ttu-id="540d2-142">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="540d2-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="540d2-143">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="540d2-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="540d2-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="540d2-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="540d2-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="540d2-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="540d2-146">エラーとその修復に関する詳細情報を含むオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="540d2-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="540d2-147">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="540d2-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="540d2-148">eventName</span><span class="sxs-lookup"><span data-stu-id="540d2-148">eventName</span></span>|<span data-ttu-id="540d2-149">String</span><span class="sxs-lookup"><span data-stu-id="540d2-149">String</span></span>|<span data-ttu-id="540d2-150">トラブルシューティング イベントに対応するイベントの名前です。</span><span class="sxs-lookup"><span data-stu-id="540d2-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="540d2-151">[DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承される省略可能なフィールドします。</span><span class="sxs-lookup"><span data-stu-id="540d2-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="540d2-152">について</span><span class="sxs-lookup"><span data-stu-id="540d2-152">additionalInformation</span></span>|<span data-ttu-id="540d2-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="540d2-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="540d2-154">[DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されるトラブルシューティング イベントに関する追加情報を提供する文字列キーと文字列値のペアのセット</span><span class="sxs-lookup"><span data-stu-id="540d2-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="540d2-155">tokenId</span><span class="sxs-lookup"><span data-stu-id="540d2-155">tokenId</span></span>|<span data-ttu-id="540d2-156">String</span><span class="sxs-lookup"><span data-stu-id="540d2-156">String</span></span>|<span data-ttu-id="540d2-157">Apple ボリューム購入プログラム トークンの識別子です。</span><span class="sxs-lookup"><span data-stu-id="540d2-157">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="540d2-158">応答</span><span class="sxs-lookup"><span data-stu-id="540d2-158">Response</span></span>
<span data-ttu-id="540d2-159">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="540d2-159">If successful, this method returns a `200 OK` response code and an updated [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="540d2-160">例</span><span class="sxs-lookup"><span data-stu-id="540d2-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="540d2-161">要求</span><span class="sxs-lookup"><span data-stu-id="540d2-161">Request</span></span>
<span data-ttu-id="540d2-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="540d2-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
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

### <a name="response"></a><span data-ttu-id="540d2-163">応答</span><span class="sxs-lookup"><span data-stu-id="540d2-163">Response</span></span>
<span data-ttu-id="540d2-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="540d2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




