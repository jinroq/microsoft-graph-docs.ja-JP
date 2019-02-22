---
title: mobileAppTroubleshootingEvent リソースの種類
description: 複数のワークフローをサポートする Microsoft Graph API for Intune の mobileAppTroubleshootingEvent リソースについて説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cfa126fea86c7edb302953efc3b88376f2d68a09
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162945"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a><span data-ttu-id="a15bc-103">mobileAppTroubleshootingEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a15bc-103">mobileAppTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="a15bc-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a15bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a15bc-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a15bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a15bc-106">デバイスの管理とトラブルシューティングのイベントワークフローについて、ユーザーのデバイスアプリケーションのインストール状態を表すイベント。</span><span class="sxs-lookup"><span data-stu-id="a15bc-106">Event representing a users device application install status for device management and troubleshooting event workflows.</span></span>

## <a name="methods"></a><span data-ttu-id="a15bc-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a15bc-107">Methods</span></span>
|<span data-ttu-id="a15bc-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a15bc-108">Method</span></span>|<span data-ttu-id="a15bc-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a15bc-109">Return Type</span></span>|<span data-ttu-id="a15bc-110">説明</span><span class="sxs-lookup"><span data-stu-id="a15bc-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a15bc-111">リスト mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="a15bc-111">List mobileAppTroubleshootingEvents</span></span>](../api/intune-shared-mobileapptroubleshootingevent-list.md)|<span data-ttu-id="a15bc-112">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a15bc-112">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) collection</span></span>|<span data-ttu-id="a15bc-113">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a15bc-113">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="a15bc-114">mobileAppTroubleshootingEvent を取得する</span><span class="sxs-lookup"><span data-stu-id="a15bc-114">Get mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-get.md)|[<span data-ttu-id="a15bc-115">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="a15bc-115">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="a15bc-116">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a15bc-116">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="a15bc-117">mobileAppTroubleshootingEvent を作成する</span><span class="sxs-lookup"><span data-stu-id="a15bc-117">Create mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-create.md)|[<span data-ttu-id="a15bc-118">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="a15bc-118">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="a15bc-119">新しい[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a15bc-119">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="a15bc-120">mobileAppTroubleshootingEvent の削除</span><span class="sxs-lookup"><span data-stu-id="a15bc-120">Delete mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-delete.md)|<span data-ttu-id="a15bc-121">なし</span><span class="sxs-lookup"><span data-stu-id="a15bc-121">None</span></span>|<span data-ttu-id="a15bc-122">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="a15bc-122">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="a15bc-123">mobileAppTroubleshootingEvent の更新</span><span class="sxs-lookup"><span data-stu-id="a15bc-123">Update mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-update.md)|[<span data-ttu-id="a15bc-124">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="a15bc-124">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="a15bc-125">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a15bc-125">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a15bc-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a15bc-126">Properties</span></span>
|<span data-ttu-id="a15bc-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a15bc-127">Property</span></span>|<span data-ttu-id="a15bc-128">型</span><span class="sxs-lookup"><span data-stu-id="a15bc-128">Type</span></span>|<span data-ttu-id="a15bc-129">説明</span><span class="sxs-lookup"><span data-stu-id="a15bc-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a15bc-130">id</span><span class="sxs-lookup"><span data-stu-id="a15bc-130">id</span></span>|<span data-ttu-id="a15bc-131">文字列</span><span class="sxs-lookup"><span data-stu-id="a15bc-131">String</span></span>|<span data-ttu-id="a15bc-132">オブジェクトの UUID。</span><span class="sxs-lookup"><span data-stu-id="a15bc-132">UUID for the object.</span></span>|
|<span data-ttu-id="a15bc-133">**トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="a15bc-133">**Troubleshooting**</span></span>|
|<span data-ttu-id="a15bc-134">additionalinformation</span><span class="sxs-lookup"><span data-stu-id="a15bc-134">additionalInformation</span></span>|<span data-ttu-id="a15bc-135">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a15bc-135">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a15bc-136">[devicemanagementトラブルシューティングイベント](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されたトラブルシューティングイベントに関する追加情報を提供する文字列キーと文字列値のペアのセット。</span><span class="sxs-lookup"><span data-stu-id="a15bc-136">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a15bc-137">applicationId</span><span class="sxs-lookup"><span data-stu-id="a15bc-137">applicationId</span></span>|<span data-ttu-id="a15bc-138">String</span><span class="sxs-lookup"><span data-stu-id="a15bc-138">String</span></span>|<span data-ttu-id="a15bc-139">Intune アプリケーション識別子。</span><span class="sxs-lookup"><span data-stu-id="a15bc-139">Intune application identifier.</span></span>|
|<span data-ttu-id="a15bc-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="a15bc-140">correlationId</span></span>|<span data-ttu-id="a15bc-141">String</span><span class="sxs-lookup"><span data-stu-id="a15bc-141">String</span></span>|<span data-ttu-id="a15bc-142">サービスのエラーをトレースするために使用される ID。</span><span class="sxs-lookup"><span data-stu-id="a15bc-142">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="a15bc-143">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="a15bc-143">eventDateTime</span></span>|<span data-ttu-id="a15bc-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a15bc-144">DateTimeOffset</span></span>|<span data-ttu-id="a15bc-145">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="a15bc-145">Time when the event occurred .</span></span> |
|<span data-ttu-id="a15bc-146">eventName</span><span class="sxs-lookup"><span data-stu-id="a15bc-146">eventName</span></span>|<span data-ttu-id="a15bc-147">String</span><span class="sxs-lookup"><span data-stu-id="a15bc-147">String</span></span>|<span data-ttu-id="a15bc-148">トラブルシューティングイベントに対応するイベント名。</span><span class="sxs-lookup"><span data-stu-id="a15bc-148">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="a15bc-149">省略可能</span><span class="sxs-lookup"><span data-stu-id="a15bc-149">Optional</span></span>|
|<span data-ttu-id="a15bc-150">履歴</span><span class="sxs-lookup"><span data-stu-id="a15bc-150">history</span></span>|<span data-ttu-id="a15bc-151">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a15bc-151">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="a15bc-152">Intune モバイルアプリケーションのトラブルシューティングの履歴項目</span><span class="sxs-lookup"><span data-stu-id="a15bc-152">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="a15bc-153">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="a15bc-153">managedDeviceIdentifier</span></span>|<span data-ttu-id="a15bc-154">String</span><span class="sxs-lookup"><span data-stu-id="a15bc-154">String</span></span>|<span data-ttu-id="a15bc-155">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="a15bc-155">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="a15bc-156">トラブルシューティングのエラーの詳細</span><span class="sxs-lookup"><span data-stu-id="a15bc-156">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="a15bc-157">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="a15bc-157">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="a15bc-158">エラーとその修復に関する詳細情報を含むオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="a15bc-158">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="a15bc-159">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a15bc-159">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a15bc-160">userId</span><span class="sxs-lookup"><span data-stu-id="a15bc-160">userId</span></span>|<span data-ttu-id="a15bc-161">String</span><span class="sxs-lookup"><span data-stu-id="a15bc-161">String</span></span>|<span data-ttu-id="a15bc-162">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="a15bc-162">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a15bc-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a15bc-163">Relationships</span></span>
|<span data-ttu-id="a15bc-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a15bc-164">Relationship</span></span>|<span data-ttu-id="a15bc-165">型</span><span class="sxs-lookup"><span data-stu-id="a15bc-165">Type</span></span>|<span data-ttu-id="a15bc-166">説明</span><span class="sxs-lookup"><span data-stu-id="a15bc-166">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a15bc-167">**デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="a15bc-167">**Device management**</span></span>|
|<span data-ttu-id="a15bc-168">appLogCollectionRequests</span><span class="sxs-lookup"><span data-stu-id="a15bc-168">appLogCollectionRequests</span></span>|<span data-ttu-id="a15bc-169">[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a15bc-169">[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) collection</span></span>|<span data-ttu-id="a15bc-170">このプロパティは、を指定します。</span><span class="sxs-lookup"><span data-stu-id="a15bc-170">The collection property of AppLogUploadRequest.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a15bc-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a15bc-171">JSON Representation</span></span>
<span data-ttu-id="a15bc-172">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a15bc-172">Here is a JSON representation of the resource.</span></span>
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




