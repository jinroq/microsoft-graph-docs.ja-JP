---
title: managedEBookCategory リソースの種類
description: Intune eBook の分類項目を 1 つのプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: 5bc95696a9949fa4be2f58d39a18adf4875a9056
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356918"
---
# <a name="managedebookcategory-resource-type"></a><span data-ttu-id="10e7d-103">managedEBookCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="10e7d-103">managedEBookCategory resource type</span></span>

> <span data-ttu-id="10e7d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="10e7d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10e7d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="10e7d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10e7d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="10e7d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10e7d-107">Intune eBook の分類項目を 1 つのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="10e7d-107">Contains properties for a single Intune eBook category.</span></span>
## <a name="methods"></a><span data-ttu-id="10e7d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="10e7d-108">Methods</span></span>
|<span data-ttu-id="10e7d-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="10e7d-109">Method</span></span>|<span data-ttu-id="10e7d-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="10e7d-110">Return Type</span></span>|<span data-ttu-id="10e7d-111">説明</span><span class="sxs-lookup"><span data-stu-id="10e7d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="10e7d-112">リスト managedEBookCategories</span><span class="sxs-lookup"><span data-stu-id="10e7d-112">List managedEBookCategories</span></span>](../api/intune-books-managedebookcategory-list.md)|<span data-ttu-id="10e7d-113">[managedEBookCategory](../resources/intune-books-managedebookcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="10e7d-113">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="10e7d-114">[ManagedEBookCategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="10e7d-114">List properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) objects.</span></span>|
|[<span data-ttu-id="10e7d-115">ManagedEBookCategory を取得します。</span><span class="sxs-lookup"><span data-stu-id="10e7d-115">Get managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-get.md)|[<span data-ttu-id="10e7d-116">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="10e7d-116">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="10e7d-117">[ManagedEBookCategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="10e7d-117">Read properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="10e7d-118">ManagedEBookCategory を作成します。</span><span class="sxs-lookup"><span data-stu-id="10e7d-118">Create managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-create.md)|[<span data-ttu-id="10e7d-119">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="10e7d-119">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="10e7d-120">新しい[managedEBookCategory](../resources/intune-books-managedebookcategory.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="10e7d-120">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="10e7d-121">ManagedEBookCategory を削除します。</span><span class="sxs-lookup"><span data-stu-id="10e7d-121">Delete managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-delete.md)|<span data-ttu-id="10e7d-122">なし</span><span class="sxs-lookup"><span data-stu-id="10e7d-122">None</span></span>|<span data-ttu-id="10e7d-123">の[managedEBookCategory](../resources/intune-books-managedebookcategory.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="10e7d-123">Deletes a [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>|
|[<span data-ttu-id="10e7d-124">ManagedEBookCategory を更新します。</span><span class="sxs-lookup"><span data-stu-id="10e7d-124">Update managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-update.md)|[<span data-ttu-id="10e7d-125">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="10e7d-125">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="10e7d-126">[ManagedEBookCategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="10e7d-126">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="10e7d-127">Properties</span><span class="sxs-lookup"><span data-stu-id="10e7d-127">Properties</span></span>
|<span data-ttu-id="10e7d-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="10e7d-128">Property</span></span>|<span data-ttu-id="10e7d-129">種類</span><span class="sxs-lookup"><span data-stu-id="10e7d-129">Type</span></span>|<span data-ttu-id="10e7d-130">説明</span><span class="sxs-lookup"><span data-stu-id="10e7d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10e7d-131">ID</span><span class="sxs-lookup"><span data-stu-id="10e7d-131">id</span></span>|<span data-ttu-id="10e7d-132">String</span><span class="sxs-lookup"><span data-stu-id="10e7d-132">String</span></span>|<span data-ttu-id="10e7d-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="10e7d-133">The key of the entity.</span></span>|
|<span data-ttu-id="10e7d-134">displayName</span><span class="sxs-lookup"><span data-stu-id="10e7d-134">displayName</span></span>|<span data-ttu-id="10e7d-135">String</span><span class="sxs-lookup"><span data-stu-id="10e7d-135">String</span></span>|<span data-ttu-id="10e7d-136">EBook カテゴリの名前です。</span><span class="sxs-lookup"><span data-stu-id="10e7d-136">The name of the eBook category.</span></span>|
|<span data-ttu-id="10e7d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10e7d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="10e7d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10e7d-138">DateTimeOffset</span></span>|<span data-ttu-id="10e7d-139">日付と時刻、ManagedEBookCategory が最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="10e7d-139">The date and time the ManagedEBookCategory was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10e7d-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="10e7d-140">Relationships</span></span>
<span data-ttu-id="10e7d-141">なし</span><span class="sxs-lookup"><span data-stu-id="10e7d-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="10e7d-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="10e7d-142">JSON Representation</span></span>
<span data-ttu-id="10e7d-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="10e7d-143">Here is a JSON representation of the resource.</span></span>
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




