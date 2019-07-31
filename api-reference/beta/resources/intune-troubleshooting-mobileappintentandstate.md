---
title: mobileAppIntentAndState リソースの種類
description: 特定のデバイスの MobileApp インテントとインストール状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f46374e0b766d07f16becfc4861f6574967e2a1b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967200"
---
# <a name="mobileappintentandstate-resource-type"></a><span data-ttu-id="0e66e-103">mobileAppIntentAndState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0e66e-103">mobileAppIntentAndState resource type</span></span>

> <span data-ttu-id="0e66e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e66e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e66e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0e66e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e66e-106">特定のデバイスの MobileApp インテントとインストール状態。</span><span class="sxs-lookup"><span data-stu-id="0e66e-106">MobileApp Intent and Install State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="0e66e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0e66e-107">Methods</span></span>
|<span data-ttu-id="0e66e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0e66e-108">Method</span></span>|<span data-ttu-id="0e66e-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0e66e-109">Return Type</span></span>|<span data-ttu-id="0e66e-110">説明</span><span class="sxs-lookup"><span data-stu-id="0e66e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0e66e-111">リスト mobileAppIntentAndStates</span><span class="sxs-lookup"><span data-stu-id="0e66e-111">List mobileAppIntentAndStates</span></span>](../api/intune-troubleshooting-mobileappintentandstate-list.md)|<span data-ttu-id="0e66e-112">[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0e66e-112">[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) collection</span></span>|<span data-ttu-id="0e66e-113">[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0e66e-113">List properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects.</span></span>|
|[<span data-ttu-id="0e66e-114">MobileAppIntentAndState を取得する</span><span class="sxs-lookup"><span data-stu-id="0e66e-114">Get mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-get.md)|[<span data-ttu-id="0e66e-115">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="0e66e-115">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="0e66e-116">[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0e66e-116">Read properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|
|[<span data-ttu-id="0e66e-117">MobileAppIntentAndState を作成する</span><span class="sxs-lookup"><span data-stu-id="0e66e-117">Create mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-create.md)|[<span data-ttu-id="0e66e-118">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="0e66e-118">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="0e66e-119">新しい[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0e66e-119">Create a new [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|
|[<span data-ttu-id="0e66e-120">MobileAppIntentAndState の削除</span><span class="sxs-lookup"><span data-stu-id="0e66e-120">Delete mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-delete.md)|<span data-ttu-id="0e66e-121">None</span><span class="sxs-lookup"><span data-stu-id="0e66e-121">None</span></span>|<span data-ttu-id="0e66e-122">[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="0e66e-122">Deletes a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>|
|[<span data-ttu-id="0e66e-123">MobileAppIntentAndState の更新</span><span class="sxs-lookup"><span data-stu-id="0e66e-123">Update mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-update.md)|[<span data-ttu-id="0e66e-124">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="0e66e-124">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="0e66e-125">[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0e66e-125">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0e66e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e66e-126">Properties</span></span>
|<span data-ttu-id="0e66e-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e66e-127">Property</span></span>|<span data-ttu-id="0e66e-128">型</span><span class="sxs-lookup"><span data-stu-id="0e66e-128">Type</span></span>|<span data-ttu-id="0e66e-129">説明</span><span class="sxs-lookup"><span data-stu-id="0e66e-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e66e-130">id</span><span class="sxs-lookup"><span data-stu-id="0e66e-130">id</span></span>|<span data-ttu-id="0e66e-131">文字列</span><span class="sxs-lookup"><span data-stu-id="0e66e-131">String</span></span>|<span data-ttu-id="0e66e-132">オブジェクトの UUID</span><span class="sxs-lookup"><span data-stu-id="0e66e-132">UUID for the object</span></span>|
|<span data-ttu-id="0e66e-133">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="0e66e-133">managedDeviceIdentifier</span></span>|<span data-ttu-id="0e66e-134">String</span><span class="sxs-lookup"><span data-stu-id="0e66e-134">String</span></span>|<span data-ttu-id="0e66e-135">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="0e66e-135">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="0e66e-136">userId</span><span class="sxs-lookup"><span data-stu-id="0e66e-136">userId</span></span>|<span data-ttu-id="0e66e-137">String</span><span class="sxs-lookup"><span data-stu-id="0e66e-137">String</span></span>|<span data-ttu-id="0e66e-138">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="0e66e-138">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="0e66e-139">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="0e66e-139">mobileAppList</span></span>|<span data-ttu-id="0e66e-140">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0e66e-140">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="0e66e-141">テナントのペイロードの意図と状態の一覧。</span><span class="sxs-lookup"><span data-stu-id="0e66e-141">The list of payload intents and states for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e66e-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0e66e-142">Relationships</span></span>
<span data-ttu-id="0e66e-143">なし</span><span class="sxs-lookup"><span data-stu-id="0e66e-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e66e-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0e66e-144">JSON Representation</span></span>
<span data-ttu-id="0e66e-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0e66e-145">Here is a JSON representation of the resource.</span></span>
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





