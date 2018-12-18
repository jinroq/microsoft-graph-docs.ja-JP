---
title: deviceConfigurationAssignment リソースの種類
description: デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。
author: tfitzmac
ms.openlocfilehash: ef5a9156b98eb8915471dbc042f6e028542be768
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343296"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="0f1fa-103">deviceConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0f1fa-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="0f1fa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0f1fa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f1fa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f1fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f1fa-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0f1fa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f1fa-107">デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="0f1fa-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="0f1fa-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0f1fa-108">Methods</span></span>
|<span data-ttu-id="0f1fa-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="0f1fa-109">Method</span></span>|<span data-ttu-id="0f1fa-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0f1fa-110">Return Type</span></span>|<span data-ttu-id="0f1fa-111">説明</span><span class="sxs-lookup"><span data-stu-id="0f1fa-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0f1fa-112">deviceConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="0f1fa-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="0f1fa-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0f1fa-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0f1fa-114">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0f1fa-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="0f1fa-115">deviceConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="0f1fa-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="0f1fa-116">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0f1fa-116">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="0f1fa-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0f1fa-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="0f1fa-118">deviceConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="0f1fa-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="0f1fa-119">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0f1fa-119">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="0f1fa-120">新しい [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0f1fa-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="0f1fa-121">deviceConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="0f1fa-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="0f1fa-122">なし</span><span class="sxs-lookup"><span data-stu-id="0f1fa-122">None</span></span>|<span data-ttu-id="0f1fa-123">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="0f1fa-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="0f1fa-124">deviceConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="0f1fa-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="0f1fa-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0f1fa-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="0f1fa-126">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0f1fa-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0f1fa-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f1fa-127">Properties</span></span>
|<span data-ttu-id="0f1fa-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f1fa-128">Property</span></span>|<span data-ttu-id="0f1fa-129">種類</span><span class="sxs-lookup"><span data-stu-id="0f1fa-129">Type</span></span>|<span data-ttu-id="0f1fa-130">説明</span><span class="sxs-lookup"><span data-stu-id="0f1fa-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f1fa-131">ID</span><span class="sxs-lookup"><span data-stu-id="0f1fa-131">id</span></span>|<span data-ttu-id="0f1fa-132">String</span><span class="sxs-lookup"><span data-stu-id="0f1fa-132">String</span></span>|<span data-ttu-id="0f1fa-133">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="0f1fa-133">The key of the assignment.</span></span>|
|<span data-ttu-id="0f1fa-134">target</span><span class="sxs-lookup"><span data-stu-id="0f1fa-134">target</span></span>|[<span data-ttu-id="0f1fa-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0f1fa-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0f1fa-136">デバイス構成の割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="0f1fa-136">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f1fa-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0f1fa-137">Relationships</span></span>
<span data-ttu-id="0f1fa-138">なし</span><span class="sxs-lookup"><span data-stu-id="0f1fa-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0f1fa-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0f1fa-139">JSON Representation</span></span>
<span data-ttu-id="0f1fa-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0f1fa-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





