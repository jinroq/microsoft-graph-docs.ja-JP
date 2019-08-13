---
title: mobileAppContent リソースの種類
description: 特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。 各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 090a55e73ac823101386c23b18811163131099a6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327515"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="6a897-104">mobileAppContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6a897-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="6a897-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a897-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a897-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a897-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a897-107">特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6a897-107">Contains content properties for a specific app version.</span></span> <span data-ttu-id="6a897-108">各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="6a897-108">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="6a897-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="6a897-109">Methods</span></span>
|<span data-ttu-id="6a897-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="6a897-110">Method</span></span>|<span data-ttu-id="6a897-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6a897-111">Return Type</span></span>|<span data-ttu-id="6a897-112">説明</span><span class="sxs-lookup"><span data-stu-id="6a897-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6a897-113">mobileAppContents のリスト</span><span class="sxs-lookup"><span data-stu-id="6a897-113">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="6a897-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6a897-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="6a897-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6a897-115">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="6a897-116">MobileAppContent の取得</span><span class="sxs-lookup"><span data-stu-id="6a897-116">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="6a897-117">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="6a897-117">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="6a897-118">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6a897-118">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="6a897-119">mobileAppContent の作成</span><span class="sxs-lookup"><span data-stu-id="6a897-119">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="6a897-120">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="6a897-120">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="6a897-121">新しい [mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6a897-121">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="6a897-122">mobileAppContent の削除</span><span class="sxs-lookup"><span data-stu-id="6a897-122">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="6a897-123">なし</span><span class="sxs-lookup"><span data-stu-id="6a897-123">None</span></span>|<span data-ttu-id="6a897-124">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="6a897-124">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="6a897-125">mobileAppContent の更新</span><span class="sxs-lookup"><span data-stu-id="6a897-125">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="6a897-126">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="6a897-126">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="6a897-127">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6a897-127">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6a897-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a897-128">Properties</span></span>
|<span data-ttu-id="6a897-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a897-129">Property</span></span>|<span data-ttu-id="6a897-130">型</span><span class="sxs-lookup"><span data-stu-id="6a897-130">Type</span></span>|<span data-ttu-id="6a897-131">説明</span><span class="sxs-lookup"><span data-stu-id="6a897-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a897-132">id</span><span class="sxs-lookup"><span data-stu-id="6a897-132">id</span></span>|<span data-ttu-id="6a897-133">String</span><span class="sxs-lookup"><span data-stu-id="6a897-133">String</span></span>|<span data-ttu-id="6a897-134">アプリのコンテンツのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="6a897-134">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a897-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6a897-135">Relationships</span></span>
|<span data-ttu-id="6a897-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6a897-136">Relationship</span></span>|<span data-ttu-id="6a897-137">型</span><span class="sxs-lookup"><span data-stu-id="6a897-137">Type</span></span>|<span data-ttu-id="6a897-138">説明</span><span class="sxs-lookup"><span data-stu-id="6a897-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a897-139">files</span><span class="sxs-lookup"><span data-stu-id="6a897-139">files</span></span>|<span data-ttu-id="6a897-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6a897-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="6a897-141">このアプリのコンテンツのバージョンに関するファイルのリストです。</span><span class="sxs-lookup"><span data-stu-id="6a897-141">The list of files for this app content version.</span></span>|
|<span data-ttu-id="6a897-142">containedApps</span><span class="sxs-lookup"><span data-stu-id="6a897-142">containedApps</span></span>|<span data-ttu-id="6a897-143">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6a897-143">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="6a897-144">パッケージとして機能する MobileLobApp に含まれているアプリのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="6a897-144">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6a897-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6a897-145">JSON Representation</span></span>
<span data-ttu-id="6a897-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6a897-146">Here is a JSON representation of the resource.</span></span>
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



