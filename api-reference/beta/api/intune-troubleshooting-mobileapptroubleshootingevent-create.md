---
title: MobileAppTroubleshootingEvent を作成します。
description: 新しい mobileAppTroubleshootingEvent オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 59eea166285f55de32df2728f9bbc834e0eecac8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978145"
---
# <a name="create-mobileapptroubleshootingevent"></a><span data-ttu-id="91f34-103">MobileAppTroubleshootingEvent を作成します。</span><span class="sxs-lookup"><span data-stu-id="91f34-103">Create mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="91f34-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="91f34-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91f34-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91f34-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91f34-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="91f34-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91f34-107">新しい[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="91f34-107">Create a new [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="91f34-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="91f34-108">Prerequisites</span></span>
<span data-ttu-id="91f34-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91f34-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91f34-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="91f34-111">Permission type</span></span>|<span data-ttu-id="91f34-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="91f34-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91f34-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="91f34-113">Delegated (work or school account)</span></span>|<span data-ttu-id="91f34-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91f34-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="91f34-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="91f34-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91f34-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91f34-116">Not supported.</span></span>|
|<span data-ttu-id="91f34-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="91f34-117">Application</span></span>|<span data-ttu-id="91f34-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91f34-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91f34-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="91f34-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="91f34-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91f34-120">Request headers</span></span>
|<span data-ttu-id="91f34-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91f34-121">Header</span></span>|<span data-ttu-id="91f34-122">値</span><span class="sxs-lookup"><span data-stu-id="91f34-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91f34-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="91f34-123">Authorization</span></span>|<span data-ttu-id="91f34-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="91f34-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91f34-125">Accept</span><span class="sxs-lookup"><span data-stu-id="91f34-125">Accept</span></span>|<span data-ttu-id="91f34-126">application/json</span><span class="sxs-lookup"><span data-stu-id="91f34-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91f34-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="91f34-127">Request body</span></span>
<span data-ttu-id="91f34-128">要求の本文に mobileAppTroubleshootingEvent オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="91f34-128">In the request body, supply a JSON representation for the mobileAppTroubleshootingEvent object.</span></span>

<span data-ttu-id="91f34-129">次の表は、mobileAppTroubleshootingEvent を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="91f34-129">The following table shows the properties that are required when you create the mobileAppTroubleshootingEvent.</span></span>

|<span data-ttu-id="91f34-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91f34-130">Property</span></span>|<span data-ttu-id="91f34-131">型</span><span class="sxs-lookup"><span data-stu-id="91f34-131">Type</span></span>|<span data-ttu-id="91f34-132">説明</span><span class="sxs-lookup"><span data-stu-id="91f34-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91f34-133">ID</span><span class="sxs-lookup"><span data-stu-id="91f34-133">id</span></span>|<span data-ttu-id="91f34-134">String</span><span class="sxs-lookup"><span data-stu-id="91f34-134">String</span></span>|<span data-ttu-id="91f34-135">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="91f34-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="91f34-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="91f34-136">eventDateTime</span></span>|<span data-ttu-id="91f34-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91f34-137">DateTimeOffset</span></span>|<span data-ttu-id="91f34-138">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="91f34-138">Time when the event occurred .</span></span> <span data-ttu-id="91f34-139">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="91f34-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="91f34-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="91f34-140">correlationId</span></span>|<span data-ttu-id="91f34-141">String</span><span class="sxs-lookup"><span data-stu-id="91f34-141">String</span></span>|<span data-ttu-id="91f34-142">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="91f34-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="91f34-143">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="91f34-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="91f34-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="91f34-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="91f34-145">String</span><span class="sxs-lookup"><span data-stu-id="91f34-145">String</span></span>|<span data-ttu-id="91f34-146">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="91f34-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="91f34-147">userId</span><span class="sxs-lookup"><span data-stu-id="91f34-147">userId</span></span>|<span data-ttu-id="91f34-148">String</span><span class="sxs-lookup"><span data-stu-id="91f34-148">String</span></span>|<span data-ttu-id="91f34-149">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="91f34-149">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="91f34-150">applicationId</span><span class="sxs-lookup"><span data-stu-id="91f34-150">applicationId</span></span>|<span data-ttu-id="91f34-151">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="91f34-151">String</span></span>|<span data-ttu-id="91f34-152">Intune アプリケーション識別子です。</span><span class="sxs-lookup"><span data-stu-id="91f34-152">Intune application identifier.</span></span>|
|<span data-ttu-id="91f34-153">履歴</span><span class="sxs-lookup"><span data-stu-id="91f34-153">history</span></span>|<span data-ttu-id="91f34-154">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="91f34-154">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="91f34-155">Intune モバイル アプリケーションの履歴項目のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="91f34-155">Intune Mobile Application Troubleshooting History Item</span></span>|



## <a name="response"></a><span data-ttu-id="91f34-156">応答</span><span class="sxs-lookup"><span data-stu-id="91f34-156">Response</span></span>
<span data-ttu-id="91f34-157">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="91f34-157">If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91f34-158">例</span><span class="sxs-lookup"><span data-stu-id="91f34-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="91f34-159">要求</span><span class="sxs-lookup"><span data-stu-id="91f34-159">Request</span></span>
<span data-ttu-id="91f34-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="91f34-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 489

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "applicationId": "Application Id value",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "2017-01-01T00:03:20.8380798-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="91f34-161">応答</span><span class="sxs-lookup"><span data-stu-id="91f34-161">Response</span></span>
<span data-ttu-id="91f34-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="91f34-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 538

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "applicationId": "Application Id value",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "2017-01-01T00:03:20.8380798-08:00"
    }
  ]
}
```





