---
title: embeddedSIMActivationCodePool リソースの種類
description: プールは、埋め込まれた SIM アクティブ化コードのグループを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f1402c699e490593036ac6836c70abe43731826c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998801"
---
# <a name="embeddedsimactivationcodepool-resource-type"></a><span data-ttu-id="cea62-103">embeddedSIMActivationCodePool リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cea62-103">embeddedSIMActivationCodePool resource type</span></span>

> <span data-ttu-id="cea62-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cea62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cea62-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cea62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cea62-106">プールは、埋め込まれた SIM アクティブ化コードのグループを表します。</span><span class="sxs-lookup"><span data-stu-id="cea62-106">A pool represents a group of embedded SIM activation codes.</span></span>

## <a name="methods"></a><span data-ttu-id="cea62-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="cea62-107">Methods</span></span>
|<span data-ttu-id="cea62-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="cea62-108">Method</span></span>|<span data-ttu-id="cea62-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cea62-109">Return Type</span></span>|<span data-ttu-id="cea62-110">説明</span><span class="sxs-lookup"><span data-stu-id="cea62-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cea62-111">リスト embeddedSIMActivationCodePools</span><span class="sxs-lookup"><span data-stu-id="cea62-111">List embeddedSIMActivationCodePools</span></span>](../api/intune-esim-embeddedsimactivationcodepool-list.md)|<span data-ttu-id="cea62-112">[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cea62-112">[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) collection</span></span>|<span data-ttu-id="cea62-113">[EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="cea62-113">List properties and relationships of the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) objects.</span></span>|
|[<span data-ttu-id="cea62-114">EmbeddedSIMActivationCodePool を取得する</span><span class="sxs-lookup"><span data-stu-id="cea62-114">Get embeddedSIMActivationCodePool</span></span>](../api/intune-esim-embeddedsimactivationcodepool-get.md)|[<span data-ttu-id="cea62-115">embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="cea62-115">embeddedSIMActivationCodePool</span></span>](../resources/intune-esim-embeddedsimactivationcodepool.md)|<span data-ttu-id="cea62-116">[EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="cea62-116">Read properties and relationships of the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>|
|[<span data-ttu-id="cea62-117">EmbeddedSIMActivationCodePool を作成する</span><span class="sxs-lookup"><span data-stu-id="cea62-117">Create embeddedSIMActivationCodePool</span></span>](../api/intune-esim-embeddedsimactivationcodepool-create.md)|[<span data-ttu-id="cea62-118">embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="cea62-118">embeddedSIMActivationCodePool</span></span>](../resources/intune-esim-embeddedsimactivationcodepool.md)|<span data-ttu-id="cea62-119">新しい[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cea62-119">Create a new [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>|
|[<span data-ttu-id="cea62-120">EmbeddedSIMActivationCodePool の削除</span><span class="sxs-lookup"><span data-stu-id="cea62-120">Delete embeddedSIMActivationCodePool</span></span>](../api/intune-esim-embeddedsimactivationcodepool-delete.md)|<span data-ttu-id="cea62-121">None</span><span class="sxs-lookup"><span data-stu-id="cea62-121">None</span></span>|<span data-ttu-id="cea62-122">[EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="cea62-122">Deletes a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span></span>|
|[<span data-ttu-id="cea62-123">EmbeddedSIMActivationCodePool の更新</span><span class="sxs-lookup"><span data-stu-id="cea62-123">Update embeddedSIMActivationCodePool</span></span>](../api/intune-esim-embeddedsimactivationcodepool-update.md)|[<span data-ttu-id="cea62-124">embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="cea62-124">embeddedSIMActivationCodePool</span></span>](../resources/intune-esim-embeddedsimactivationcodepool.md)|<span data-ttu-id="cea62-125">[EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cea62-125">Update the properties of a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>|
|[<span data-ttu-id="cea62-126">assign アクション</span><span class="sxs-lookup"><span data-stu-id="cea62-126">assign action</span></span>](../api/intune-esim-embeddedsimactivationcodepool-assign.md)|<span data-ttu-id="cea62-127">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cea62-127">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="cea62-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cea62-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="cea62-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cea62-129">Properties</span></span>
|<span data-ttu-id="cea62-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cea62-130">Property</span></span>|<span data-ttu-id="cea62-131">型</span><span class="sxs-lookup"><span data-stu-id="cea62-131">Type</span></span>|<span data-ttu-id="cea62-132">説明</span><span class="sxs-lookup"><span data-stu-id="cea62-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cea62-133">id</span><span class="sxs-lookup"><span data-stu-id="cea62-133">id</span></span>|<span data-ttu-id="cea62-134">文字列</span><span class="sxs-lookup"><span data-stu-id="cea62-134">String</span></span>|<span data-ttu-id="cea62-135">埋め込まれた SIM アクティブ化コードプールの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="cea62-135">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="cea62-136">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="cea62-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="cea62-137">displayName</span><span class="sxs-lookup"><span data-stu-id="cea62-137">displayName</span></span>|<span data-ttu-id="cea62-138">String</span><span class="sxs-lookup"><span data-stu-id="cea62-138">String</span></span>|<span data-ttu-id="cea62-139">埋め込まれた SIM アクティブ化コードプールの管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="cea62-139">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="cea62-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cea62-140">createdDateTime</span></span>|<span data-ttu-id="cea62-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cea62-141">DateTimeOffset</span></span>|<span data-ttu-id="cea62-142">埋め込まれた SIM ライセンス認証コードプールが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="cea62-142">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="cea62-143">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="cea62-143">Generated service side.</span></span>|
|<span data-ttu-id="cea62-144">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cea62-144">modifiedDateTime</span></span>|<span data-ttu-id="cea62-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cea62-145">DateTimeOffset</span></span>|<span data-ttu-id="cea62-146">埋め込まれた SIM ライセンス認証コードプールが最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="cea62-146">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="cea62-147">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="cea62-147">Updated service side.</span></span>|
|<span data-ttu-id="cea62-148">activationCodes</span><span class="sxs-lookup"><span data-stu-id="cea62-148">activationCodes</span></span>|<span data-ttu-id="cea62-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cea62-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="cea62-150">このプールに属するアクティブ化コード。</span><span class="sxs-lookup"><span data-stu-id="cea62-150">The activation codes which belong to this pool.</span></span> <span data-ttu-id="cea62-151">このナビゲーションプロパティは、アクティブ化コードを Intune に送信するために使用されますが、Intune からのアクティブ化コードの読み取りには使用できません。</span><span class="sxs-lookup"><span data-stu-id="cea62-151">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="cea62-152">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="cea62-152">activationCodeCount</span></span>|<span data-ttu-id="cea62-153">Int32</span><span class="sxs-lookup"><span data-stu-id="cea62-153">Int32</span></span>|<span data-ttu-id="cea62-154">このプールに属するアクティブ化コードの合計数。</span><span class="sxs-lookup"><span data-stu-id="cea62-154">The total count of activation codes which belong to this pool.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cea62-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cea62-155">Relationships</span></span>
|<span data-ttu-id="cea62-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cea62-156">Relationship</span></span>|<span data-ttu-id="cea62-157">型</span><span class="sxs-lookup"><span data-stu-id="cea62-157">Type</span></span>|<span data-ttu-id="cea62-158">説明</span><span class="sxs-lookup"><span data-stu-id="cea62-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cea62-159">assignments</span><span class="sxs-lookup"><span data-stu-id="cea62-159">assignments</span></span>|<span data-ttu-id="cea62-160">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cea62-160">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="cea62-161">このプールが割り当てられているターゲットのリストへのナビゲーションプロパティ。</span><span class="sxs-lookup"><span data-stu-id="cea62-161">Navigational property to a list of targets to which this pool is assigned.</span></span>|
|<span data-ttu-id="cea62-162">deviceStates</span><span class="sxs-lookup"><span data-stu-id="cea62-162">deviceStates</span></span>|<span data-ttu-id="cea62-163">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cea62-163">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) collection</span></span>|<span data-ttu-id="cea62-164">このプールのデバイス状態のリストへのナビゲーションプロパティ。</span><span class="sxs-lookup"><span data-stu-id="cea62-164">Navigational property to a list of device states for this pool.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cea62-165">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cea62-165">JSON Representation</span></span>
<span data-ttu-id="cea62-166">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cea62-166">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCodePool"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "String",
      "matchingIdentifier": "String",
      "smdpPlusServerAddress": "String"
    }
  ],
  "activationCodeCount": 1024
}
```





