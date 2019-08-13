---
title: embeddedSIMActivationCodePoolAssignment リソースの種類
description: 埋め込まれた SIM ライセンス認証コードプール割り当てエンティティは、特定の embeddedSIMActivationCodePool を AAD デバイスグループに割り当てます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 70f9d2bf36fc4c143ad629160089c8a3a988603b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331722"
---
# <a name="embeddedsimactivationcodepoolassignment-resource-type"></a><span data-ttu-id="91457-103">embeddedSIMActivationCodePoolAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="91457-103">embeddedSIMActivationCodePoolAssignment resource type</span></span>

> <span data-ttu-id="91457-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91457-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91457-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="91457-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91457-106">埋め込まれた SIM ライセンス認証コードプール割り当てエンティティは、特定の embeddedSIMActivationCodePool を AAD デバイスグループに割り当てます。</span><span class="sxs-lookup"><span data-stu-id="91457-106">The embedded SIM activation code pool assignment entity assigns a specific embeddedSIMActivationCodePool to an AAD device group.</span></span>

## <a name="methods"></a><span data-ttu-id="91457-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="91457-107">Methods</span></span>
|<span data-ttu-id="91457-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="91457-108">Method</span></span>|<span data-ttu-id="91457-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="91457-109">Return Type</span></span>|<span data-ttu-id="91457-110">説明</span><span class="sxs-lookup"><span data-stu-id="91457-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="91457-111">リスト embeddedSIMActivationCodePoolAssignments</span><span class="sxs-lookup"><span data-stu-id="91457-111">List embeddedSIMActivationCodePoolAssignments</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-list.md)|<span data-ttu-id="91457-112">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="91457-112">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="91457-113">[EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="91457-113">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>|
|[<span data-ttu-id="91457-114">EmbeddedSIMActivationCodePoolAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="91457-114">Get embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-get.md)|[<span data-ttu-id="91457-115">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="91457-115">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="91457-116">[EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="91457-116">Read properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="91457-117">EmbeddedSIMActivationCodePoolAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="91457-117">Create embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-create.md)|[<span data-ttu-id="91457-118">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="91457-118">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="91457-119">新しい[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="91457-119">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="91457-120">EmbeddedSIMActivationCodePoolAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="91457-120">Delete embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-delete.md)|<span data-ttu-id="91457-121">None</span><span class="sxs-lookup"><span data-stu-id="91457-121">None</span></span>|<span data-ttu-id="91457-122">[EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="91457-122">Deletes a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>|
|[<span data-ttu-id="91457-123">EmbeddedSIMActivationCodePoolAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="91457-123">Update embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-update.md)|[<span data-ttu-id="91457-124">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="91457-124">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="91457-125">[EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="91457-125">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="91457-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91457-126">Properties</span></span>
|<span data-ttu-id="91457-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91457-127">Property</span></span>|<span data-ttu-id="91457-128">型</span><span class="sxs-lookup"><span data-stu-id="91457-128">Type</span></span>|<span data-ttu-id="91457-129">説明</span><span class="sxs-lookup"><span data-stu-id="91457-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91457-130">id</span><span class="sxs-lookup"><span data-stu-id="91457-130">id</span></span>|<span data-ttu-id="91457-131">String</span><span class="sxs-lookup"><span data-stu-id="91457-131">String</span></span>|<span data-ttu-id="91457-132">埋め込まれている SIM ライセンス認証コードプールの割り当ての一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="91457-132">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="91457-133">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="91457-133">System generated value assigned when created.</span></span>|
|<span data-ttu-id="91457-134">target</span><span class="sxs-lookup"><span data-stu-id="91457-134">target</span></span>|[<span data-ttu-id="91457-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="91457-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="91457-136">埋め込まれた SIM アクティブ化コードプールの対象となるグループの種類。</span><span class="sxs-lookup"><span data-stu-id="91457-136">The type of groups targeted by the embedded SIM activation code pool.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91457-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="91457-137">Relationships</span></span>
<span data-ttu-id="91457-138">なし</span><span class="sxs-lookup"><span data-stu-id="91457-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91457-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91457-139">JSON Representation</span></span>
<span data-ttu-id="91457-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="91457-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCodePoolAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



