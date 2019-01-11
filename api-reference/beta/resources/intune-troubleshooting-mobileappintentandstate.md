---
title: mobileAppIntentAndState リソースの種類
description: MobileApp の意図と特定のデバイスのインストールの状態です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 037faeb02f18f304153dbe19fef640cc1183ddcd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819797"
---
# <a name="mobileappintentandstate-resource-type"></a><span data-ttu-id="c21f7-103">mobileAppIntentAndState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c21f7-103">mobileAppIntentAndState resource type</span></span>

> <span data-ttu-id="c21f7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c21f7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c21f7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c21f7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c21f7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c21f7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c21f7-107">MobileApp の意図と特定のデバイスのインストールの状態です。</span><span class="sxs-lookup"><span data-stu-id="c21f7-107">MobileApp Intent and Install State for a given device.</span></span>
## <a name="methods"></a><span data-ttu-id="c21f7-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c21f7-108">Methods</span></span>
|<span data-ttu-id="c21f7-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c21f7-109">Method</span></span>|<span data-ttu-id="c21f7-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c21f7-110">Return Type</span></span>|<span data-ttu-id="c21f7-111">説明</span><span class="sxs-lookup"><span data-stu-id="c21f7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c21f7-112">リスト mobileAppIntentAndStates</span><span class="sxs-lookup"><span data-stu-id="c21f7-112">List mobileAppIntentAndStates</span></span>](../api/intune-troubleshooting-mobileappintentandstate-list.md)|<span data-ttu-id="c21f7-113">[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c21f7-113">[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) collection</span></span>|<span data-ttu-id="c21f7-114">[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="c21f7-114">List properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects.</span></span>|
|[<span data-ttu-id="c21f7-115">MobileAppIntentAndState を取得します。</span><span class="sxs-lookup"><span data-stu-id="c21f7-115">Get mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-get.md)|[<span data-ttu-id="c21f7-116">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="c21f7-116">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="c21f7-117">[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c21f7-117">Read properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|
|[<span data-ttu-id="c21f7-118">MobileAppIntentAndState を作成します。</span><span class="sxs-lookup"><span data-stu-id="c21f7-118">Create mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-create.md)|[<span data-ttu-id="c21f7-119">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="c21f7-119">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="c21f7-120">新しい[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c21f7-120">Create a new [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|
|[<span data-ttu-id="c21f7-121">MobileAppIntentAndState を削除します。</span><span class="sxs-lookup"><span data-stu-id="c21f7-121">Delete mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-delete.md)|<span data-ttu-id="c21f7-122">なし</span><span class="sxs-lookup"><span data-stu-id="c21f7-122">None</span></span>|<span data-ttu-id="c21f7-123">の[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="c21f7-123">Deletes a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>|
|[<span data-ttu-id="c21f7-124">MobileAppIntentAndState を更新します。</span><span class="sxs-lookup"><span data-stu-id="c21f7-124">Update mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-update.md)|[<span data-ttu-id="c21f7-125">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="c21f7-125">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="c21f7-126">[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c21f7-126">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c21f7-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c21f7-127">Properties</span></span>
|<span data-ttu-id="c21f7-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c21f7-128">Property</span></span>|<span data-ttu-id="c21f7-129">種類</span><span class="sxs-lookup"><span data-stu-id="c21f7-129">Type</span></span>|<span data-ttu-id="c21f7-130">説明</span><span class="sxs-lookup"><span data-stu-id="c21f7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c21f7-131">ID</span><span class="sxs-lookup"><span data-stu-id="c21f7-131">id</span></span>|<span data-ttu-id="c21f7-132">String</span><span class="sxs-lookup"><span data-stu-id="c21f7-132">String</span></span>|<span data-ttu-id="c21f7-133">オブジェクトの UUID</span><span class="sxs-lookup"><span data-stu-id="c21f7-133">UUID for the object</span></span>|
|<span data-ttu-id="c21f7-134">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="c21f7-134">managedDeviceIdentifier</span></span>|<span data-ttu-id="c21f7-135">String</span><span class="sxs-lookup"><span data-stu-id="c21f7-135">String</span></span>|<span data-ttu-id="c21f7-136">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="c21f7-136">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="c21f7-137">userId</span><span class="sxs-lookup"><span data-stu-id="c21f7-137">userId</span></span>|<span data-ttu-id="c21f7-138">String</span><span class="sxs-lookup"><span data-stu-id="c21f7-138">String</span></span>|<span data-ttu-id="c21f7-139">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="c21f7-139">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="c21f7-140">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="c21f7-140">mobileAppList</span></span>|<span data-ttu-id="c21f7-141">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c21f7-141">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="c21f7-142">ペイロードの目的と、テナントの状態の一覧です。</span><span class="sxs-lookup"><span data-stu-id="c21f7-142">The list of payload intents and states for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c21f7-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c21f7-143">Relationships</span></span>
<span data-ttu-id="c21f7-144">なし</span><span class="sxs-lookup"><span data-stu-id="c21f7-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c21f7-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c21f7-145">JSON Representation</span></span>
<span data-ttu-id="c21f7-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c21f7-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppIntentAndState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "id": "String (identifier)",
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "String",
      "displayName": "String",
      "mobileAppIntent": "String",
      "displayVersion": "String",
      "installState": "String",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "String",
          "minimumOperatingSystemVersion": "String",
          "maximumOperatingSystemVersion": "String"
        }
      ]
    }
  ]
}
```





