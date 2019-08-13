---
title: mobileAppRelationship リソースの種類
description: 子モバイルアプリと親モバイルアプリとの関係を記述します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 97ff0d0331523a93d57c9f14cd8bb45910b9cdb2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331855"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="1f131-103">mobileAppRelationship リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1f131-103">mobileAppRelationship resource type</span></span>

> <span data-ttu-id="1f131-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f131-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f131-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1f131-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f131-106">子モバイルアプリと親モバイルアプリとの関係を記述します。</span><span class="sxs-lookup"><span data-stu-id="1f131-106">Describes the relationship for a child mobile app to its parent mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="1f131-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="1f131-107">Methods</span></span>
|<span data-ttu-id="1f131-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1f131-108">Method</span></span>|<span data-ttu-id="1f131-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1f131-109">Return Type</span></span>|<span data-ttu-id="1f131-110">説明</span><span class="sxs-lookup"><span data-stu-id="1f131-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1f131-111">リスト mobileAppRelationships</span><span class="sxs-lookup"><span data-stu-id="1f131-111">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="1f131-112">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1f131-112">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="1f131-113">[MobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1f131-113">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="1f131-114">MobileAppRelationship を取得する</span><span class="sxs-lookup"><span data-stu-id="1f131-114">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="1f131-115">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="1f131-115">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="1f131-116">[MobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1f131-116">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1f131-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f131-117">Properties</span></span>
|<span data-ttu-id="1f131-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f131-118">Property</span></span>|<span data-ttu-id="1f131-119">型</span><span class="sxs-lookup"><span data-stu-id="1f131-119">Type</span></span>|<span data-ttu-id="1f131-120">説明</span><span class="sxs-lookup"><span data-stu-id="1f131-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f131-121">id</span><span class="sxs-lookup"><span data-stu-id="1f131-121">id</span></span>|<span data-ttu-id="1f131-122">String</span><span class="sxs-lookup"><span data-stu-id="1f131-122">String</span></span>|<span data-ttu-id="1f131-123">リレーションシップエンティティ id。</span><span class="sxs-lookup"><span data-stu-id="1f131-123">The relationship entity id.</span></span>|
|<span data-ttu-id="1f131-124">targetId</span><span class="sxs-lookup"><span data-stu-id="1f131-124">targetId</span></span>|<span data-ttu-id="1f131-125">String</span><span class="sxs-lookup"><span data-stu-id="1f131-125">String</span></span>|<span data-ttu-id="1f131-126">ターゲットの子モバイルアプリのアプリ id。</span><span class="sxs-lookup"><span data-stu-id="1f131-126">The target child mobile app's app id.</span></span>|
|<span data-ttu-id="1f131-127">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="1f131-127">targetDisplayName</span></span>|<span data-ttu-id="1f131-128">String</span><span class="sxs-lookup"><span data-stu-id="1f131-128">String</span></span>|<span data-ttu-id="1f131-129">ターゲットの子モバイルアプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="1f131-129">The target child mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f131-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1f131-130">Relationships</span></span>
<span data-ttu-id="1f131-131">なし</span><span class="sxs-lookup"><span data-stu-id="1f131-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f131-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1f131-132">JSON Representation</span></span>
<span data-ttu-id="1f131-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1f131-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppRelationship"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppRelationship",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String"
}
```



