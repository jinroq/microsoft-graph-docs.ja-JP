---
title: mobileAppContent リソースの種類
description: 特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。 各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a3ed4b5d1e05b3d1f8621cecf875a6fbbe9d740
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990310"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="c7679-104">mobileAppContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c7679-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="c7679-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7679-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7679-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c7679-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7679-107">特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c7679-107">Contains content properties for a specific app version.</span></span> <span data-ttu-id="c7679-108">各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="c7679-108">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="c7679-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c7679-109">Methods</span></span>
|<span data-ttu-id="c7679-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="c7679-110">Method</span></span>|<span data-ttu-id="c7679-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c7679-111">Return Type</span></span>|<span data-ttu-id="c7679-112">説明</span><span class="sxs-lookup"><span data-stu-id="c7679-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c7679-113">mobileAppContents のリスト</span><span class="sxs-lookup"><span data-stu-id="c7679-113">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="c7679-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c7679-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="c7679-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c7679-115">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="c7679-116">MobileAppContent の取得</span><span class="sxs-lookup"><span data-stu-id="c7679-116">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="c7679-117">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c7679-117">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="c7679-118">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c7679-118">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="c7679-119">mobileAppContent の作成</span><span class="sxs-lookup"><span data-stu-id="c7679-119">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="c7679-120">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c7679-120">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="c7679-121">新しい [mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c7679-121">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="c7679-122">mobileAppContent の削除</span><span class="sxs-lookup"><span data-stu-id="c7679-122">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="c7679-123">なし</span><span class="sxs-lookup"><span data-stu-id="c7679-123">None</span></span>|<span data-ttu-id="c7679-124">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="c7679-124">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="c7679-125">mobileAppContent の更新</span><span class="sxs-lookup"><span data-stu-id="c7679-125">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="c7679-126">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c7679-126">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="c7679-127">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c7679-127">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c7679-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7679-128">Properties</span></span>
|<span data-ttu-id="c7679-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7679-129">Property</span></span>|<span data-ttu-id="c7679-130">型</span><span class="sxs-lookup"><span data-stu-id="c7679-130">Type</span></span>|<span data-ttu-id="c7679-131">説明</span><span class="sxs-lookup"><span data-stu-id="c7679-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7679-132">id</span><span class="sxs-lookup"><span data-stu-id="c7679-132">id</span></span>|<span data-ttu-id="c7679-133">String</span><span class="sxs-lookup"><span data-stu-id="c7679-133">String</span></span>|<span data-ttu-id="c7679-134">アプリのコンテンツのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="c7679-134">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7679-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c7679-135">Relationships</span></span>
|<span data-ttu-id="c7679-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c7679-136">Relationship</span></span>|<span data-ttu-id="c7679-137">型</span><span class="sxs-lookup"><span data-stu-id="c7679-137">Type</span></span>|<span data-ttu-id="c7679-138">説明</span><span class="sxs-lookup"><span data-stu-id="c7679-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7679-139">files</span><span class="sxs-lookup"><span data-stu-id="c7679-139">files</span></span>|<span data-ttu-id="c7679-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c7679-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="c7679-141">このアプリのコンテンツのバージョンに関するファイルのリストです。</span><span class="sxs-lookup"><span data-stu-id="c7679-141">The list of files for this app content version.</span></span>|
|<span data-ttu-id="c7679-142">containedApps</span><span class="sxs-lookup"><span data-stu-id="c7679-142">containedApps</span></span>|<span data-ttu-id="c7679-143">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c7679-143">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="c7679-144">パッケージとして機能する MobileLobApp に含まれているアプリのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="c7679-144">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7679-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c7679-145">JSON Representation</span></span>
<span data-ttu-id="c7679-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c7679-146">Here is a JSON representation of the resource.</span></span>
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





