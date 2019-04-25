---
title: deviceManagementBooleanSettingInstance リソースの種類
description: ブール値を表す設定インスタンス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ff746cc368ba3048075ce795f514709ad2866bee
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523547"
---
# <a name="devicemanagementbooleansettinginstance-resource-type"></a><span data-ttu-id="d6ea2-103">deviceManagementBooleanSettingInstance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d6ea2-103">deviceManagementBooleanSettingInstance resource type</span></span>

> <span data-ttu-id="d6ea2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6ea2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6ea2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d6ea2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6ea2-106">ブール値を表す設定インスタンス</span><span class="sxs-lookup"><span data-stu-id="d6ea2-106">A setting instance representing a boolean value</span></span>


<span data-ttu-id="d6ea2-107">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="d6ea2-107">Inherits from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d6ea2-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d6ea2-108">Methods</span></span>
|<span data-ttu-id="d6ea2-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d6ea2-109">Method</span></span>|<span data-ttu-id="d6ea2-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d6ea2-110">Return Type</span></span>|<span data-ttu-id="d6ea2-111">説明</span><span class="sxs-lookup"><span data-stu-id="d6ea2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d6ea2-112">リスト deviceManagementBooleanSettingInstances</span><span class="sxs-lookup"><span data-stu-id="d6ea2-112">List deviceManagementBooleanSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementbooleansettinginstance-list.md)|<span data-ttu-id="d6ea2-113">[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d6ea2-113">[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) collection</span></span>|<span data-ttu-id="d6ea2-114">[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d6ea2-114">List properties and relationships of the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="d6ea2-115">deviceManagementBooleanSettingInstance を取得する</span><span class="sxs-lookup"><span data-stu-id="d6ea2-115">Get deviceManagementBooleanSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementbooleansettinginstance-get.md)|[<span data-ttu-id="d6ea2-116">deviceManagementBooleanSettingInstance</span><span class="sxs-lookup"><span data-stu-id="d6ea2-116">deviceManagementBooleanSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|<span data-ttu-id="d6ea2-117">[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d6ea2-117">Read properties and relationships of the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>|
|[<span data-ttu-id="d6ea2-118">deviceManagementBooleanSettingInstance を作成する</span><span class="sxs-lookup"><span data-stu-id="d6ea2-118">Create deviceManagementBooleanSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementbooleansettinginstance-create.md)|[<span data-ttu-id="d6ea2-119">deviceManagementBooleanSettingInstance</span><span class="sxs-lookup"><span data-stu-id="d6ea2-119">deviceManagementBooleanSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|<span data-ttu-id="d6ea2-120">新しい[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d6ea2-120">Create a new [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>|
|[<span data-ttu-id="d6ea2-121">deviceManagementBooleanSettingInstance の削除</span><span class="sxs-lookup"><span data-stu-id="d6ea2-121">Delete deviceManagementBooleanSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementbooleansettinginstance-delete.md)|<span data-ttu-id="d6ea2-122">なし</span><span class="sxs-lookup"><span data-stu-id="d6ea2-122">None</span></span>|<span data-ttu-id="d6ea2-123">[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="d6ea2-123">Deletes a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md).</span></span>|
|[<span data-ttu-id="d6ea2-124">deviceManagementBooleanSettingInstance の更新</span><span class="sxs-lookup"><span data-stu-id="d6ea2-124">Update deviceManagementBooleanSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementbooleansettinginstance-update.md)|[<span data-ttu-id="d6ea2-125">deviceManagementBooleanSettingInstance</span><span class="sxs-lookup"><span data-stu-id="d6ea2-125">deviceManagementBooleanSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|<span data-ttu-id="d6ea2-126">[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d6ea2-126">Update the properties of a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d6ea2-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6ea2-127">Properties</span></span>
|<span data-ttu-id="d6ea2-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6ea2-128">Property</span></span>|<span data-ttu-id="d6ea2-129">型</span><span class="sxs-lookup"><span data-stu-id="d6ea2-129">Type</span></span>|<span data-ttu-id="d6ea2-130">説明</span><span class="sxs-lookup"><span data-stu-id="d6ea2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6ea2-131">id</span><span class="sxs-lookup"><span data-stu-id="d6ea2-131">id</span></span>|<span data-ttu-id="d6ea2-132">String</span><span class="sxs-lookup"><span data-stu-id="d6ea2-132">String</span></span>|<span data-ttu-id="d6ea2-133">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された設定インスタンス ID</span><span class="sxs-lookup"><span data-stu-id="d6ea2-133">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="d6ea2-134">definitionId</span><span class="sxs-lookup"><span data-stu-id="d6ea2-134">definitionId</span></span>|<span data-ttu-id="d6ea2-135">String</span><span class="sxs-lookup"><span data-stu-id="d6ea2-135">String</span></span>|<span data-ttu-id="d6ea2-136">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承されたこのインスタンスの設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="d6ea2-136">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="d6ea2-137">valuejson</span><span class="sxs-lookup"><span data-stu-id="d6ea2-137">valueJson</span></span>|<span data-ttu-id="d6ea2-138">String</span><span class="sxs-lookup"><span data-stu-id="d6ea2-138">String</span></span>|<span data-ttu-id="d6ea2-139">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された値の JSON 表現</span><span class="sxs-lookup"><span data-stu-id="d6ea2-139">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="d6ea2-140">value</span><span class="sxs-lookup"><span data-stu-id="d6ea2-140">value</span></span>|<span data-ttu-id="d6ea2-141">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="d6ea2-141">Boolean</span></span>|<span data-ttu-id="d6ea2-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="d6ea2-142">The boolean value</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6ea2-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d6ea2-143">Relationships</span></span>
<span data-ttu-id="d6ea2-144">なし</span><span class="sxs-lookup"><span data-stu-id="d6ea2-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6ea2-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d6ea2-145">JSON Representation</span></span>
<span data-ttu-id="d6ea2-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d6ea2-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementBooleanSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "value": true
}
```





