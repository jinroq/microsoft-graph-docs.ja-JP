---
title: MobileAppTroubleshootingEvent を作成します。
description: Intune は、複数のワークフローをサポートするための Microsoft グラフ API を作成する mobileAppTroubleshootingEvent メソッドを説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e409aa663ff2471222a7e36a9e381505792f37eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431636"
---
# <a name="create-mobileapptroubleshootingevent"></a><span data-ttu-id="36971-103">MobileAppTroubleshootingEvent を作成します。</span><span class="sxs-lookup"><span data-stu-id="36971-103">Create mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="36971-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="36971-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="36971-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36971-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36971-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="36971-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36971-107">新しい[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="36971-107">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36971-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="36971-108">Prerequisites</span></span>
<span data-ttu-id="36971-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36971-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="36971-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="36971-111">Permission type</span></span>|<span data-ttu-id="36971-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="36971-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36971-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="36971-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="36971-114">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="36971-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="36971-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36971-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="36971-116">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="36971-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="36971-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36971-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="36971-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="36971-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36971-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36971-119">Not supported.</span></span>|
|<span data-ttu-id="36971-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="36971-120">Application</span></span>|<span data-ttu-id="36971-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36971-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36971-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="36971-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="36971-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36971-123">Request headers</span></span>
|<span data-ttu-id="36971-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36971-124">Header</span></span>|<span data-ttu-id="36971-125">値</span><span class="sxs-lookup"><span data-stu-id="36971-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36971-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="36971-126">Authorization</span></span>|<span data-ttu-id="36971-127">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="36971-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36971-128">Accept</span><span class="sxs-lookup"><span data-stu-id="36971-128">Accept</span></span>|<span data-ttu-id="36971-129">application/json</span><span class="sxs-lookup"><span data-stu-id="36971-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36971-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="36971-130">Request body</span></span>
<span data-ttu-id="36971-131">要求の本文に mobileAppTroubleshootingEvent オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="36971-131">In the request body, supply a JSON representation for the mobileAppTroubleshootingEvent object.</span></span>

<span data-ttu-id="36971-132">次の表は、mobileAppTroubleshootingEvent を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="36971-132">The following table shows the properties that are required when you create the mobileAppTroubleshootingEvent.</span></span>

|<span data-ttu-id="36971-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36971-133">Property</span></span>|<span data-ttu-id="36971-134">型</span><span class="sxs-lookup"><span data-stu-id="36971-134">Type</span></span>|<span data-ttu-id="36971-135">説明</span><span class="sxs-lookup"><span data-stu-id="36971-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36971-136">id</span><span class="sxs-lookup"><span data-stu-id="36971-136">id</span></span>|<span data-ttu-id="36971-137">String</span><span class="sxs-lookup"><span data-stu-id="36971-137">String</span></span>|<span data-ttu-id="36971-138">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="36971-138">The GUID for the object</span></span>|
|<span data-ttu-id="36971-139">**トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="36971-139">**Troubleshooting**</span></span>|
|<span data-ttu-id="36971-140">について</span><span class="sxs-lookup"><span data-stu-id="36971-140">additionalInformation</span></span>|<span data-ttu-id="36971-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="36971-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="36971-142">トラブルシューティング イベントに関する追加情報を提供する文字列キーと文字列値のペアのセットです。</span><span class="sxs-lookup"><span data-stu-id="36971-142">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="36971-143">applicationId</span><span class="sxs-lookup"><span data-stu-id="36971-143">applicationId</span></span>|<span data-ttu-id="36971-144">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="36971-144">String</span></span>|<span data-ttu-id="36971-145">Intune アプリケーション識別子です。</span><span class="sxs-lookup"><span data-stu-id="36971-145">Intune application identifier.</span></span>|
|<span data-ttu-id="36971-146">correlationId</span><span class="sxs-lookup"><span data-stu-id="36971-146">correlationId</span></span>|<span data-ttu-id="36971-147">String</span><span class="sxs-lookup"><span data-stu-id="36971-147">String</span></span>|<span data-ttu-id="36971-148">サービスでエラーのトレースに使用される ID です。</span><span class="sxs-lookup"><span data-stu-id="36971-148">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="36971-149">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="36971-149">eventDateTime</span></span>|<span data-ttu-id="36971-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36971-150">DateTimeOffset</span></span>|<span data-ttu-id="36971-151">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="36971-151">Time when the event occurred .</span></span> |
|<span data-ttu-id="36971-152">eventName</span><span class="sxs-lookup"><span data-stu-id="36971-152">eventName</span></span>|<span data-ttu-id="36971-153">String</span><span class="sxs-lookup"><span data-stu-id="36971-153">String</span></span>|<span data-ttu-id="36971-154">トラブルシューティング イベントに対応するイベントの名前です。</span><span class="sxs-lookup"><span data-stu-id="36971-154">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="36971-155">省略可能。</span><span class="sxs-lookup"><span data-stu-id="36971-155">Optional.</span></span>|
|<span data-ttu-id="36971-156">履歴</span><span class="sxs-lookup"><span data-stu-id="36971-156">history</span></span>|<span data-ttu-id="36971-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="36971-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="36971-158">Intune モバイル アプリケーションの履歴項目のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="36971-158">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="36971-159">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="36971-159">managedDeviceIdentifier</span></span>|<span data-ttu-id="36971-160">String</span><span class="sxs-lookup"><span data-stu-id="36971-160">String</span></span>|<span data-ttu-id="36971-161">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="36971-161">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="36971-162">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="36971-162">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="36971-163">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="36971-163">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="36971-164">エラーとその修復に関する詳細情報を含むオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="36971-164">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="36971-165">userId</span><span class="sxs-lookup"><span data-stu-id="36971-165">userId</span></span>|<span data-ttu-id="36971-166">String</span><span class="sxs-lookup"><span data-stu-id="36971-166">String</span></span>|<span data-ttu-id="36971-167">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="36971-167">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="36971-168">応答</span><span class="sxs-lookup"><span data-stu-id="36971-168">Response</span></span>
<span data-ttu-id="36971-169">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="36971-169">If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36971-170">例</span><span class="sxs-lookup"><span data-stu-id="36971-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="36971-171">要求</span><span class="sxs-lookup"><span data-stu-id="36971-171">Request</span></span>
<span data-ttu-id="36971-172">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="36971-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="36971-173">応答</span><span class="sxs-lookup"><span data-stu-id="36971-173">Response</span></span>
<span data-ttu-id="36971-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="36971-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```




