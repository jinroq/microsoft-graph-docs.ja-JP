---
title: managedebookcategory リソースの種類
description: 単一の Intune 電子ブックカテゴリのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef3d0d621394af0cfe949031d79ff374ba0491b8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795871"
---
# <a name="managedebookcategory-resource-type"></a><span data-ttu-id="4028d-103">managedebookcategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4028d-103">managedEBookCategory resource type</span></span>

> <span data-ttu-id="4028d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4028d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4028d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4028d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4028d-106">単一の Intune 電子ブックカテゴリのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4028d-106">Contains properties for a single Intune eBook category.</span></span>

## <a name="methods"></a><span data-ttu-id="4028d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4028d-107">Methods</span></span>
|<span data-ttu-id="4028d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4028d-108">Method</span></span>|<span data-ttu-id="4028d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4028d-109">Return Type</span></span>|<span data-ttu-id="4028d-110">説明</span><span class="sxs-lookup"><span data-stu-id="4028d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4028d-111">managedebookcategories のリスト</span><span class="sxs-lookup"><span data-stu-id="4028d-111">List managedEBookCategories</span></span>](../api/intune-books-managedebookcategory-list.md)|<span data-ttu-id="4028d-112">[managedebookcategory](../resources/intune-books-managedebookcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4028d-112">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="4028d-113">[managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="4028d-113">List properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) objects.</span></span>|
|[<span data-ttu-id="4028d-114">managedebookcategory の取得</span><span class="sxs-lookup"><span data-stu-id="4028d-114">Get managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-get.md)|[<span data-ttu-id="4028d-115">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="4028d-115">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="4028d-116">[managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4028d-116">Read properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="4028d-117">managedebookcategory の作成</span><span class="sxs-lookup"><span data-stu-id="4028d-117">Create managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-create.md)|[<span data-ttu-id="4028d-118">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="4028d-118">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="4028d-119">新しい[managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4028d-119">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="4028d-120">managedebookcategory の削除</span><span class="sxs-lookup"><span data-stu-id="4028d-120">Delete managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-delete.md)|<span data-ttu-id="4028d-121">なし</span><span class="sxs-lookup"><span data-stu-id="4028d-121">None</span></span>|<span data-ttu-id="4028d-122">[managedebookcategory](../resources/intune-books-managedebookcategory.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="4028d-122">Deletes a [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>|
|[<span data-ttu-id="4028d-123">managedebookcategory の更新</span><span class="sxs-lookup"><span data-stu-id="4028d-123">Update managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-update.md)|[<span data-ttu-id="4028d-124">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="4028d-124">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="4028d-125">[managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4028d-125">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4028d-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4028d-126">Properties</span></span>
|<span data-ttu-id="4028d-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4028d-127">Property</span></span>|<span data-ttu-id="4028d-128">型</span><span class="sxs-lookup"><span data-stu-id="4028d-128">Type</span></span>|<span data-ttu-id="4028d-129">説明</span><span class="sxs-lookup"><span data-stu-id="4028d-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4028d-130">id</span><span class="sxs-lookup"><span data-stu-id="4028d-130">id</span></span>|<span data-ttu-id="4028d-131">String</span><span class="sxs-lookup"><span data-stu-id="4028d-131">String</span></span>|<span data-ttu-id="4028d-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4028d-132">The key of the entity.</span></span>|
|<span data-ttu-id="4028d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="4028d-133">displayName</span></span>|<span data-ttu-id="4028d-134">String</span><span class="sxs-lookup"><span data-stu-id="4028d-134">String</span></span>|<span data-ttu-id="4028d-135">eBook カテゴリの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="4028d-135">The name of the eBook category.</span></span>|
|<span data-ttu-id="4028d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4028d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4028d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4028d-137">DateTimeOffset</span></span>|<span data-ttu-id="4028d-138">managedebookcategory が最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="4028d-138">The date and time the ManagedEBookCategory was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4028d-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4028d-139">Relationships</span></span>
<span data-ttu-id="4028d-140">なし</span><span class="sxs-lookup"><span data-stu-id="4028d-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4028d-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4028d-141">JSON Representation</span></span>
<span data-ttu-id="4028d-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4028d-142">Here is a JSON representation of the resource.</span></span>
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





