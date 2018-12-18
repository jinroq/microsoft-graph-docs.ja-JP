---
title: mobileAppCategory リソースの種類
description: Intune のアプリの単一カテゴリのプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: f40e9a24269d276c89d770acb0d772a7bdf94c51
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340762"
---
# <a name="mobileappcategory-resource-type"></a><span data-ttu-id="47059-103">mobileAppCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="47059-103">mobileAppCategory resource type</span></span>

> <span data-ttu-id="47059-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="47059-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47059-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47059-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47059-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="47059-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47059-107">Intune のアプリの単一カテゴリのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="47059-107">Contains properties for a single Intune app category.</span></span>
## <a name="methods"></a><span data-ttu-id="47059-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="47059-108">Methods</span></span>
|<span data-ttu-id="47059-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="47059-109">Method</span></span>|<span data-ttu-id="47059-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="47059-110">Return Type</span></span>|<span data-ttu-id="47059-111">説明</span><span class="sxs-lookup"><span data-stu-id="47059-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="47059-112">mobileAppCategories のリスト</span><span class="sxs-lookup"><span data-stu-id="47059-112">List mobileAppCategories</span></span>](../api/intune-apps-mobileappcategory-list.md)|<span data-ttu-id="47059-113">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="47059-113">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="47059-114">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="47059-114">List properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects.</span></span>|
|[<span data-ttu-id="47059-115">mobileAppCategory の取得</span><span class="sxs-lookup"><span data-stu-id="47059-115">Get mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-get.md)|[<span data-ttu-id="47059-116">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="47059-116">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="47059-117">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="47059-117">Read properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|
|[<span data-ttu-id="47059-118">mobileAppCategory の作成</span><span class="sxs-lookup"><span data-stu-id="47059-118">Create mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-create.md)|[<span data-ttu-id="47059-119">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="47059-119">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="47059-120">新しい [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="47059-120">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|
|[<span data-ttu-id="47059-121">mobileAppCategory の削除</span><span class="sxs-lookup"><span data-stu-id="47059-121">Delete mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-delete.md)|<span data-ttu-id="47059-122">なし</span><span class="sxs-lookup"><span data-stu-id="47059-122">None</span></span>|<span data-ttu-id="47059-123">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="47059-123">Deletes a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>|
|[<span data-ttu-id="47059-124">mobileAppCategory の更新</span><span class="sxs-lookup"><span data-stu-id="47059-124">Update mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-update.md)|[<span data-ttu-id="47059-125">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="47059-125">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="47059-126">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="47059-126">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="47059-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47059-127">Properties</span></span>
|<span data-ttu-id="47059-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47059-128">Property</span></span>|<span data-ttu-id="47059-129">種類</span><span class="sxs-lookup"><span data-stu-id="47059-129">Type</span></span>|<span data-ttu-id="47059-130">説明</span><span class="sxs-lookup"><span data-stu-id="47059-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47059-131">ID</span><span class="sxs-lookup"><span data-stu-id="47059-131">id</span></span>|<span data-ttu-id="47059-132">String</span><span class="sxs-lookup"><span data-stu-id="47059-132">String</span></span>|<span data-ttu-id="47059-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="47059-133">The key of the entity.</span></span>|
|<span data-ttu-id="47059-134">displayName</span><span class="sxs-lookup"><span data-stu-id="47059-134">displayName</span></span>|<span data-ttu-id="47059-135">String</span><span class="sxs-lookup"><span data-stu-id="47059-135">String</span></span>|<span data-ttu-id="47059-136">アプリのカテゴリの名前。</span><span class="sxs-lookup"><span data-stu-id="47059-136">The name of the app category.</span></span>|
|<span data-ttu-id="47059-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47059-137">lastModifiedDateTime</span></span>|<span data-ttu-id="47059-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47059-138">DateTimeOffset</span></span>|<span data-ttu-id="47059-139">mobileAppCategory が最後に変更された日時です。</span><span class="sxs-lookup"><span data-stu-id="47059-139">The date and time the mobileAppCategory was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47059-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="47059-140">Relationships</span></span>
<span data-ttu-id="47059-141">なし</span><span class="sxs-lookup"><span data-stu-id="47059-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="47059-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="47059-142">JSON Representation</span></span>
<span data-ttu-id="47059-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="47059-143">Here is a JSON representation of the resource.</span></span>
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





