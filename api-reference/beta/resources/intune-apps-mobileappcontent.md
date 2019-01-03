---
title: mobileAppContent リソースの種類
description: 特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。 各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。
author: tfitzmac
ms.openlocfilehash: 8cc5bd6e3c7aa5f08236d2662821a9a5d03707d0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360348"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="f21eb-104">mobileAppContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f21eb-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="f21eb-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f21eb-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f21eb-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f21eb-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f21eb-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f21eb-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f21eb-108">特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f21eb-108">Contains content properties for a specific app version.</span></span> <span data-ttu-id="f21eb-109">各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f21eb-109">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="f21eb-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="f21eb-110">Methods</span></span>
|<span data-ttu-id="f21eb-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="f21eb-111">Method</span></span>|<span data-ttu-id="f21eb-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f21eb-112">Return Type</span></span>|<span data-ttu-id="f21eb-113">説明</span><span class="sxs-lookup"><span data-stu-id="f21eb-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f21eb-114">mobileAppContents のリスト</span><span class="sxs-lookup"><span data-stu-id="f21eb-114">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="f21eb-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f21eb-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="f21eb-116">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f21eb-116">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="f21eb-117">MobileAppContent の取得</span><span class="sxs-lookup"><span data-stu-id="f21eb-117">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="f21eb-118">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="f21eb-118">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="f21eb-119">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f21eb-119">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="f21eb-120">mobileAppContent の作成</span><span class="sxs-lookup"><span data-stu-id="f21eb-120">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="f21eb-121">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="f21eb-121">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="f21eb-122">新しい [mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f21eb-122">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="f21eb-123">mobileAppContent の削除</span><span class="sxs-lookup"><span data-stu-id="f21eb-123">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="f21eb-124">なし</span><span class="sxs-lookup"><span data-stu-id="f21eb-124">None</span></span>|<span data-ttu-id="f21eb-125">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="f21eb-125">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="f21eb-126">mobileAppContent の更新</span><span class="sxs-lookup"><span data-stu-id="f21eb-126">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="f21eb-127">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="f21eb-127">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="f21eb-128">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f21eb-128">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f21eb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f21eb-129">Properties</span></span>
|<span data-ttu-id="f21eb-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f21eb-130">Property</span></span>|<span data-ttu-id="f21eb-131">種類</span><span class="sxs-lookup"><span data-stu-id="f21eb-131">Type</span></span>|<span data-ttu-id="f21eb-132">説明</span><span class="sxs-lookup"><span data-stu-id="f21eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f21eb-133">ID</span><span class="sxs-lookup"><span data-stu-id="f21eb-133">id</span></span>|<span data-ttu-id="f21eb-134">String</span><span class="sxs-lookup"><span data-stu-id="f21eb-134">String</span></span>|<span data-ttu-id="f21eb-135">アプリのコンテンツのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="f21eb-135">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f21eb-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f21eb-136">Relationships</span></span>
|<span data-ttu-id="f21eb-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f21eb-137">Relationship</span></span>|<span data-ttu-id="f21eb-138">型</span><span class="sxs-lookup"><span data-stu-id="f21eb-138">Type</span></span>|<span data-ttu-id="f21eb-139">説明</span><span class="sxs-lookup"><span data-stu-id="f21eb-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f21eb-140">files</span><span class="sxs-lookup"><span data-stu-id="f21eb-140">files</span></span>|<span data-ttu-id="f21eb-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f21eb-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="f21eb-142">このアプリのコンテンツのバージョンに関するファイルのリストです。</span><span class="sxs-lookup"><span data-stu-id="f21eb-142">The list of files for this app content version.</span></span>|
|<span data-ttu-id="f21eb-143">containedApps</span><span class="sxs-lookup"><span data-stu-id="f21eb-143">containedApps</span></span>|<span data-ttu-id="f21eb-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f21eb-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="f21eb-145">パッケージとして機能する、MobileLobApp に含まれているアプリケーションのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f21eb-145">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f21eb-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f21eb-146">JSON Representation</span></span>
<span data-ttu-id="f21eb-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f21eb-147">Here is a JSON representation of the resource.</span></span>
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




