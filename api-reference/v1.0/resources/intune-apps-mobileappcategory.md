---
title: mobileAppCategory リソースの種類
description: Intune のアプリの単一カテゴリのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b87ef1bbfff84a19c939fa1eb5d9371b2732ac46
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982023"
---
# <a name="mobileappcategory-resource-type"></a><span data-ttu-id="26d19-103">mobileAppCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="26d19-103">mobileAppCategory resource type</span></span>

> <span data-ttu-id="26d19-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="26d19-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26d19-105">Intune のアプリの単一カテゴリのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="26d19-105">Contains properties for a single Intune app category.</span></span>
## <a name="methods"></a><span data-ttu-id="26d19-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="26d19-106">Methods</span></span>
|<span data-ttu-id="26d19-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="26d19-107">Method</span></span>|<span data-ttu-id="26d19-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="26d19-108">Return Type</span></span>|<span data-ttu-id="26d19-109">説明</span><span class="sxs-lookup"><span data-stu-id="26d19-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="26d19-110">mobileAppCategories のリスト</span><span class="sxs-lookup"><span data-stu-id="26d19-110">List mobileAppCategories</span></span>](../api/intune-apps-mobileappcategory-list.md)|<span data-ttu-id="26d19-111">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="26d19-111">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="26d19-112">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="26d19-112">List properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects.</span></span>|
|[<span data-ttu-id="26d19-113">mobileAppCategory の取得</span><span class="sxs-lookup"><span data-stu-id="26d19-113">Get mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-get.md)|[<span data-ttu-id="26d19-114">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="26d19-114">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="26d19-115">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="26d19-115">Read properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|
|[<span data-ttu-id="26d19-116">mobileAppCategory の作成</span><span class="sxs-lookup"><span data-stu-id="26d19-116">Create mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-create.md)|[<span data-ttu-id="26d19-117">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="26d19-117">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="26d19-118">新しい [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="26d19-118">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|
|[<span data-ttu-id="26d19-119">mobileAppCategory の削除</span><span class="sxs-lookup"><span data-stu-id="26d19-119">Delete mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-delete.md)|<span data-ttu-id="26d19-120">なし</span><span class="sxs-lookup"><span data-stu-id="26d19-120">None</span></span>|<span data-ttu-id="26d19-121">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="26d19-121">Deletes a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>|
|[<span data-ttu-id="26d19-122">mobileAppCategory の更新</span><span class="sxs-lookup"><span data-stu-id="26d19-122">Update mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-update.md)|[<span data-ttu-id="26d19-123">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="26d19-123">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="26d19-124">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="26d19-124">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="26d19-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26d19-125">Properties</span></span>
|<span data-ttu-id="26d19-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26d19-126">Property</span></span>|<span data-ttu-id="26d19-127">型</span><span class="sxs-lookup"><span data-stu-id="26d19-127">Type</span></span>|<span data-ttu-id="26d19-128">説明</span><span class="sxs-lookup"><span data-stu-id="26d19-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26d19-129">ID</span><span class="sxs-lookup"><span data-stu-id="26d19-129">id</span></span>|<span data-ttu-id="26d19-130">String</span><span class="sxs-lookup"><span data-stu-id="26d19-130">String</span></span>|<span data-ttu-id="26d19-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="26d19-131">The key of the entity.</span></span>|
|<span data-ttu-id="26d19-132">displayName</span><span class="sxs-lookup"><span data-stu-id="26d19-132">displayName</span></span>|<span data-ttu-id="26d19-133">String</span><span class="sxs-lookup"><span data-stu-id="26d19-133">String</span></span>|<span data-ttu-id="26d19-134">アプリのカテゴリの名前。</span><span class="sxs-lookup"><span data-stu-id="26d19-134">The name of the app category.</span></span>|
|<span data-ttu-id="26d19-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26d19-135">lastModifiedDateTime</span></span>|<span data-ttu-id="26d19-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26d19-136">DateTimeOffset</span></span>|<span data-ttu-id="26d19-137">mobileAppCategory が最後に変更された日時です。</span><span class="sxs-lookup"><span data-stu-id="26d19-137">The date and time the mobileAppCategory was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26d19-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="26d19-138">Relationships</span></span>
<span data-ttu-id="26d19-139">なし</span><span class="sxs-lookup"><span data-stu-id="26d19-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="26d19-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="26d19-140">JSON Representation</span></span>
<span data-ttu-id="26d19-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="26d19-141">Here is a JSON representation of the resource.</span></span>
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



