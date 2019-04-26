---
title: embeddedSIMActivationCodePoolAssignment リソースの種類
description: 埋め込まれた SIM ライセンス認証コードプール割り当てエンティティは、特定の embeddedSIMActivationCodePool を AAD デバイスグループに割り当てます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a5ec64384bd5620b74f9cdca2148e6b3064e9c98
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571136"
---
# <a name="embeddedsimactivationcodepoolassignment-resource-type"></a><span data-ttu-id="e4857-103">embeddedSIMActivationCodePoolAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e4857-103">embeddedSIMActivationCodePoolAssignment resource type</span></span>

> <span data-ttu-id="e4857-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e4857-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4857-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e4857-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4857-106">埋め込まれた SIM ライセンス認証コードプール割り当てエンティティは、特定の embeddedSIMActivationCodePool を AAD デバイスグループに割り当てます。</span><span class="sxs-lookup"><span data-stu-id="e4857-106">The embedded SIM activation code pool assignment entity assigns a specific embeddedSIMActivationCodePool to an AAD device group.</span></span>

## <a name="methods"></a><span data-ttu-id="e4857-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e4857-107">Methods</span></span>
|<span data-ttu-id="e4857-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e4857-108">Method</span></span>|<span data-ttu-id="e4857-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e4857-109">Return Type</span></span>|<span data-ttu-id="e4857-110">説明</span><span class="sxs-lookup"><span data-stu-id="e4857-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e4857-111">リスト embeddedSIMActivationCodePoolAssignments</span><span class="sxs-lookup"><span data-stu-id="e4857-111">List embeddedSIMActivationCodePoolAssignments</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-list.md)|<span data-ttu-id="e4857-112">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e4857-112">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="e4857-113">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e4857-113">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>|
|[<span data-ttu-id="e4857-114">embeddedSIMActivationCodePoolAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="e4857-114">Get embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-get.md)|[<span data-ttu-id="e4857-115">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="e4857-115">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="e4857-116">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e4857-116">Read properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="e4857-117">embeddedSIMActivationCodePoolAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="e4857-117">Create embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-create.md)|[<span data-ttu-id="e4857-118">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="e4857-118">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="e4857-119">新しい[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e4857-119">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="e4857-120">embeddedSIMActivationCodePoolAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="e4857-120">Delete embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-delete.md)|<span data-ttu-id="e4857-121">なし</span><span class="sxs-lookup"><span data-stu-id="e4857-121">None</span></span>|<span data-ttu-id="e4857-122">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="e4857-122">Deletes a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>|
|[<span data-ttu-id="e4857-123">embeddedSIMActivationCodePoolAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="e4857-123">Update embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-update.md)|[<span data-ttu-id="e4857-124">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="e4857-124">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="e4857-125">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e4857-125">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e4857-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4857-126">Properties</span></span>
|<span data-ttu-id="e4857-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4857-127">Property</span></span>|<span data-ttu-id="e4857-128">型</span><span class="sxs-lookup"><span data-stu-id="e4857-128">Type</span></span>|<span data-ttu-id="e4857-129">説明</span><span class="sxs-lookup"><span data-stu-id="e4857-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4857-130">id</span><span class="sxs-lookup"><span data-stu-id="e4857-130">id</span></span>|<span data-ttu-id="e4857-131">String</span><span class="sxs-lookup"><span data-stu-id="e4857-131">String</span></span>|<span data-ttu-id="e4857-132">埋め込まれている SIM ライセンス認証コードプールの割り当ての一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="e4857-132">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="e4857-133">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="e4857-133">System generated value assigned when created.</span></span>|
|<span data-ttu-id="e4857-134">target</span><span class="sxs-lookup"><span data-stu-id="e4857-134">target</span></span>|[<span data-ttu-id="e4857-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e4857-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e4857-136">埋め込まれた SIM アクティブ化コードプールの対象となるグループの種類。</span><span class="sxs-lookup"><span data-stu-id="e4857-136">The type of groups targeted by the embedded SIM activation code pool.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4857-137">関係</span><span class="sxs-lookup"><span data-stu-id="e4857-137">Relationships</span></span>
<span data-ttu-id="e4857-138">なし</span><span class="sxs-lookup"><span data-stu-id="e4857-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4857-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e4857-139">JSON Representation</span></span>
<span data-ttu-id="e4857-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e4857-140">Here is a JSON representation of the resource.</span></span>
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





