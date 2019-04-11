---
title: embeddedSIMActivationCodePoolAssignment リソースの種類
description: 埋め込まれた SIM ライセンス認証コードプール割り当てエンティティは、特定の embeddedSIMActivationCodePool を AAD デバイスグループに割り当てます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a5ec64384bd5620b74f9cdca2148e6b3064e9c98
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771524"
---
# <a name="embeddedsimactivationcodepoolassignment-resource-type"></a><span data-ttu-id="10024-103">embeddedSIMActivationCodePoolAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="10024-103">embeddedSIMActivationCodePoolAssignment resource type</span></span>

> <span data-ttu-id="10024-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="10024-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10024-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="10024-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10024-106">埋め込まれた SIM ライセンス認証コードプール割り当てエンティティは、特定の embeddedSIMActivationCodePool を AAD デバイスグループに割り当てます。</span><span class="sxs-lookup"><span data-stu-id="10024-106">The embedded SIM activation code pool assignment entity assigns a specific embeddedSIMActivationCodePool to an AAD device group.</span></span>

## <a name="methods"></a><span data-ttu-id="10024-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="10024-107">Methods</span></span>
|<span data-ttu-id="10024-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="10024-108">Method</span></span>|<span data-ttu-id="10024-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="10024-109">Return Type</span></span>|<span data-ttu-id="10024-110">説明</span><span class="sxs-lookup"><span data-stu-id="10024-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="10024-111">リスト embeddedSIMActivationCodePoolAssignments</span><span class="sxs-lookup"><span data-stu-id="10024-111">List embeddedSIMActivationCodePoolAssignments</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-list.md)|<span data-ttu-id="10024-112">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="10024-112">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="10024-113">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="10024-113">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>|
|[<span data-ttu-id="10024-114">embeddedSIMActivationCodePoolAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="10024-114">Get embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-get.md)|[<span data-ttu-id="10024-115">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="10024-115">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="10024-116">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="10024-116">Read properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="10024-117">embeddedSIMActivationCodePoolAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="10024-117">Create embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-create.md)|[<span data-ttu-id="10024-118">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="10024-118">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="10024-119">新しい[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="10024-119">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="10024-120">embeddedSIMActivationCodePoolAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="10024-120">Delete embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-delete.md)|<span data-ttu-id="10024-121">なし</span><span class="sxs-lookup"><span data-stu-id="10024-121">None</span></span>|<span data-ttu-id="10024-122">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="10024-122">Deletes a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>|
|[<span data-ttu-id="10024-123">embeddedSIMActivationCodePoolAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="10024-123">Update embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-update.md)|[<span data-ttu-id="10024-124">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="10024-124">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="10024-125">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="10024-125">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="10024-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="10024-126">Properties</span></span>
|<span data-ttu-id="10024-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="10024-127">Property</span></span>|<span data-ttu-id="10024-128">型</span><span class="sxs-lookup"><span data-stu-id="10024-128">Type</span></span>|<span data-ttu-id="10024-129">説明</span><span class="sxs-lookup"><span data-stu-id="10024-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10024-130">id</span><span class="sxs-lookup"><span data-stu-id="10024-130">id</span></span>|<span data-ttu-id="10024-131">String</span><span class="sxs-lookup"><span data-stu-id="10024-131">String</span></span>|<span data-ttu-id="10024-132">埋め込まれている SIM ライセンス認証コードプールの割り当ての一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="10024-132">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="10024-133">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="10024-133">System generated value assigned when created.</span></span>|
|<span data-ttu-id="10024-134">target</span><span class="sxs-lookup"><span data-stu-id="10024-134">target</span></span>|[<span data-ttu-id="10024-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="10024-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="10024-136">埋め込まれた SIM アクティブ化コードプールの対象となるグループの種類。</span><span class="sxs-lookup"><span data-stu-id="10024-136">The type of groups targeted by the embedded SIM activation code pool.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10024-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="10024-137">Relationships</span></span>
<span data-ttu-id="10024-138">なし</span><span class="sxs-lookup"><span data-stu-id="10024-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10024-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="10024-139">JSON Representation</span></span>
<span data-ttu-id="10024-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="10024-140">Here is a JSON representation of the resource.</span></span>
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





