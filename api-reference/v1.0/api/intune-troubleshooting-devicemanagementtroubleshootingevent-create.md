---
title: deviceManagementTroubleshootingEvent の作成
description: 新しい deviceManagementTroubleshootingEvent オブジェクトを作成します。
ms.openlocfilehash: b6af29c77037c4da49d1593341718a8e798805c2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022387"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="b98cf-103">deviceManagementTroubleshootingEvent の作成</span><span class="sxs-lookup"><span data-stu-id="b98cf-103">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="b98cf-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b98cf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b98cf-105">新しい [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b98cf-105">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b98cf-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b98cf-106">Prerequisites</span></span>
<span data-ttu-id="b98cf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b98cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b98cf-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b98cf-109">Permission type</span></span>|<span data-ttu-id="b98cf-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b98cf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b98cf-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b98cf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b98cf-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b98cf-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b98cf-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b98cf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b98cf-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b98cf-114">Not supported.</span></span>|
|<span data-ttu-id="b98cf-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b98cf-115">Application</span></span>|<span data-ttu-id="b98cf-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b98cf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b98cf-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b98cf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="b98cf-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b98cf-118">Request headers</span></span>
|<span data-ttu-id="b98cf-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b98cf-119">Header</span></span>|<span data-ttu-id="b98cf-120">値</span><span class="sxs-lookup"><span data-stu-id="b98cf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b98cf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b98cf-121">Authorization</span></span>|<span data-ttu-id="b98cf-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b98cf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b98cf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b98cf-123">Accept</span></span>|<span data-ttu-id="b98cf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b98cf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b98cf-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b98cf-125">Request body</span></span>
<span data-ttu-id="b98cf-126">要求本文で、deviceManagementTroubleshootingEvent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b98cf-126">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="b98cf-127">次の表に、deviceManagementTroubleshootingEvent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b98cf-127">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="b98cf-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b98cf-128">Property</span></span>|<span data-ttu-id="b98cf-129">型</span><span class="sxs-lookup"><span data-stu-id="b98cf-129">Type</span></span>|<span data-ttu-id="b98cf-130">説明</span><span class="sxs-lookup"><span data-stu-id="b98cf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b98cf-131">id</span><span class="sxs-lookup"><span data-stu-id="b98cf-131">id</span></span>|<span data-ttu-id="b98cf-132">String</span><span class="sxs-lookup"><span data-stu-id="b98cf-132">String</span></span>|<span data-ttu-id="b98cf-133">オブジェクトの UUID</span><span class="sxs-lookup"><span data-stu-id="b98cf-133">UUID for the object</span></span>|
|<span data-ttu-id="b98cf-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="b98cf-134">eventDateTime</span></span>|<span data-ttu-id="b98cf-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b98cf-135">DateTimeOffset</span></span>|<span data-ttu-id="b98cf-136">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="b98cf-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="b98cf-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="b98cf-137">correlationId</span></span>|<span data-ttu-id="b98cf-138">String</span><span class="sxs-lookup"><span data-stu-id="b98cf-138">String</span></span>|<span data-ttu-id="b98cf-139">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="b98cf-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="b98cf-140">応答</span><span class="sxs-lookup"><span data-stu-id="b98cf-140">Response</span></span>
<span data-ttu-id="b98cf-141">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b98cf-141">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b98cf-142">例</span><span class="sxs-lookup"><span data-stu-id="b98cf-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="b98cf-143">要求</span><span class="sxs-lookup"><span data-stu-id="b98cf-143">Request</span></span>
<span data-ttu-id="b98cf-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b98cf-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="b98cf-145">応答</span><span class="sxs-lookup"><span data-stu-id="b98cf-145">Response</span></span>
<span data-ttu-id="b98cf-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b98cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```



