---
title: 更新プログラム (りんご evpptoken) のトラブルシューティングイベント
description: "\"sevpptokenトラブルシューティング\" イベントオブジェクトのプロパティを更新します。"
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0382305cb7b597d3972d7acc671d20878d210ae9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526721"
---
# <a name="update-applevpptokentroubleshootingevent"></a><span data-ttu-id="148a3-103">更新プログラム (りんご evpptoken) のトラブルシューティングイベント</span><span class="sxs-lookup"><span data-stu-id="148a3-103">Update appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="148a3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="148a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="148a3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="148a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="148a3-106">" [sevpptokenトラブルシューティング" イベント](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="148a3-106">Update the properties of a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="148a3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="148a3-107">Prerequisites</span></span>
<span data-ttu-id="148a3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="148a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="148a3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="148a3-110">Permission type</span></span>|<span data-ttu-id="148a3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="148a3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="148a3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="148a3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="148a3-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="148a3-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="148a3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="148a3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="148a3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="148a3-115">Not supported.</span></span>|
|<span data-ttu-id="148a3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="148a3-116">Application</span></span>|<span data-ttu-id="148a3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="148a3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="148a3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="148a3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="148a3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="148a3-119">Request headers</span></span>
|<span data-ttu-id="148a3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="148a3-120">Header</span></span>|<span data-ttu-id="148a3-121">値</span><span class="sxs-lookup"><span data-stu-id="148a3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="148a3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="148a3-122">Authorization</span></span>|<span data-ttu-id="148a3-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="148a3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="148a3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="148a3-124">Accept</span></span>|<span data-ttu-id="148a3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="148a3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="148a3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="148a3-126">Request body</span></span>
<span data-ttu-id="148a3-127">要求本文で、[りんご evpptokenのトラブルシューティングイベント](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="148a3-127">In the request body, supply a JSON representation for the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

<span data-ttu-id="148a3-128">次の表に、[[りんご evpptokenトラブルシューティング] イベント](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="148a3-128">The following table shows the properties that are required when you create the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).</span></span>

|<span data-ttu-id="148a3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="148a3-129">Property</span></span>|<span data-ttu-id="148a3-130">型</span><span class="sxs-lookup"><span data-stu-id="148a3-130">Type</span></span>|<span data-ttu-id="148a3-131">説明</span><span class="sxs-lookup"><span data-stu-id="148a3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="148a3-132">id</span><span class="sxs-lookup"><span data-stu-id="148a3-132">id</span></span>|<span data-ttu-id="148a3-133">String</span><span class="sxs-lookup"><span data-stu-id="148a3-133">String</span></span>|<span data-ttu-id="148a3-134">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="148a3-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="148a3-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="148a3-135">eventDateTime</span></span>|<span data-ttu-id="148a3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="148a3-136">DateTimeOffset</span></span>|<span data-ttu-id="148a3-137">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="148a3-137">Time when the event occurred .</span></span> <span data-ttu-id="148a3-138">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="148a3-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="148a3-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="148a3-139">correlationId</span></span>|<span data-ttu-id="148a3-140">String</span><span class="sxs-lookup"><span data-stu-id="148a3-140">String</span></span>|<span data-ttu-id="148a3-141">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="148a3-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="148a3-142">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="148a3-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="148a3-143">トラブルシューティングのエラーの詳細</span><span class="sxs-lookup"><span data-stu-id="148a3-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="148a3-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="148a3-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="148a3-145">エラーとその修復に関する詳細情報を含むオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="148a3-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="148a3-146">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="148a3-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="148a3-147">eventName</span><span class="sxs-lookup"><span data-stu-id="148a3-147">eventName</span></span>|<span data-ttu-id="148a3-148">String</span><span class="sxs-lookup"><span data-stu-id="148a3-148">String</span></span>|<span data-ttu-id="148a3-149">トラブルシューティングイベントに対応するイベント名。</span><span class="sxs-lookup"><span data-stu-id="148a3-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="148a3-150">[devicemanagementトラブルシューティングイベント](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されるオプションフィールドです</span><span class="sxs-lookup"><span data-stu-id="148a3-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="148a3-151">additionalinformation</span><span class="sxs-lookup"><span data-stu-id="148a3-151">additionalInformation</span></span>|<span data-ttu-id="148a3-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="148a3-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="148a3-153">[devicemanagementトラブルシューティングイベント](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されたトラブルシューティングイベントに関する追加情報を提供する文字列キーと文字列値のペアのセット。</span><span class="sxs-lookup"><span data-stu-id="148a3-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="148a3-154">tokenid</span><span class="sxs-lookup"><span data-stu-id="148a3-154">tokenId</span></span>|<span data-ttu-id="148a3-155">String</span><span class="sxs-lookup"><span data-stu-id="148a3-155">String</span></span>|<span data-ttu-id="148a3-156">Apple volume purchase program のトークン識別子です。</span><span class="sxs-lookup"><span data-stu-id="148a3-156">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="148a3-157">応答</span><span class="sxs-lookup"><span data-stu-id="148a3-157">Response</span></span>
<span data-ttu-id="148a3-158">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[りんご evpptokenトラブルシューティングイベント](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="148a3-158">If successful, this method returns a `200 OK` response code and an updated [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="148a3-159">例</span><span class="sxs-lookup"><span data-stu-id="148a3-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="148a3-160">要求</span><span class="sxs-lookup"><span data-stu-id="148a3-160">Request</span></span>
<span data-ttu-id="148a3-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="148a3-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="148a3-162">応答</span><span class="sxs-lookup"><span data-stu-id="148a3-162">Response</span></span>
<span data-ttu-id="148a3-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="148a3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



