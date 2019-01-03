---
title: deviceManagementTroubleshootingEvent の更新
description: deviceManagementTroubleshootingEvent オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: ec4cf8d98d51ec369739158c3cf8f6daf2e2ac8e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358808"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="b7b82-103">deviceManagementTroubleshootingEvent の更新</span><span class="sxs-lookup"><span data-stu-id="b7b82-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="b7b82-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b7b82-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7b82-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7b82-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7b82-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7b82-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7b82-107">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b7b82-107">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b7b82-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b7b82-108">Prerequisites</span></span>
<span data-ttu-id="b7b82-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7b82-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7b82-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b7b82-111">Permission type</span></span>|<span data-ttu-id="b7b82-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b7b82-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7b82-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b7b82-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b7b82-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7b82-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b7b82-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b7b82-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7b82-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7b82-116">Not supported.</span></span>|
|<span data-ttu-id="b7b82-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b7b82-117">Application</span></span>|<span data-ttu-id="b7b82-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7b82-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7b82-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b7b82-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="b7b82-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7b82-120">Request headers</span></span>
|<span data-ttu-id="b7b82-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7b82-121">Header</span></span>|<span data-ttu-id="b7b82-122">値</span><span class="sxs-lookup"><span data-stu-id="b7b82-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7b82-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7b82-123">Authorization</span></span>|<span data-ttu-id="b7b82-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b7b82-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7b82-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b7b82-125">Accept</span></span>|<span data-ttu-id="b7b82-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b7b82-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7b82-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b7b82-127">Request body</span></span>
<span data-ttu-id="b7b82-128">要求本文で、[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b7b82-128">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="b7b82-129">次の表に、[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b7b82-129">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="b7b82-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7b82-130">Property</span></span>|<span data-ttu-id="b7b82-131">種類</span><span class="sxs-lookup"><span data-stu-id="b7b82-131">Type</span></span>|<span data-ttu-id="b7b82-132">説明</span><span class="sxs-lookup"><span data-stu-id="b7b82-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7b82-133">ID</span><span class="sxs-lookup"><span data-stu-id="b7b82-133">id</span></span>|<span data-ttu-id="b7b82-134">String</span><span class="sxs-lookup"><span data-stu-id="b7b82-134">String</span></span>|<span data-ttu-id="b7b82-135">オブジェクトの UUID</span><span class="sxs-lookup"><span data-stu-id="b7b82-135">UUID for the object</span></span>|
|<span data-ttu-id="b7b82-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="b7b82-136">eventDateTime</span></span>|<span data-ttu-id="b7b82-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7b82-137">DateTimeOffset</span></span>|<span data-ttu-id="b7b82-138">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="b7b82-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="b7b82-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="b7b82-139">correlationId</span></span>|<span data-ttu-id="b7b82-140">String</span><span class="sxs-lookup"><span data-stu-id="b7b82-140">String</span></span>|<span data-ttu-id="b7b82-141">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="b7b82-141">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="b7b82-142">応答</span><span class="sxs-lookup"><span data-stu-id="b7b82-142">Response</span></span>
<span data-ttu-id="b7b82-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b7b82-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7b82-144">例</span><span class="sxs-lookup"><span data-stu-id="b7b82-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="b7b82-145">要求</span><span class="sxs-lookup"><span data-stu-id="b7b82-145">Request</span></span>
<span data-ttu-id="b7b82-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b7b82-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 104

{
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="b7b82-147">応答</span><span class="sxs-lookup"><span data-stu-id="b7b82-147">Response</span></span>
<span data-ttu-id="b7b82-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b7b82-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```




