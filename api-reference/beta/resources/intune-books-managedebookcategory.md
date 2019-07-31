---
title: managedEBookCategory リソースの種類
description: 単一の Intune 電子ブックカテゴリのプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eda8f89a905d01b2ae41bb68ec61ec917a8bc264
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004821"
---
# <a name="managedebookcategory-resource-type"></a><span data-ttu-id="bcc96-103">managedEBookCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bcc96-103">managedEBookCategory resource type</span></span>

> <span data-ttu-id="bcc96-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bcc96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcc96-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bcc96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcc96-106">単一の Intune 電子ブックカテゴリのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="bcc96-106">Contains properties for a single Intune eBook category.</span></span>

## <a name="methods"></a><span data-ttu-id="bcc96-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="bcc96-107">Methods</span></span>
|<span data-ttu-id="bcc96-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="bcc96-108">Method</span></span>|<span data-ttu-id="bcc96-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bcc96-109">Return Type</span></span>|<span data-ttu-id="bcc96-110">説明</span><span class="sxs-lookup"><span data-stu-id="bcc96-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bcc96-111">ManagedEBookCategories のリスト</span><span class="sxs-lookup"><span data-stu-id="bcc96-111">List managedEBookCategories</span></span>](../api/intune-books-managedebookcategory-list.md)|<span data-ttu-id="bcc96-112">[Managedebookcategory](../resources/intune-books-managedebookcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bcc96-112">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="bcc96-113">[Managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="bcc96-113">List properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) objects.</span></span>|
|[<span data-ttu-id="bcc96-114">ManagedEBookCategory の取得</span><span class="sxs-lookup"><span data-stu-id="bcc96-114">Get managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-get.md)|[<span data-ttu-id="bcc96-115">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="bcc96-115">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="bcc96-116">[Managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bcc96-116">Read properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="bcc96-117">ManagedEBookCategory の作成</span><span class="sxs-lookup"><span data-stu-id="bcc96-117">Create managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-create.md)|[<span data-ttu-id="bcc96-118">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="bcc96-118">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="bcc96-119">新しい[Managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bcc96-119">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="bcc96-120">ManagedEBookCategory の削除</span><span class="sxs-lookup"><span data-stu-id="bcc96-120">Delete managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-delete.md)|<span data-ttu-id="bcc96-121">None</span><span class="sxs-lookup"><span data-stu-id="bcc96-121">None</span></span>|<span data-ttu-id="bcc96-122">[Managedebookcategory](../resources/intune-books-managedebookcategory.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="bcc96-122">Deletes a [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>|
|[<span data-ttu-id="bcc96-123">ManagedEBookCategory の更新</span><span class="sxs-lookup"><span data-stu-id="bcc96-123">Update managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-update.md)|[<span data-ttu-id="bcc96-124">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="bcc96-124">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="bcc96-125">[Managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bcc96-125">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bcc96-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bcc96-126">Properties</span></span>
|<span data-ttu-id="bcc96-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bcc96-127">Property</span></span>|<span data-ttu-id="bcc96-128">型</span><span class="sxs-lookup"><span data-stu-id="bcc96-128">Type</span></span>|<span data-ttu-id="bcc96-129">説明</span><span class="sxs-lookup"><span data-stu-id="bcc96-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcc96-130">id</span><span class="sxs-lookup"><span data-stu-id="bcc96-130">id</span></span>|<span data-ttu-id="bcc96-131">文字列</span><span class="sxs-lookup"><span data-stu-id="bcc96-131">String</span></span>|<span data-ttu-id="bcc96-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="bcc96-132">The key of the entity.</span></span>|
|<span data-ttu-id="bcc96-133">displayName</span><span class="sxs-lookup"><span data-stu-id="bcc96-133">displayName</span></span>|<span data-ttu-id="bcc96-134">String</span><span class="sxs-lookup"><span data-stu-id="bcc96-134">String</span></span>|<span data-ttu-id="bcc96-135">EBook カテゴリの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="bcc96-135">The name of the eBook category.</span></span>|
|<span data-ttu-id="bcc96-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bcc96-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bcc96-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcc96-137">DateTimeOffset</span></span>|<span data-ttu-id="bcc96-138">ManagedEBookCategory が最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="bcc96-138">The date and time the ManagedEBookCategory was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bcc96-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bcc96-139">Relationships</span></span>
<span data-ttu-id="bcc96-140">なし</span><span class="sxs-lookup"><span data-stu-id="bcc96-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bcc96-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bcc96-141">JSON Representation</span></span>
<span data-ttu-id="bcc96-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bcc96-142">Here is a JSON representation of the resource.</span></span>
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





