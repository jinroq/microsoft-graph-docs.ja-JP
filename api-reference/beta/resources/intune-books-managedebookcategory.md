---
title: managedEBookCategory リソースの種類
description: 単一の Intune 電子ブックカテゴリのプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ad1f8c2d4c680ef3594d29a11eb15edcb708b77a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335103"
---
# <a name="managedebookcategory-resource-type"></a><span data-ttu-id="15e38-103">managedEBookCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="15e38-103">managedEBookCategory resource type</span></span>

> <span data-ttu-id="15e38-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15e38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15e38-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="15e38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15e38-106">単一の Intune 電子ブックカテゴリのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="15e38-106">Contains properties for a single Intune eBook category.</span></span>

## <a name="methods"></a><span data-ttu-id="15e38-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="15e38-107">Methods</span></span>
|<span data-ttu-id="15e38-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="15e38-108">Method</span></span>|<span data-ttu-id="15e38-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="15e38-109">Return Type</span></span>|<span data-ttu-id="15e38-110">説明</span><span class="sxs-lookup"><span data-stu-id="15e38-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="15e38-111">ManagedEBookCategories のリスト</span><span class="sxs-lookup"><span data-stu-id="15e38-111">List managedEBookCategories</span></span>](../api/intune-books-managedebookcategory-list.md)|<span data-ttu-id="15e38-112">[Managedebookcategory](../resources/intune-books-managedebookcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="15e38-112">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="15e38-113">[Managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="15e38-113">List properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) objects.</span></span>|
|[<span data-ttu-id="15e38-114">ManagedEBookCategory の取得</span><span class="sxs-lookup"><span data-stu-id="15e38-114">Get managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-get.md)|[<span data-ttu-id="15e38-115">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="15e38-115">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="15e38-116">[Managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="15e38-116">Read properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="15e38-117">ManagedEBookCategory の作成</span><span class="sxs-lookup"><span data-stu-id="15e38-117">Create managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-create.md)|[<span data-ttu-id="15e38-118">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="15e38-118">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="15e38-119">新しい[Managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="15e38-119">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="15e38-120">ManagedEBookCategory の削除</span><span class="sxs-lookup"><span data-stu-id="15e38-120">Delete managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-delete.md)|<span data-ttu-id="15e38-121">None</span><span class="sxs-lookup"><span data-stu-id="15e38-121">None</span></span>|<span data-ttu-id="15e38-122">[Managedebookcategory](../resources/intune-books-managedebookcategory.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="15e38-122">Deletes a [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>|
|[<span data-ttu-id="15e38-123">ManagedEBookCategory の更新</span><span class="sxs-lookup"><span data-stu-id="15e38-123">Update managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-update.md)|[<span data-ttu-id="15e38-124">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="15e38-124">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="15e38-125">[Managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="15e38-125">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="15e38-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15e38-126">Properties</span></span>
|<span data-ttu-id="15e38-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15e38-127">Property</span></span>|<span data-ttu-id="15e38-128">型</span><span class="sxs-lookup"><span data-stu-id="15e38-128">Type</span></span>|<span data-ttu-id="15e38-129">説明</span><span class="sxs-lookup"><span data-stu-id="15e38-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15e38-130">id</span><span class="sxs-lookup"><span data-stu-id="15e38-130">id</span></span>|<span data-ttu-id="15e38-131">文字列</span><span class="sxs-lookup"><span data-stu-id="15e38-131">String</span></span>|<span data-ttu-id="15e38-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="15e38-132">The key of the entity.</span></span>|
|<span data-ttu-id="15e38-133">displayName</span><span class="sxs-lookup"><span data-stu-id="15e38-133">displayName</span></span>|<span data-ttu-id="15e38-134">String</span><span class="sxs-lookup"><span data-stu-id="15e38-134">String</span></span>|<span data-ttu-id="15e38-135">EBook カテゴリの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="15e38-135">The name of the eBook category.</span></span>|
|<span data-ttu-id="15e38-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15e38-136">lastModifiedDateTime</span></span>|<span data-ttu-id="15e38-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15e38-137">DateTimeOffset</span></span>|<span data-ttu-id="15e38-138">ManagedEBookCategory が最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="15e38-138">The date and time the ManagedEBookCategory was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15e38-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="15e38-139">Relationships</span></span>
<span data-ttu-id="15e38-140">なし</span><span class="sxs-lookup"><span data-stu-id="15e38-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15e38-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="15e38-141">JSON Representation</span></span>
<span data-ttu-id="15e38-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="15e38-142">Here is a JSON representation of the resource.</span></span>
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



