---
title: mobileAppContent リソースの種類
description: 特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。 各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。
ms.openlocfilehash: 75d00e0b59fe3ca0848c5ad1bcdade76a9430ec1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023096"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="85248-104">mobileAppContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="85248-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="85248-105">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="85248-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85248-106">特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="85248-106">Contains content properties for a specific app version.</span></span> <span data-ttu-id="85248-107">各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="85248-107">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="85248-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="85248-108">Methods</span></span>
|<span data-ttu-id="85248-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="85248-109">Method</span></span>|<span data-ttu-id="85248-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="85248-110">Return Type</span></span>|<span data-ttu-id="85248-111">説明</span><span class="sxs-lookup"><span data-stu-id="85248-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="85248-112">mobileAppContents のリスト</span><span class="sxs-lookup"><span data-stu-id="85248-112">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="85248-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="85248-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="85248-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="85248-114">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="85248-115">MobileAppContent の取得</span><span class="sxs-lookup"><span data-stu-id="85248-115">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="85248-116">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="85248-116">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="85248-117">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="85248-117">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="85248-118">mobileAppContent の作成</span><span class="sxs-lookup"><span data-stu-id="85248-118">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="85248-119">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="85248-119">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="85248-120">新しい [mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="85248-120">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="85248-121">mobileAppContent の削除</span><span class="sxs-lookup"><span data-stu-id="85248-121">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="85248-122">なし</span><span class="sxs-lookup"><span data-stu-id="85248-122">None</span></span>|<span data-ttu-id="85248-123">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="85248-123">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="85248-124">mobileAppContent の更新</span><span class="sxs-lookup"><span data-stu-id="85248-124">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="85248-125">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="85248-125">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="85248-126">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="85248-126">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="85248-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85248-127">Properties</span></span>
|<span data-ttu-id="85248-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85248-128">Property</span></span>|<span data-ttu-id="85248-129">型</span><span class="sxs-lookup"><span data-stu-id="85248-129">Type</span></span>|<span data-ttu-id="85248-130">説明</span><span class="sxs-lookup"><span data-stu-id="85248-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85248-131">id</span><span class="sxs-lookup"><span data-stu-id="85248-131">id</span></span>|<span data-ttu-id="85248-132">String</span><span class="sxs-lookup"><span data-stu-id="85248-132">String</span></span>|<span data-ttu-id="85248-133">アプリのコンテンツのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="85248-133">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85248-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="85248-134">Relationships</span></span>
|<span data-ttu-id="85248-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="85248-135">Relationship</span></span>|<span data-ttu-id="85248-136">型</span><span class="sxs-lookup"><span data-stu-id="85248-136">Type</span></span>|<span data-ttu-id="85248-137">説明</span><span class="sxs-lookup"><span data-stu-id="85248-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85248-138">files</span><span class="sxs-lookup"><span data-stu-id="85248-138">files</span></span>|<span data-ttu-id="85248-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="85248-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="85248-140">このアプリのコンテンツのバージョンに関するファイルのリストです。</span><span class="sxs-lookup"><span data-stu-id="85248-140">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="85248-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="85248-141">JSON Representation</span></span>
<span data-ttu-id="85248-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="85248-142">Here is a JSON representation of the resource.</span></span>
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



