---
title: mobileAppContent リソースの種類
description: 特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。 各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 57266335608e97924edbddc056d931725a633e4f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939120"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="1d808-104">mobileAppContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1d808-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="1d808-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1d808-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d808-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d808-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d808-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1d808-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d808-108">特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1d808-108">Contains content properties for a specific app version.</span></span> <span data-ttu-id="1d808-109">各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1d808-109">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="1d808-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="1d808-110">Methods</span></span>
|<span data-ttu-id="1d808-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="1d808-111">Method</span></span>|<span data-ttu-id="1d808-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1d808-112">Return Type</span></span>|<span data-ttu-id="1d808-113">説明</span><span class="sxs-lookup"><span data-stu-id="1d808-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1d808-114">mobileAppContents のリスト</span><span class="sxs-lookup"><span data-stu-id="1d808-114">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="1d808-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1d808-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="1d808-116">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1d808-116">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="1d808-117">MobileAppContent の取得</span><span class="sxs-lookup"><span data-stu-id="1d808-117">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="1d808-118">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="1d808-118">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="1d808-119">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1d808-119">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="1d808-120">mobileAppContent の作成</span><span class="sxs-lookup"><span data-stu-id="1d808-120">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="1d808-121">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="1d808-121">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="1d808-122">新しい [mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1d808-122">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="1d808-123">mobileAppContent の削除</span><span class="sxs-lookup"><span data-stu-id="1d808-123">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="1d808-124">なし</span><span class="sxs-lookup"><span data-stu-id="1d808-124">None</span></span>|<span data-ttu-id="1d808-125">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="1d808-125">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="1d808-126">mobileAppContent の更新</span><span class="sxs-lookup"><span data-stu-id="1d808-126">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="1d808-127">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="1d808-127">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="1d808-128">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1d808-128">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1d808-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d808-129">Properties</span></span>
|<span data-ttu-id="1d808-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d808-130">Property</span></span>|<span data-ttu-id="1d808-131">型</span><span class="sxs-lookup"><span data-stu-id="1d808-131">Type</span></span>|<span data-ttu-id="1d808-132">説明</span><span class="sxs-lookup"><span data-stu-id="1d808-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d808-133">ID</span><span class="sxs-lookup"><span data-stu-id="1d808-133">id</span></span>|<span data-ttu-id="1d808-134">String</span><span class="sxs-lookup"><span data-stu-id="1d808-134">String</span></span>|<span data-ttu-id="1d808-135">アプリのコンテンツのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="1d808-135">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d808-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1d808-136">Relationships</span></span>
|<span data-ttu-id="1d808-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1d808-137">Relationship</span></span>|<span data-ttu-id="1d808-138">型</span><span class="sxs-lookup"><span data-stu-id="1d808-138">Type</span></span>|<span data-ttu-id="1d808-139">説明</span><span class="sxs-lookup"><span data-stu-id="1d808-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d808-140">files</span><span class="sxs-lookup"><span data-stu-id="1d808-140">files</span></span>|<span data-ttu-id="1d808-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1d808-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="1d808-142">このアプリのコンテンツのバージョンに関するファイルのリストです。</span><span class="sxs-lookup"><span data-stu-id="1d808-142">The list of files for this app content version.</span></span>|
|<span data-ttu-id="1d808-143">containedApps</span><span class="sxs-lookup"><span data-stu-id="1d808-143">containedApps</span></span>|<span data-ttu-id="1d808-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1d808-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="1d808-145">パッケージとして機能する、MobileLobApp に含まれているアプリケーションのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="1d808-145">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d808-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d808-146">JSON Representation</span></span>
<span data-ttu-id="1d808-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1d808-147">Here is a JSON representation of the resource.</span></span>
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





