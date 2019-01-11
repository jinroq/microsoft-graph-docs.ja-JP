---
title: mobileAppTroubleshootingEvent リソースの種類
description: ユーザー デバイスのアプリケーションを表すイベントは、状態をインストールします。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8441015f594d227066db39f3f643cc8136637668
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846369"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a><span data-ttu-id="6408f-103">mobileAppTroubleshootingEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6408f-103">mobileAppTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="6408f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6408f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6408f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6408f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6408f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6408f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6408f-107">ユーザー デバイスのアプリケーションを表すイベントは、状態をインストールします。</span><span class="sxs-lookup"><span data-stu-id="6408f-107">Event representing a users device application install status.</span></span>

<span data-ttu-id="6408f-108">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="6408f-108">Inherits from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6408f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="6408f-109">Methods</span></span>
|<span data-ttu-id="6408f-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="6408f-110">Method</span></span>|<span data-ttu-id="6408f-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6408f-111">Return Type</span></span>|<span data-ttu-id="6408f-112">説明</span><span class="sxs-lookup"><span data-stu-id="6408f-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6408f-113">リスト mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="6408f-113">List mobileAppTroubleshootingEvents</span></span>](../api/intune-troubleshooting-mobileapptroubleshootingevent-list.md)|<span data-ttu-id="6408f-114">[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6408f-114">[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) collection</span></span>|<span data-ttu-id="6408f-115">[MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="6408f-115">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="6408f-116">MobileAppTroubleshootingEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="6408f-116">Get mobileAppTroubleshootingEvent</span></span>](../api/intune-troubleshooting-mobileapptroubleshootingevent-get.md)|[<span data-ttu-id="6408f-117">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="6408f-117">mobileAppTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)|<span data-ttu-id="6408f-118">[MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6408f-118">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="6408f-119">MobileAppTroubleshootingEvent を作成します。</span><span class="sxs-lookup"><span data-stu-id="6408f-119">Create mobileAppTroubleshootingEvent</span></span>](../api/intune-troubleshooting-mobileapptroubleshootingevent-create.md)|[<span data-ttu-id="6408f-120">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="6408f-120">mobileAppTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)|<span data-ttu-id="6408f-121">新しい[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6408f-121">Create a new [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="6408f-122">MobileAppTroubleshootingEvent を削除します。</span><span class="sxs-lookup"><span data-stu-id="6408f-122">Delete mobileAppTroubleshootingEvent</span></span>](../api/intune-troubleshooting-mobileapptroubleshootingevent-delete.md)|<span data-ttu-id="6408f-123">なし</span><span class="sxs-lookup"><span data-stu-id="6408f-123">None</span></span>|<span data-ttu-id="6408f-124">の[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="6408f-124">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="6408f-125">MobileAppTroubleshootingEvent を更新します。</span><span class="sxs-lookup"><span data-stu-id="6408f-125">Update mobileAppTroubleshootingEvent</span></span>](../api/intune-troubleshooting-mobileapptroubleshootingevent-update.md)|[<span data-ttu-id="6408f-126">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="6408f-126">mobileAppTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)|<span data-ttu-id="6408f-127">[MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6408f-127">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6408f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6408f-128">Properties</span></span>
|<span data-ttu-id="6408f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6408f-129">Property</span></span>|<span data-ttu-id="6408f-130">種類</span><span class="sxs-lookup"><span data-stu-id="6408f-130">Type</span></span>|<span data-ttu-id="6408f-131">説明</span><span class="sxs-lookup"><span data-stu-id="6408f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6408f-132">ID</span><span class="sxs-lookup"><span data-stu-id="6408f-132">id</span></span>|<span data-ttu-id="6408f-133">String</span><span class="sxs-lookup"><span data-stu-id="6408f-133">String</span></span>|<span data-ttu-id="6408f-134">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="6408f-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="6408f-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="6408f-135">eventDateTime</span></span>|<span data-ttu-id="6408f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6408f-136">DateTimeOffset</span></span>|<span data-ttu-id="6408f-137">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="6408f-137">Time when the event occurred .</span></span> <span data-ttu-id="6408f-138">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6408f-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="6408f-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="6408f-139">correlationId</span></span>|<span data-ttu-id="6408f-140">String</span><span class="sxs-lookup"><span data-stu-id="6408f-140">String</span></span>|<span data-ttu-id="6408f-141">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="6408f-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="6408f-142">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6408f-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="6408f-143">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="6408f-143">managedDeviceIdentifier</span></span>|<span data-ttu-id="6408f-144">String</span><span class="sxs-lookup"><span data-stu-id="6408f-144">String</span></span>|<span data-ttu-id="6408f-145">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="6408f-145">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="6408f-146">userId</span><span class="sxs-lookup"><span data-stu-id="6408f-146">userId</span></span>|<span data-ttu-id="6408f-147">String</span><span class="sxs-lookup"><span data-stu-id="6408f-147">String</span></span>|<span data-ttu-id="6408f-148">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="6408f-148">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="6408f-149">applicationId</span><span class="sxs-lookup"><span data-stu-id="6408f-149">applicationId</span></span>|<span data-ttu-id="6408f-150">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="6408f-150">String</span></span>|<span data-ttu-id="6408f-151">Intune アプリケーション識別子です。</span><span class="sxs-lookup"><span data-stu-id="6408f-151">Intune application identifier.</span></span>|
|<span data-ttu-id="6408f-152">履歴</span><span class="sxs-lookup"><span data-stu-id="6408f-152">history</span></span>|<span data-ttu-id="6408f-153">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6408f-153">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="6408f-154">Intune モバイル アプリケーションの履歴項目のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="6408f-154">Intune Mobile Application Troubleshooting History Item</span></span>|

## <a name="relationships"></a><span data-ttu-id="6408f-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6408f-155">Relationships</span></span>
<span data-ttu-id="6408f-156">なし</span><span class="sxs-lookup"><span data-stu-id="6408f-156">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6408f-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6408f-157">JSON Representation</span></span>
<span data-ttu-id="6408f-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6408f-158">Here is a JSON representation of the resource.</span></span>
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





