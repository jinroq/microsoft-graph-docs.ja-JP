---
title: mobileAppTroubleshootingEvent リソースの種類
description: Intune は、複数のワークフローをサポートする Microsoft グラフ API の mobileAppTroubleshootingEvent リソースについて説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bb519309f68f732a28ed8f26235f01f37d9628b9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430515"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a><span data-ttu-id="bc347-103">mobileAppTroubleshootingEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bc347-103">mobileAppTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="bc347-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bc347-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bc347-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc347-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc347-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bc347-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc347-107">ユーザー デバイスのアプリケーションを表すイベントは、デバイスの管理とトラブルシューティング イベント ワークフローの状態をインストールします。</span><span class="sxs-lookup"><span data-stu-id="bc347-107">Event representing a users device application install status for device management and troubleshooting event workflows.</span></span>

## <a name="methods"></a><span data-ttu-id="bc347-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="bc347-108">Methods</span></span>
|<span data-ttu-id="bc347-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="bc347-109">Method</span></span>|<span data-ttu-id="bc347-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bc347-110">Return Type</span></span>|<span data-ttu-id="bc347-111">説明</span><span class="sxs-lookup"><span data-stu-id="bc347-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bc347-112">リスト mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="bc347-112">List mobileAppTroubleshootingEvents</span></span>](../api/intune-shared-mobileapptroubleshootingevent-list.md)|<span data-ttu-id="bc347-113">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bc347-113">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) collection</span></span>|<span data-ttu-id="bc347-114">[MobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="bc347-114">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="bc347-115">MobileAppTroubleshootingEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="bc347-115">Get mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-get.md)|[<span data-ttu-id="bc347-116">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="bc347-116">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="bc347-117">[MobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bc347-117">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="bc347-118">MobileAppTroubleshootingEvent を作成します。</span><span class="sxs-lookup"><span data-stu-id="bc347-118">Create mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-create.md)|[<span data-ttu-id="bc347-119">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="bc347-119">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="bc347-120">新しい[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bc347-120">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="bc347-121">MobileAppTroubleshootingEvent を削除します。</span><span class="sxs-lookup"><span data-stu-id="bc347-121">Delete mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-delete.md)|<span data-ttu-id="bc347-122">なし</span><span class="sxs-lookup"><span data-stu-id="bc347-122">None</span></span>|<span data-ttu-id="bc347-123">の[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="bc347-123">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="bc347-124">MobileAppTroubleshootingEvent を更新します。</span><span class="sxs-lookup"><span data-stu-id="bc347-124">Update mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-update.md)|[<span data-ttu-id="bc347-125">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="bc347-125">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="bc347-126">[MobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bc347-126">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc347-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc347-127">Properties</span></span>
|<span data-ttu-id="bc347-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc347-128">Property</span></span>|<span data-ttu-id="bc347-129">型</span><span class="sxs-lookup"><span data-stu-id="bc347-129">Type</span></span>|<span data-ttu-id="bc347-130">説明</span><span class="sxs-lookup"><span data-stu-id="bc347-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc347-131">id</span><span class="sxs-lookup"><span data-stu-id="bc347-131">id</span></span>|<span data-ttu-id="bc347-132">String</span><span class="sxs-lookup"><span data-stu-id="bc347-132">String</span></span>|<span data-ttu-id="bc347-133">オブジェクトの UUID です。</span><span class="sxs-lookup"><span data-stu-id="bc347-133">UUID for the object.</span></span>|
|<span data-ttu-id="bc347-134">**トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="bc347-134">**Troubleshooting**</span></span>|
|<span data-ttu-id="bc347-135">について</span><span class="sxs-lookup"><span data-stu-id="bc347-135">additionalInformation</span></span>|<span data-ttu-id="bc347-136">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bc347-136">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="bc347-137">[DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されるトラブルシューティング イベントに関する追加情報を提供する文字列キーと文字列値のペアのセット</span><span class="sxs-lookup"><span data-stu-id="bc347-137">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="bc347-138">applicationId</span><span class="sxs-lookup"><span data-stu-id="bc347-138">applicationId</span></span>|<span data-ttu-id="bc347-139">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="bc347-139">String</span></span>|<span data-ttu-id="bc347-140">Intune アプリケーション識別子です。</span><span class="sxs-lookup"><span data-stu-id="bc347-140">Intune application identifier.</span></span>|
|<span data-ttu-id="bc347-141">correlationId</span><span class="sxs-lookup"><span data-stu-id="bc347-141">correlationId</span></span>|<span data-ttu-id="bc347-142">String</span><span class="sxs-lookup"><span data-stu-id="bc347-142">String</span></span>|<span data-ttu-id="bc347-143">サービスでエラーのトレースに使用される ID です。</span><span class="sxs-lookup"><span data-stu-id="bc347-143">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="bc347-144">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="bc347-144">eventDateTime</span></span>|<span data-ttu-id="bc347-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc347-145">DateTimeOffset</span></span>|<span data-ttu-id="bc347-146">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="bc347-146">Time when the event occurred .</span></span> |
|<span data-ttu-id="bc347-147">eventName</span><span class="sxs-lookup"><span data-stu-id="bc347-147">eventName</span></span>|<span data-ttu-id="bc347-148">String</span><span class="sxs-lookup"><span data-stu-id="bc347-148">String</span></span>|<span data-ttu-id="bc347-149">トラブルシューティング イベントに対応するイベントの名前です。</span><span class="sxs-lookup"><span data-stu-id="bc347-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="bc347-150">省略可能</span><span class="sxs-lookup"><span data-stu-id="bc347-150">Optional</span></span>|
|<span data-ttu-id="bc347-151">履歴</span><span class="sxs-lookup"><span data-stu-id="bc347-151">history</span></span>|<span data-ttu-id="bc347-152">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bc347-152">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="bc347-153">Intune モバイル アプリケーションの履歴項目のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="bc347-153">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="bc347-154">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="bc347-154">managedDeviceIdentifier</span></span>|<span data-ttu-id="bc347-155">String</span><span class="sxs-lookup"><span data-stu-id="bc347-155">String</span></span>|<span data-ttu-id="bc347-156">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="bc347-156">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="bc347-157">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="bc347-157">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="bc347-158">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="bc347-158">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="bc347-159">エラーとその修復に関する詳細情報を含むオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="bc347-159">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="bc347-160">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bc347-160">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="bc347-161">userId</span><span class="sxs-lookup"><span data-stu-id="bc347-161">userId</span></span>|<span data-ttu-id="bc347-162">String</span><span class="sxs-lookup"><span data-stu-id="bc347-162">String</span></span>|<span data-ttu-id="bc347-163">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="bc347-163">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc347-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bc347-164">Relationships</span></span>
|<span data-ttu-id="bc347-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bc347-165">Relationship</span></span>|<span data-ttu-id="bc347-166">型</span><span class="sxs-lookup"><span data-stu-id="bc347-166">Type</span></span>|<span data-ttu-id="bc347-167">説明</span><span class="sxs-lookup"><span data-stu-id="bc347-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc347-168">**デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="bc347-168">**Device management**</span></span>|
|<span data-ttu-id="bc347-169">appLogCollectionRequests</span><span class="sxs-lookup"><span data-stu-id="bc347-169">appLogCollectionRequests</span></span>|<span data-ttu-id="bc347-170">[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bc347-170">[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) collection</span></span>|<span data-ttu-id="bc347-171">AppLogUploadRequest のコレクションのプロパティです。</span><span class="sxs-lookup"><span data-stu-id="bc347-171">The collection property of AppLogUploadRequest.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="bc347-172">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bc347-172">JSON Representation</span></span>
<span data-ttu-id="bc347-173">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bc347-173">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "String",
    "failure": "String",
    "failureDetails": "String",
    "remediation": "String",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "String",
        "link": "String"
      }
    ]
  },
  "eventName": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "applicationId": "String",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "String (timestamp)"
    }
  ]
}
```




