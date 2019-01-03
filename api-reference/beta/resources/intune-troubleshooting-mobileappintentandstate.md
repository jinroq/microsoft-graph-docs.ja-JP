---
title: mobileAppIntentAndState リソースの種類
description: MobileApp の意図と特定のデバイスのインストールの状態です。
author: tfitzmac
ms.openlocfilehash: 40ffbac3f86ccce3037a6585fa608dd4055bd428
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356057"
---
# <a name="mobileappintentandstate-resource-type"></a><span data-ttu-id="c1a25-103">mobileAppIntentAndState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1a25-103">mobileAppIntentAndState resource type</span></span>

> <span data-ttu-id="c1a25-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c1a25-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1a25-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1a25-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1a25-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c1a25-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1a25-107">MobileApp の意図と特定のデバイスのインストールの状態です。</span><span class="sxs-lookup"><span data-stu-id="c1a25-107">MobileApp Intent and Install State for a given device.</span></span>
## <a name="methods"></a><span data-ttu-id="c1a25-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c1a25-108">Methods</span></span>
|<span data-ttu-id="c1a25-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c1a25-109">Method</span></span>|<span data-ttu-id="c1a25-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c1a25-110">Return Type</span></span>|<span data-ttu-id="c1a25-111">説明</span><span class="sxs-lookup"><span data-stu-id="c1a25-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c1a25-112">リスト mobileAppIntentAndStates</span><span class="sxs-lookup"><span data-stu-id="c1a25-112">List mobileAppIntentAndStates</span></span>](../api/intune-troubleshooting-mobileappintentandstate-list.md)|<span data-ttu-id="c1a25-113">[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c1a25-113">[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) collection</span></span>|<span data-ttu-id="c1a25-114">[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="c1a25-114">List properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects.</span></span>|
|[<span data-ttu-id="c1a25-115">MobileAppIntentAndState を取得します。</span><span class="sxs-lookup"><span data-stu-id="c1a25-115">Get mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-get.md)|[<span data-ttu-id="c1a25-116">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="c1a25-116">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="c1a25-117">[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c1a25-117">Read properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|
|[<span data-ttu-id="c1a25-118">MobileAppIntentAndState を作成します。</span><span class="sxs-lookup"><span data-stu-id="c1a25-118">Create mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-create.md)|[<span data-ttu-id="c1a25-119">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="c1a25-119">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="c1a25-120">新しい[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c1a25-120">Create a new [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|
|[<span data-ttu-id="c1a25-121">MobileAppIntentAndState を削除します。</span><span class="sxs-lookup"><span data-stu-id="c1a25-121">Delete mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-delete.md)|<span data-ttu-id="c1a25-122">なし</span><span class="sxs-lookup"><span data-stu-id="c1a25-122">None</span></span>|<span data-ttu-id="c1a25-123">の[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="c1a25-123">Deletes a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>|
|[<span data-ttu-id="c1a25-124">MobileAppIntentAndState を更新します。</span><span class="sxs-lookup"><span data-stu-id="c1a25-124">Update mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-update.md)|[<span data-ttu-id="c1a25-125">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="c1a25-125">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="c1a25-126">[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c1a25-126">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c1a25-127">Properties</span><span class="sxs-lookup"><span data-stu-id="c1a25-127">Properties</span></span>
|<span data-ttu-id="c1a25-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1a25-128">Property</span></span>|<span data-ttu-id="c1a25-129">種類</span><span class="sxs-lookup"><span data-stu-id="c1a25-129">Type</span></span>|<span data-ttu-id="c1a25-130">説明</span><span class="sxs-lookup"><span data-stu-id="c1a25-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1a25-131">ID</span><span class="sxs-lookup"><span data-stu-id="c1a25-131">id</span></span>|<span data-ttu-id="c1a25-132">String</span><span class="sxs-lookup"><span data-stu-id="c1a25-132">String</span></span>|<span data-ttu-id="c1a25-133">オブジェクトの UUID</span><span class="sxs-lookup"><span data-stu-id="c1a25-133">UUID for the object</span></span>|
|<span data-ttu-id="c1a25-134">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="c1a25-134">managedDeviceIdentifier</span></span>|<span data-ttu-id="c1a25-135">String</span><span class="sxs-lookup"><span data-stu-id="c1a25-135">String</span></span>|<span data-ttu-id="c1a25-136">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="c1a25-136">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="c1a25-137">userId</span><span class="sxs-lookup"><span data-stu-id="c1a25-137">userId</span></span>|<span data-ttu-id="c1a25-138">String</span><span class="sxs-lookup"><span data-stu-id="c1a25-138">String</span></span>|<span data-ttu-id="c1a25-139">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="c1a25-139">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="c1a25-140">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="c1a25-140">mobileAppList</span></span>|<span data-ttu-id="c1a25-141">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c1a25-141">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="c1a25-142">ペイロードの目的と、テナントの状態の一覧です。</span><span class="sxs-lookup"><span data-stu-id="c1a25-142">The list of payload intents and states for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1a25-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c1a25-143">Relationships</span></span>
<span data-ttu-id="c1a25-144">なし</span><span class="sxs-lookup"><span data-stu-id="c1a25-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c1a25-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1a25-145">JSON Representation</span></span>
<span data-ttu-id="c1a25-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c1a25-146">Here is a JSON representation of the resource.</span></span>
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




