---
title: mobileAppContent リソースの種類
description: 特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。 各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。
ms.openlocfilehash: e57c4c0823636143962ac5fe1c50f4377e731f84
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070095"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="72ecd-104">mobileAppContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="72ecd-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="72ecd-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="72ecd-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72ecd-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72ecd-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72ecd-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="72ecd-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72ecd-108">特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="72ecd-108">Contains content properties for a specific app version.</span></span> <span data-ttu-id="72ecd-109">各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="72ecd-109">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="72ecd-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="72ecd-110">Methods</span></span>
|<span data-ttu-id="72ecd-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="72ecd-111">Method</span></span>|<span data-ttu-id="72ecd-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="72ecd-112">Return Type</span></span>|<span data-ttu-id="72ecd-113">説明</span><span class="sxs-lookup"><span data-stu-id="72ecd-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="72ecd-114">mobileAppContents のリスト</span><span class="sxs-lookup"><span data-stu-id="72ecd-114">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="72ecd-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="72ecd-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="72ecd-116">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="72ecd-116">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="72ecd-117">MobileAppContent の取得</span><span class="sxs-lookup"><span data-stu-id="72ecd-117">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="72ecd-118">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="72ecd-118">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="72ecd-119">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="72ecd-119">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="72ecd-120">mobileAppContent の作成</span><span class="sxs-lookup"><span data-stu-id="72ecd-120">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="72ecd-121">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="72ecd-121">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="72ecd-122">新しい [mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="72ecd-122">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="72ecd-123">mobileAppContent の削除</span><span class="sxs-lookup"><span data-stu-id="72ecd-123">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="72ecd-124">なし</span><span class="sxs-lookup"><span data-stu-id="72ecd-124">None</span></span>|<span data-ttu-id="72ecd-125">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="72ecd-125">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="72ecd-126">mobileAppContent の更新</span><span class="sxs-lookup"><span data-stu-id="72ecd-126">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="72ecd-127">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="72ecd-127">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="72ecd-128">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="72ecd-128">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="72ecd-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="72ecd-129">Properties</span></span>
|<span data-ttu-id="72ecd-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="72ecd-130">Property</span></span>|<span data-ttu-id="72ecd-131">型</span><span class="sxs-lookup"><span data-stu-id="72ecd-131">Type</span></span>|<span data-ttu-id="72ecd-132">説明</span><span class="sxs-lookup"><span data-stu-id="72ecd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72ecd-133">id</span><span class="sxs-lookup"><span data-stu-id="72ecd-133">id</span></span>|<span data-ttu-id="72ecd-134">String</span><span class="sxs-lookup"><span data-stu-id="72ecd-134">String</span></span>|<span data-ttu-id="72ecd-135">アプリのコンテンツのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="72ecd-135">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72ecd-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="72ecd-136">Relationships</span></span>
|<span data-ttu-id="72ecd-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="72ecd-137">Relationship</span></span>|<span data-ttu-id="72ecd-138">型</span><span class="sxs-lookup"><span data-stu-id="72ecd-138">Type</span></span>|<span data-ttu-id="72ecd-139">説明</span><span class="sxs-lookup"><span data-stu-id="72ecd-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72ecd-140">files</span><span class="sxs-lookup"><span data-stu-id="72ecd-140">files</span></span>|<span data-ttu-id="72ecd-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="72ecd-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="72ecd-142">このアプリのコンテンツのバージョンに関するファイルのリストです。</span><span class="sxs-lookup"><span data-stu-id="72ecd-142">The list of files for this app content version.</span></span>|
|<span data-ttu-id="72ecd-143">containedApps</span><span class="sxs-lookup"><span data-stu-id="72ecd-143">containedApps</span></span>|<span data-ttu-id="72ecd-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="72ecd-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="72ecd-145">パッケージとして機能する、MobileLobApp に含まれているアプリケーションのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="72ecd-145">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="72ecd-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="72ecd-146">JSON Representation</span></span>
<span data-ttu-id="72ecd-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="72ecd-147">Here is a JSON representation of the resource.</span></span>
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





