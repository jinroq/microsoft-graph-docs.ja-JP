---
title: managedebookcategory リソースの種類
description: 単一の Intune 電子ブックカテゴリのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cb96477944edad4e2ca85020aa273e6718f8cdc2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152453"
---
# <a name="managedebookcategory-resource-type"></a><span data-ttu-id="85ad2-103">managedebookcategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="85ad2-103">managedEBookCategory resource type</span></span>

> <span data-ttu-id="85ad2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85ad2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85ad2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="85ad2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85ad2-106">単一の Intune 電子ブックカテゴリのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="85ad2-106">Contains properties for a single Intune eBook category.</span></span>

## <a name="methods"></a><span data-ttu-id="85ad2-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="85ad2-107">Methods</span></span>
|<span data-ttu-id="85ad2-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="85ad2-108">Method</span></span>|<span data-ttu-id="85ad2-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="85ad2-109">Return Type</span></span>|<span data-ttu-id="85ad2-110">説明</span><span class="sxs-lookup"><span data-stu-id="85ad2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="85ad2-111">managedebookcategories のリスト</span><span class="sxs-lookup"><span data-stu-id="85ad2-111">List managedEBookCategories</span></span>](../api/intune-books-managedebookcategory-list.md)|<span data-ttu-id="85ad2-112">[managedebookcategory](../resources/intune-books-managedebookcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="85ad2-112">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="85ad2-113">[managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="85ad2-113">List properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) objects.</span></span>|
|[<span data-ttu-id="85ad2-114">managedebookcategory の取得</span><span class="sxs-lookup"><span data-stu-id="85ad2-114">Get managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-get.md)|[<span data-ttu-id="85ad2-115">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="85ad2-115">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="85ad2-116">[managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="85ad2-116">Read properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="85ad2-117">managedebookcategory の作成</span><span class="sxs-lookup"><span data-stu-id="85ad2-117">Create managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-create.md)|[<span data-ttu-id="85ad2-118">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="85ad2-118">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="85ad2-119">新しい[managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="85ad2-119">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="85ad2-120">managedebookcategory の削除</span><span class="sxs-lookup"><span data-stu-id="85ad2-120">Delete managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-delete.md)|<span data-ttu-id="85ad2-121">なし</span><span class="sxs-lookup"><span data-stu-id="85ad2-121">None</span></span>|<span data-ttu-id="85ad2-122">[managedebookcategory](../resources/intune-books-managedebookcategory.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="85ad2-122">Deletes a [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>|
|[<span data-ttu-id="85ad2-123">managedebookcategory の更新</span><span class="sxs-lookup"><span data-stu-id="85ad2-123">Update managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-update.md)|[<span data-ttu-id="85ad2-124">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="85ad2-124">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="85ad2-125">[managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="85ad2-125">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="85ad2-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85ad2-126">Properties</span></span>
|<span data-ttu-id="85ad2-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85ad2-127">Property</span></span>|<span data-ttu-id="85ad2-128">型</span><span class="sxs-lookup"><span data-stu-id="85ad2-128">Type</span></span>|<span data-ttu-id="85ad2-129">説明</span><span class="sxs-lookup"><span data-stu-id="85ad2-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85ad2-130">id</span><span class="sxs-lookup"><span data-stu-id="85ad2-130">id</span></span>|<span data-ttu-id="85ad2-131">String</span><span class="sxs-lookup"><span data-stu-id="85ad2-131">String</span></span>|<span data-ttu-id="85ad2-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="85ad2-132">The key of the entity.</span></span>|
|<span data-ttu-id="85ad2-133">displayName</span><span class="sxs-lookup"><span data-stu-id="85ad2-133">displayName</span></span>|<span data-ttu-id="85ad2-134">String</span><span class="sxs-lookup"><span data-stu-id="85ad2-134">String</span></span>|<span data-ttu-id="85ad2-135">eBook カテゴリの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="85ad2-135">The name of the eBook category.</span></span>|
|<span data-ttu-id="85ad2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85ad2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="85ad2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85ad2-137">DateTimeOffset</span></span>|<span data-ttu-id="85ad2-138">managedebookcategory が最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="85ad2-138">The date and time the ManagedEBookCategory was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85ad2-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="85ad2-139">Relationships</span></span>
<span data-ttu-id="85ad2-140">なし</span><span class="sxs-lookup"><span data-stu-id="85ad2-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85ad2-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="85ad2-141">JSON Representation</span></span>
<span data-ttu-id="85ad2-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="85ad2-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```




