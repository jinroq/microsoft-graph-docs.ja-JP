---
title: mobileAppIntentAndState リソースの種類
description: MobileApp の意図と特定のデバイスのインストールの状態です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 01792d30bdf821d4dd0795926e116bdc12b95ad9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402406"
---
# <a name="mobileappintentandstate-resource-type"></a><span data-ttu-id="f5612-103">mobileAppIntentAndState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f5612-103">mobileAppIntentAndState resource type</span></span>

> <span data-ttu-id="f5612-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f5612-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f5612-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5612-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5612-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f5612-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5612-107">MobileApp の意図と特定のデバイスのインストールの状態です。</span><span class="sxs-lookup"><span data-stu-id="f5612-107">MobileApp Intent and Install State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="f5612-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f5612-108">Methods</span></span>
|<span data-ttu-id="f5612-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="f5612-109">Method</span></span>|<span data-ttu-id="f5612-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f5612-110">Return Type</span></span>|<span data-ttu-id="f5612-111">説明</span><span class="sxs-lookup"><span data-stu-id="f5612-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f5612-112">リスト mobileAppIntentAndStates</span><span class="sxs-lookup"><span data-stu-id="f5612-112">List mobileAppIntentAndStates</span></span>](../api/intune-troubleshooting-mobileappintentandstate-list.md)|<span data-ttu-id="f5612-113">[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f5612-113">[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) collection</span></span>|<span data-ttu-id="f5612-114">[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="f5612-114">List properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects.</span></span>|
|[<span data-ttu-id="f5612-115">MobileAppIntentAndState を取得します。</span><span class="sxs-lookup"><span data-stu-id="f5612-115">Get mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-get.md)|[<span data-ttu-id="f5612-116">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="f5612-116">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="f5612-117">[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5612-117">Read properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|
|[<span data-ttu-id="f5612-118">MobileAppIntentAndState を作成します。</span><span class="sxs-lookup"><span data-stu-id="f5612-118">Create mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-create.md)|[<span data-ttu-id="f5612-119">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="f5612-119">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="f5612-120">新しい[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f5612-120">Create a new [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|
|[<span data-ttu-id="f5612-121">MobileAppIntentAndState を削除します。</span><span class="sxs-lookup"><span data-stu-id="f5612-121">Delete mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-delete.md)|<span data-ttu-id="f5612-122">なし</span><span class="sxs-lookup"><span data-stu-id="f5612-122">None</span></span>|<span data-ttu-id="f5612-123">の[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="f5612-123">Deletes a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>|
|[<span data-ttu-id="f5612-124">MobileAppIntentAndState を更新します。</span><span class="sxs-lookup"><span data-stu-id="f5612-124">Update mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-update.md)|[<span data-ttu-id="f5612-125">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="f5612-125">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="f5612-126">[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f5612-126">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f5612-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5612-127">Properties</span></span>
|<span data-ttu-id="f5612-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5612-128">Property</span></span>|<span data-ttu-id="f5612-129">型</span><span class="sxs-lookup"><span data-stu-id="f5612-129">Type</span></span>|<span data-ttu-id="f5612-130">説明</span><span class="sxs-lookup"><span data-stu-id="f5612-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5612-131">id</span><span class="sxs-lookup"><span data-stu-id="f5612-131">id</span></span>|<span data-ttu-id="f5612-132">String</span><span class="sxs-lookup"><span data-stu-id="f5612-132">String</span></span>|<span data-ttu-id="f5612-133">オブジェクトの UUID</span><span class="sxs-lookup"><span data-stu-id="f5612-133">UUID for the object</span></span>|
|<span data-ttu-id="f5612-134">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f5612-134">managedDeviceIdentifier</span></span>|<span data-ttu-id="f5612-135">String</span><span class="sxs-lookup"><span data-stu-id="f5612-135">String</span></span>|<span data-ttu-id="f5612-136">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="f5612-136">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="f5612-137">userId</span><span class="sxs-lookup"><span data-stu-id="f5612-137">userId</span></span>|<span data-ttu-id="f5612-138">String</span><span class="sxs-lookup"><span data-stu-id="f5612-138">String</span></span>|<span data-ttu-id="f5612-139">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="f5612-139">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="f5612-140">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="f5612-140">mobileAppList</span></span>|<span data-ttu-id="f5612-141">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f5612-141">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="f5612-142">ペイロードの目的と、テナントの状態の一覧です。</span><span class="sxs-lookup"><span data-stu-id="f5612-142">The list of payload intents and states for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5612-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f5612-143">Relationships</span></span>
<span data-ttu-id="f5612-144">なし</span><span class="sxs-lookup"><span data-stu-id="f5612-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5612-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f5612-145">JSON Representation</span></span>
<span data-ttu-id="f5612-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f5612-146">Here is a JSON representation of the resource.</span></span>
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




