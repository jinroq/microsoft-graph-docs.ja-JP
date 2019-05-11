---
title: mobileAppCategory リソースの種類
description: Intune のアプリの単一カテゴリのプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee6a4d90d72a7df79a19ba353448dc700ed00f68
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949977"
---
# <a name="mobileappcategory-resource-type"></a><span data-ttu-id="d61b3-103">mobileAppCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d61b3-103">mobileAppCategory resource type</span></span>

> <span data-ttu-id="d61b3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d61b3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d61b3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d61b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d61b3-106">Intune のアプリの単一カテゴリのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d61b3-106">Contains properties for a single Intune app category.</span></span>

## <a name="methods"></a><span data-ttu-id="d61b3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d61b3-107">Methods</span></span>
|<span data-ttu-id="d61b3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d61b3-108">Method</span></span>|<span data-ttu-id="d61b3-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d61b3-109">Return Type</span></span>|<span data-ttu-id="d61b3-110">説明</span><span class="sxs-lookup"><span data-stu-id="d61b3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d61b3-111">mobileAppCategories のリスト</span><span class="sxs-lookup"><span data-stu-id="d61b3-111">List mobileAppCategories</span></span>](../api/intune-apps-mobileappcategory-list.md)|<span data-ttu-id="d61b3-112">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d61b3-112">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="d61b3-113">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d61b3-113">List properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects.</span></span>|
|[<span data-ttu-id="d61b3-114">mobileAppCategory の取得</span><span class="sxs-lookup"><span data-stu-id="d61b3-114">Get mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-get.md)|[<span data-ttu-id="d61b3-115">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="d61b3-115">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="d61b3-116">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d61b3-116">Read properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|
|[<span data-ttu-id="d61b3-117">mobileAppCategory の作成</span><span class="sxs-lookup"><span data-stu-id="d61b3-117">Create mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-create.md)|[<span data-ttu-id="d61b3-118">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="d61b3-118">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="d61b3-119">新しい [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d61b3-119">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|
|[<span data-ttu-id="d61b3-120">mobileAppCategory の削除</span><span class="sxs-lookup"><span data-stu-id="d61b3-120">Delete mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-delete.md)|<span data-ttu-id="d61b3-121">なし</span><span class="sxs-lookup"><span data-stu-id="d61b3-121">None</span></span>|<span data-ttu-id="d61b3-122">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="d61b3-122">Deletes a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>|
|[<span data-ttu-id="d61b3-123">mobileAppCategory の更新</span><span class="sxs-lookup"><span data-stu-id="d61b3-123">Update mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-update.md)|[<span data-ttu-id="d61b3-124">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="d61b3-124">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="d61b3-125">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d61b3-125">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d61b3-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d61b3-126">Properties</span></span>
|<span data-ttu-id="d61b3-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d61b3-127">Property</span></span>|<span data-ttu-id="d61b3-128">型</span><span class="sxs-lookup"><span data-stu-id="d61b3-128">Type</span></span>|<span data-ttu-id="d61b3-129">説明</span><span class="sxs-lookup"><span data-stu-id="d61b3-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d61b3-130">id</span><span class="sxs-lookup"><span data-stu-id="d61b3-130">id</span></span>|<span data-ttu-id="d61b3-131">文字列</span><span class="sxs-lookup"><span data-stu-id="d61b3-131">String</span></span>|<span data-ttu-id="d61b3-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d61b3-132">The key of the entity.</span></span>|
|<span data-ttu-id="d61b3-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d61b3-133">displayName</span></span>|<span data-ttu-id="d61b3-134">String</span><span class="sxs-lookup"><span data-stu-id="d61b3-134">String</span></span>|<span data-ttu-id="d61b3-135">アプリのカテゴリの名前。</span><span class="sxs-lookup"><span data-stu-id="d61b3-135">The name of the app category.</span></span>|
|<span data-ttu-id="d61b3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d61b3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d61b3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d61b3-137">DateTimeOffset</span></span>|<span data-ttu-id="d61b3-138">mobileAppCategory が最後に変更された日時です。</span><span class="sxs-lookup"><span data-stu-id="d61b3-138">The date and time the mobileAppCategory was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d61b3-139">関係</span><span class="sxs-lookup"><span data-stu-id="d61b3-139">Relationships</span></span>
<span data-ttu-id="d61b3-140">なし</span><span class="sxs-lookup"><span data-stu-id="d61b3-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d61b3-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d61b3-141">JSON Representation</span></span>
<span data-ttu-id="d61b3-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d61b3-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```




