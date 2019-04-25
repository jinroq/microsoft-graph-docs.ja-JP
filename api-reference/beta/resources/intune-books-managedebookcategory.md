---
title: managedebookcategory リソースの種類
description: 単一の Intune 電子ブックカテゴリのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef3d0d621394af0cfe949031d79ff374ba0491b8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548293"
---
# <a name="managedebookcategory-resource-type"></a><span data-ttu-id="1da3f-103">managedebookcategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1da3f-103">managedEBookCategory resource type</span></span>

> <span data-ttu-id="1da3f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1da3f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1da3f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1da3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1da3f-106">単一の Intune 電子ブックカテゴリのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1da3f-106">Contains properties for a single Intune eBook category.</span></span>

## <a name="methods"></a><span data-ttu-id="1da3f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="1da3f-107">Methods</span></span>
|<span data-ttu-id="1da3f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1da3f-108">Method</span></span>|<span data-ttu-id="1da3f-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1da3f-109">Return Type</span></span>|<span data-ttu-id="1da3f-110">説明</span><span class="sxs-lookup"><span data-stu-id="1da3f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1da3f-111">managedebookcategories のリスト</span><span class="sxs-lookup"><span data-stu-id="1da3f-111">List managedEBookCategories</span></span>](../api/intune-books-managedebookcategory-list.md)|<span data-ttu-id="1da3f-112">[managedebookcategory](../resources/intune-books-managedebookcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1da3f-112">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="1da3f-113">[managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1da3f-113">List properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) objects.</span></span>|
|[<span data-ttu-id="1da3f-114">managedebookcategory の取得</span><span class="sxs-lookup"><span data-stu-id="1da3f-114">Get managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-get.md)|[<span data-ttu-id="1da3f-115">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="1da3f-115">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="1da3f-116">[managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1da3f-116">Read properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="1da3f-117">managedebookcategory の作成</span><span class="sxs-lookup"><span data-stu-id="1da3f-117">Create managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-create.md)|[<span data-ttu-id="1da3f-118">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="1da3f-118">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="1da3f-119">新しい[managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1da3f-119">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="1da3f-120">managedebookcategory の削除</span><span class="sxs-lookup"><span data-stu-id="1da3f-120">Delete managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-delete.md)|<span data-ttu-id="1da3f-121">なし</span><span class="sxs-lookup"><span data-stu-id="1da3f-121">None</span></span>|<span data-ttu-id="1da3f-122">[managedebookcategory](../resources/intune-books-managedebookcategory.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="1da3f-122">Deletes a [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>|
|[<span data-ttu-id="1da3f-123">managedebookcategory の更新</span><span class="sxs-lookup"><span data-stu-id="1da3f-123">Update managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-update.md)|[<span data-ttu-id="1da3f-124">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="1da3f-124">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="1da3f-125">[managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1da3f-125">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1da3f-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1da3f-126">Properties</span></span>
|<span data-ttu-id="1da3f-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1da3f-127">Property</span></span>|<span data-ttu-id="1da3f-128">型</span><span class="sxs-lookup"><span data-stu-id="1da3f-128">Type</span></span>|<span data-ttu-id="1da3f-129">説明</span><span class="sxs-lookup"><span data-stu-id="1da3f-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1da3f-130">id</span><span class="sxs-lookup"><span data-stu-id="1da3f-130">id</span></span>|<span data-ttu-id="1da3f-131">String</span><span class="sxs-lookup"><span data-stu-id="1da3f-131">String</span></span>|<span data-ttu-id="1da3f-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1da3f-132">The key of the entity.</span></span>|
|<span data-ttu-id="1da3f-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1da3f-133">displayName</span></span>|<span data-ttu-id="1da3f-134">String</span><span class="sxs-lookup"><span data-stu-id="1da3f-134">String</span></span>|<span data-ttu-id="1da3f-135">eBook カテゴリの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="1da3f-135">The name of the eBook category.</span></span>|
|<span data-ttu-id="1da3f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1da3f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1da3f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1da3f-137">DateTimeOffset</span></span>|<span data-ttu-id="1da3f-138">managedebookcategory が最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="1da3f-138">The date and time the ManagedEBookCategory was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1da3f-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1da3f-139">Relationships</span></span>
<span data-ttu-id="1da3f-140">なし</span><span class="sxs-lookup"><span data-stu-id="1da3f-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1da3f-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1da3f-141">JSON Representation</span></span>
<span data-ttu-id="1da3f-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1da3f-142">Here is a JSON representation of the resource.</span></span>
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





