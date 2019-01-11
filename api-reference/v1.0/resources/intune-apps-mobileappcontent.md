---
title: mobileAppContent リソースの種類
description: 特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。 各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cf1deeaf1a18d68675e68e7040099d31cdea552f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880298"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="6c3f9-104">mobileAppContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6c3f9-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="6c3f9-105">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6c3f9-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c3f9-106">特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c3f9-106">Contains content properties for a specific app version.</span></span> <span data-ttu-id="6c3f9-107">各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="6c3f9-107">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="6c3f9-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6c3f9-108">Methods</span></span>
|<span data-ttu-id="6c3f9-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="6c3f9-109">Method</span></span>|<span data-ttu-id="6c3f9-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6c3f9-110">Return Type</span></span>|<span data-ttu-id="6c3f9-111">説明</span><span class="sxs-lookup"><span data-stu-id="6c3f9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6c3f9-112">mobileAppContents のリスト</span><span class="sxs-lookup"><span data-stu-id="6c3f9-112">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="6c3f9-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6c3f9-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="6c3f9-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6c3f9-114">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="6c3f9-115">MobileAppContent の取得</span><span class="sxs-lookup"><span data-stu-id="6c3f9-115">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="6c3f9-116">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="6c3f9-116">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="6c3f9-117">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6c3f9-117">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="6c3f9-118">mobileAppContent の作成</span><span class="sxs-lookup"><span data-stu-id="6c3f9-118">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="6c3f9-119">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="6c3f9-119">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="6c3f9-120">新しい [mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6c3f9-120">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="6c3f9-121">mobileAppContent の削除</span><span class="sxs-lookup"><span data-stu-id="6c3f9-121">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="6c3f9-122">なし</span><span class="sxs-lookup"><span data-stu-id="6c3f9-122">None</span></span>|<span data-ttu-id="6c3f9-123">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="6c3f9-123">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="6c3f9-124">mobileAppContent の更新</span><span class="sxs-lookup"><span data-stu-id="6c3f9-124">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="6c3f9-125">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="6c3f9-125">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="6c3f9-126">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6c3f9-126">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c3f9-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c3f9-127">Properties</span></span>
|<span data-ttu-id="6c3f9-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c3f9-128">Property</span></span>|<span data-ttu-id="6c3f9-129">種類</span><span class="sxs-lookup"><span data-stu-id="6c3f9-129">Type</span></span>|<span data-ttu-id="6c3f9-130">説明</span><span class="sxs-lookup"><span data-stu-id="6c3f9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c3f9-131">ID</span><span class="sxs-lookup"><span data-stu-id="6c3f9-131">id</span></span>|<span data-ttu-id="6c3f9-132">String</span><span class="sxs-lookup"><span data-stu-id="6c3f9-132">String</span></span>|<span data-ttu-id="6c3f9-133">アプリのコンテンツのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="6c3f9-133">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c3f9-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6c3f9-134">Relationships</span></span>
|<span data-ttu-id="6c3f9-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6c3f9-135">Relationship</span></span>|<span data-ttu-id="6c3f9-136">型</span><span class="sxs-lookup"><span data-stu-id="6c3f9-136">Type</span></span>|<span data-ttu-id="6c3f9-137">説明</span><span class="sxs-lookup"><span data-stu-id="6c3f9-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c3f9-138">files</span><span class="sxs-lookup"><span data-stu-id="6c3f9-138">files</span></span>|<span data-ttu-id="6c3f9-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6c3f9-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="6c3f9-140">このアプリのコンテンツのバージョンに関するファイルのリストです。</span><span class="sxs-lookup"><span data-stu-id="6c3f9-140">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c3f9-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c3f9-141">JSON Representation</span></span>
<span data-ttu-id="6c3f9-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6c3f9-142">Here is a JSON representation of the resource.</span></span>
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



