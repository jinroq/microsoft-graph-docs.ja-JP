---
title: mobileAppCategory リソースの種類
description: Intune のアプリの単一カテゴリのプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 59f840bdd3a01ca8f8614f6e14e53d9ba95005dc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422265"
---
# <a name="mobileappcategory-resource-type"></a><span data-ttu-id="2332c-103">mobileAppCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2332c-103">mobileAppCategory resource type</span></span>

> <span data-ttu-id="2332c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2332c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2332c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2332c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2332c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2332c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2332c-107">Intune のアプリの単一カテゴリのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2332c-107">Contains properties for a single Intune app category.</span></span>

## <a name="methods"></a><span data-ttu-id="2332c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="2332c-108">Methods</span></span>
|<span data-ttu-id="2332c-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="2332c-109">Method</span></span>|<span data-ttu-id="2332c-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2332c-110">Return Type</span></span>|<span data-ttu-id="2332c-111">説明</span><span class="sxs-lookup"><span data-stu-id="2332c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2332c-112">mobileAppCategories のリスト</span><span class="sxs-lookup"><span data-stu-id="2332c-112">List mobileAppCategories</span></span>](../api/intune-apps-mobileappcategory-list.md)|<span data-ttu-id="2332c-113">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2332c-113">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="2332c-114">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2332c-114">List properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects.</span></span>|
|[<span data-ttu-id="2332c-115">mobileAppCategory の取得</span><span class="sxs-lookup"><span data-stu-id="2332c-115">Get mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-get.md)|[<span data-ttu-id="2332c-116">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="2332c-116">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="2332c-117">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2332c-117">Read properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|
|[<span data-ttu-id="2332c-118">mobileAppCategory の作成</span><span class="sxs-lookup"><span data-stu-id="2332c-118">Create mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-create.md)|[<span data-ttu-id="2332c-119">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="2332c-119">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="2332c-120">新しい [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2332c-120">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|
|[<span data-ttu-id="2332c-121">mobileAppCategory の削除</span><span class="sxs-lookup"><span data-stu-id="2332c-121">Delete mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-delete.md)|<span data-ttu-id="2332c-122">なし</span><span class="sxs-lookup"><span data-stu-id="2332c-122">None</span></span>|<span data-ttu-id="2332c-123">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="2332c-123">Deletes a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>|
|[<span data-ttu-id="2332c-124">mobileAppCategory の更新</span><span class="sxs-lookup"><span data-stu-id="2332c-124">Update mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-update.md)|[<span data-ttu-id="2332c-125">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="2332c-125">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="2332c-126">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2332c-126">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2332c-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2332c-127">Properties</span></span>
|<span data-ttu-id="2332c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2332c-128">Property</span></span>|<span data-ttu-id="2332c-129">型</span><span class="sxs-lookup"><span data-stu-id="2332c-129">Type</span></span>|<span data-ttu-id="2332c-130">説明</span><span class="sxs-lookup"><span data-stu-id="2332c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2332c-131">id</span><span class="sxs-lookup"><span data-stu-id="2332c-131">id</span></span>|<span data-ttu-id="2332c-132">String</span><span class="sxs-lookup"><span data-stu-id="2332c-132">String</span></span>|<span data-ttu-id="2332c-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2332c-133">The key of the entity.</span></span>|
|<span data-ttu-id="2332c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="2332c-134">displayName</span></span>|<span data-ttu-id="2332c-135">String</span><span class="sxs-lookup"><span data-stu-id="2332c-135">String</span></span>|<span data-ttu-id="2332c-136">アプリのカテゴリの名前。</span><span class="sxs-lookup"><span data-stu-id="2332c-136">The name of the app category.</span></span>|
|<span data-ttu-id="2332c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2332c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2332c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2332c-138">DateTimeOffset</span></span>|<span data-ttu-id="2332c-139">mobileAppCategory が最後に変更された日時です。</span><span class="sxs-lookup"><span data-stu-id="2332c-139">The date and time the mobileAppCategory was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2332c-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2332c-140">Relationships</span></span>
<span data-ttu-id="2332c-141">なし</span><span class="sxs-lookup"><span data-stu-id="2332c-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2332c-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2332c-142">JSON Representation</span></span>
<span data-ttu-id="2332c-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2332c-143">Here is a JSON representation of the resource.</span></span>
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




