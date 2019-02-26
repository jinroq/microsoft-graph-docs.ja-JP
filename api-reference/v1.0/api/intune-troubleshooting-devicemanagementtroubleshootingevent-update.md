---
title: deviceManagementTroubleshootingEvent の更新
description: deviceManagementTroubleshootingEvent オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3219a86b2d7788217b26d640443807a4818c66a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251714"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="45a8b-103">deviceManagementTroubleshootingEvent の更新</span><span class="sxs-lookup"><span data-stu-id="45a8b-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="45a8b-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="45a8b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45a8b-105">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="45a8b-105">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45a8b-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="45a8b-106">Prerequisites</span></span>
<span data-ttu-id="45a8b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45a8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="45a8b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="45a8b-109">Permission type</span></span>|<span data-ttu-id="45a8b-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="45a8b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45a8b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="45a8b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="45a8b-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45a8b-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="45a8b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="45a8b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45a8b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45a8b-114">Not supported.</span></span>|
|<span data-ttu-id="45a8b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="45a8b-115">Application</span></span>|<span data-ttu-id="45a8b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45a8b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45a8b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="45a8b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="45a8b-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="45a8b-118">Request headers</span></span>
|<span data-ttu-id="45a8b-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="45a8b-119">Header</span></span>|<span data-ttu-id="45a8b-120">値</span><span class="sxs-lookup"><span data-stu-id="45a8b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45a8b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="45a8b-121">Authorization</span></span>|<span data-ttu-id="45a8b-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="45a8b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45a8b-123">承諾</span><span class="sxs-lookup"><span data-stu-id="45a8b-123">Accept</span></span>|<span data-ttu-id="45a8b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="45a8b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45a8b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="45a8b-125">Request body</span></span>
<span data-ttu-id="45a8b-126">要求本文で、[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="45a8b-126">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="45a8b-127">次の表に、[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="45a8b-127">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="45a8b-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45a8b-128">Property</span></span>|<span data-ttu-id="45a8b-129">型</span><span class="sxs-lookup"><span data-stu-id="45a8b-129">Type</span></span>|<span data-ttu-id="45a8b-130">説明</span><span class="sxs-lookup"><span data-stu-id="45a8b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45a8b-131">id</span><span class="sxs-lookup"><span data-stu-id="45a8b-131">id</span></span>|<span data-ttu-id="45a8b-132">String</span><span class="sxs-lookup"><span data-stu-id="45a8b-132">String</span></span>|<span data-ttu-id="45a8b-133">オブジェクトの UUID</span><span class="sxs-lookup"><span data-stu-id="45a8b-133">UUID for the object</span></span>|
|<span data-ttu-id="45a8b-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="45a8b-134">eventDateTime</span></span>|<span data-ttu-id="45a8b-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45a8b-135">DateTimeOffset</span></span>|<span data-ttu-id="45a8b-136">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="45a8b-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="45a8b-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="45a8b-137">correlationId</span></span>|<span data-ttu-id="45a8b-138">String</span><span class="sxs-lookup"><span data-stu-id="45a8b-138">String</span></span>|<span data-ttu-id="45a8b-139">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="45a8b-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="45a8b-140">応答</span><span class="sxs-lookup"><span data-stu-id="45a8b-140">Response</span></span>
<span data-ttu-id="45a8b-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="45a8b-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45a8b-142">例</span><span class="sxs-lookup"><span data-stu-id="45a8b-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="45a8b-143">要求</span><span class="sxs-lookup"><span data-stu-id="45a8b-143">Request</span></span>
<span data-ttu-id="45a8b-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="45a8b-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="45a8b-145">応答</span><span class="sxs-lookup"><span data-stu-id="45a8b-145">Response</span></span>
<span data-ttu-id="45a8b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="45a8b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



