---
title: mobileAppContent リソースの種類
description: 特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。 各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9cde82585bdbe4ca4c15102e6b343810f29fdae8
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261300"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="b6132-104">mobileAppContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b6132-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="b6132-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b6132-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6132-106">特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b6132-106">Contains content properties for a specific app version.</span></span> <span data-ttu-id="b6132-107">各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b6132-107">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="b6132-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b6132-108">Methods</span></span>
|<span data-ttu-id="b6132-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="b6132-109">Method</span></span>|<span data-ttu-id="b6132-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b6132-110">Return Type</span></span>|<span data-ttu-id="b6132-111">説明</span><span class="sxs-lookup"><span data-stu-id="b6132-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b6132-112">mobileAppContents のリスト</span><span class="sxs-lookup"><span data-stu-id="b6132-112">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="b6132-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b6132-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="b6132-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b6132-114">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="b6132-115">MobileAppContent の取得</span><span class="sxs-lookup"><span data-stu-id="b6132-115">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="b6132-116">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="b6132-116">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="b6132-117">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b6132-117">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="b6132-118">mobileAppContent の作成</span><span class="sxs-lookup"><span data-stu-id="b6132-118">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="b6132-119">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="b6132-119">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="b6132-120">新しい [mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b6132-120">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="b6132-121">mobileAppContent の削除</span><span class="sxs-lookup"><span data-stu-id="b6132-121">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="b6132-122">なし</span><span class="sxs-lookup"><span data-stu-id="b6132-122">None</span></span>|<span data-ttu-id="b6132-123">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="b6132-123">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="b6132-124">mobileAppContent の更新</span><span class="sxs-lookup"><span data-stu-id="b6132-124">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="b6132-125">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="b6132-125">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="b6132-126">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b6132-126">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b6132-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6132-127">Properties</span></span>
|<span data-ttu-id="b6132-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6132-128">Property</span></span>|<span data-ttu-id="b6132-129">型</span><span class="sxs-lookup"><span data-stu-id="b6132-129">Type</span></span>|<span data-ttu-id="b6132-130">説明</span><span class="sxs-lookup"><span data-stu-id="b6132-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6132-131">id</span><span class="sxs-lookup"><span data-stu-id="b6132-131">id</span></span>|<span data-ttu-id="b6132-132">String</span><span class="sxs-lookup"><span data-stu-id="b6132-132">String</span></span>|<span data-ttu-id="b6132-133">アプリのコンテンツのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="b6132-133">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6132-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b6132-134">Relationships</span></span>
|<span data-ttu-id="b6132-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b6132-135">Relationship</span></span>|<span data-ttu-id="b6132-136">型</span><span class="sxs-lookup"><span data-stu-id="b6132-136">Type</span></span>|<span data-ttu-id="b6132-137">説明</span><span class="sxs-lookup"><span data-stu-id="b6132-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6132-138">files</span><span class="sxs-lookup"><span data-stu-id="b6132-138">files</span></span>|<span data-ttu-id="b6132-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b6132-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="b6132-140">このアプリのコンテンツのバージョンに関するファイルのリストです。</span><span class="sxs-lookup"><span data-stu-id="b6132-140">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b6132-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b6132-141">JSON Representation</span></span>
<span data-ttu-id="b6132-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b6132-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```



