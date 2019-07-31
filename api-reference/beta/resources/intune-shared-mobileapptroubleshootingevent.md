---
title: mobileAppTroubleshootingEvent リソースの種類
description: 複数のワークフローをサポートする Microsoft Graph API for Intune の mobileAppTroubleshootingEvent リソースについて説明します。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f91bb53926bdcc99d4b7796c40d5679a7685d8e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010407"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a><span data-ttu-id="bcf0b-103">mobileAppTroubleshootingEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bcf0b-103">mobileAppTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="bcf0b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bcf0b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcf0b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bcf0b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcf0b-106">デバイスの管理とトラブルシューティングのイベントワークフローについて、ユーザーのデバイスアプリケーションのインストール状態を表すイベント。</span><span class="sxs-lookup"><span data-stu-id="bcf0b-106">Event representing a users device application install status for device management and troubleshooting event workflows.</span></span>

## <a name="methods"></a><span data-ttu-id="bcf0b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="bcf0b-107">Methods</span></span>
|<span data-ttu-id="bcf0b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="bcf0b-108">Method</span></span>|<span data-ttu-id="bcf0b-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bcf0b-109">Return Type</span></span>|<span data-ttu-id="bcf0b-110">説明</span><span class="sxs-lookup"><span data-stu-id="bcf0b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bcf0b-111">リスト mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="bcf0b-111">List mobileAppTroubleshootingEvents</span></span>](../api/intune-shared-mobileapptroubleshootingevent-list.md)|<span data-ttu-id="bcf0b-112">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bcf0b-112">[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) collection</span></span>|<span data-ttu-id="bcf0b-113">[MobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="bcf0b-113">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="bcf0b-114">MobileAppTroubleshootingEvent を取得する</span><span class="sxs-lookup"><span data-stu-id="bcf0b-114">Get mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-get.md)|[<span data-ttu-id="bcf0b-115">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="bcf0b-115">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="bcf0b-116">[MobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bcf0b-116">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="bcf0b-117">MobileAppTroubleshootingEvent を作成する</span><span class="sxs-lookup"><span data-stu-id="bcf0b-117">Create mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-create.md)|[<span data-ttu-id="bcf0b-118">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="bcf0b-118">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="bcf0b-119">新しい[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bcf0b-119">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="bcf0b-120">MobileAppTroubleshootingEvent の削除</span><span class="sxs-lookup"><span data-stu-id="bcf0b-120">Delete mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-delete.md)|<span data-ttu-id="bcf0b-121">None</span><span class="sxs-lookup"><span data-stu-id="bcf0b-121">None</span></span>|<span data-ttu-id="bcf0b-122">[MobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="bcf0b-122">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="bcf0b-123">MobileAppTroubleshootingEvent の更新</span><span class="sxs-lookup"><span data-stu-id="bcf0b-123">Update mobileAppTroubleshootingEvent</span></span>](../api/intune-shared-mobileapptroubleshootingevent-update.md)|[<span data-ttu-id="bcf0b-124">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="bcf0b-124">mobileAppTroubleshootingEvent</span></span>](../resources/intune-shared-mobileapptroubleshootingevent.md)|<span data-ttu-id="bcf0b-125">[MobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bcf0b-125">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bcf0b-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bcf0b-126">Properties</span></span>
|<span data-ttu-id="bcf0b-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bcf0b-127">Property</span></span>|<span data-ttu-id="bcf0b-128">型</span><span class="sxs-lookup"><span data-stu-id="bcf0b-128">Type</span></span>|<span data-ttu-id="bcf0b-129">説明</span><span class="sxs-lookup"><span data-stu-id="bcf0b-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcf0b-130">id</span><span class="sxs-lookup"><span data-stu-id="bcf0b-130">id</span></span>|<span data-ttu-id="bcf0b-131">文字列</span><span class="sxs-lookup"><span data-stu-id="bcf0b-131">String</span></span>|<span data-ttu-id="bcf0b-132">オブジェクトの UUID。</span><span class="sxs-lookup"><span data-stu-id="bcf0b-132">UUID for the object.</span></span>|
|<span data-ttu-id="bcf0b-133">**トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="bcf0b-133">**Troubleshooting**</span></span>|
|<span data-ttu-id="bcf0b-134">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="bcf0b-134">additionalInformation</span></span>|<span data-ttu-id="bcf0b-135">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bcf0b-135">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="bcf0b-136">[Devicemanagementトラブルシューティングイベント](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されたトラブルシューティングイベントに関する追加情報を提供する文字列キーと文字列値のペアのセット。</span><span class="sxs-lookup"><span data-stu-id="bcf0b-136">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="bcf0b-137">applicationId</span><span class="sxs-lookup"><span data-stu-id="bcf0b-137">applicationId</span></span>|<span data-ttu-id="bcf0b-138">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="bcf0b-138">String</span></span>|<span data-ttu-id="bcf0b-139">Intune アプリケーション識別子。</span><span class="sxs-lookup"><span data-stu-id="bcf0b-139">Intune application identifier.</span></span>|
|<span data-ttu-id="bcf0b-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="bcf0b-140">correlationId</span></span>|<span data-ttu-id="bcf0b-141">String</span><span class="sxs-lookup"><span data-stu-id="bcf0b-141">String</span></span>|<span data-ttu-id="bcf0b-142">サービスのエラーをトレースするために使用される ID。</span><span class="sxs-lookup"><span data-stu-id="bcf0b-142">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="bcf0b-143">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="bcf0b-143">eventDateTime</span></span>|<span data-ttu-id="bcf0b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcf0b-144">DateTimeOffset</span></span>|<span data-ttu-id="bcf0b-145">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="bcf0b-145">Time when the event occurred .</span></span> |
|<span data-ttu-id="bcf0b-146">eventName</span><span class="sxs-lookup"><span data-stu-id="bcf0b-146">eventName</span></span>|<span data-ttu-id="bcf0b-147">String</span><span class="sxs-lookup"><span data-stu-id="bcf0b-147">String</span></span>|<span data-ttu-id="bcf0b-148">トラブルシューティングイベントに対応するイベント名。</span><span class="sxs-lookup"><span data-stu-id="bcf0b-148">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="bcf0b-149">省略可能</span><span class="sxs-lookup"><span data-stu-id="bcf0b-149">Optional</span></span>|
|<span data-ttu-id="bcf0b-150">履歴</span><span class="sxs-lookup"><span data-stu-id="bcf0b-150">history</span></span>|<span data-ttu-id="bcf0b-151">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bcf0b-151">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="bcf0b-152">Intune モバイルアプリケーションのトラブルシューティングの履歴項目</span><span class="sxs-lookup"><span data-stu-id="bcf0b-152">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="bcf0b-153">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="bcf0b-153">managedDeviceIdentifier</span></span>|<span data-ttu-id="bcf0b-154">String</span><span class="sxs-lookup"><span data-stu-id="bcf0b-154">String</span></span>|<span data-ttu-id="bcf0b-155">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="bcf0b-155">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="bcf0b-156">トラブルシューティングのエラーの詳細</span><span class="sxs-lookup"><span data-stu-id="bcf0b-156">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="bcf0b-157">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="bcf0b-157">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="bcf0b-158">エラーとその修復に関する詳細情報を含むオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="bcf0b-158">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="bcf0b-159">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bcf0b-159">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="bcf0b-160">userId</span><span class="sxs-lookup"><span data-stu-id="bcf0b-160">userId</span></span>|<span data-ttu-id="bcf0b-161">String</span><span class="sxs-lookup"><span data-stu-id="bcf0b-161">String</span></span>|<span data-ttu-id="bcf0b-162">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="bcf0b-162">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bcf0b-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bcf0b-163">Relationships</span></span>
|<span data-ttu-id="bcf0b-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bcf0b-164">Relationship</span></span>|<span data-ttu-id="bcf0b-165">型</span><span class="sxs-lookup"><span data-stu-id="bcf0b-165">Type</span></span>|<span data-ttu-id="bcf0b-166">説明</span><span class="sxs-lookup"><span data-stu-id="bcf0b-166">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcf0b-167">**デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="bcf0b-167">**Device management**</span></span>|
|<span data-ttu-id="bcf0b-168">appLogCollectionRequests</span><span class="sxs-lookup"><span data-stu-id="bcf0b-168">appLogCollectionRequests</span></span>|<span data-ttu-id="bcf0b-169">[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bcf0b-169">[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) collection</span></span>|<span data-ttu-id="bcf0b-170">このプロパティは、を指定します。</span><span class="sxs-lookup"><span data-stu-id="bcf0b-170">The collection property of AppLogUploadRequest.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="bcf0b-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bcf0b-171">JSON Representation</span></span>
<span data-ttu-id="bcf0b-172">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bcf0b-172">Here is a JSON representation of the resource.</span></span>
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




