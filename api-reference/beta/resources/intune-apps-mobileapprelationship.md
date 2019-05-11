---
title: mobileAppRelationship リソースの種類
description: 子モバイルアプリと親モバイルアプリとの関係を記述します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c871ba51733195947243fa9b22824156108f5eb7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949886"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="eadb3-103">mobileAppRelationship リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eadb3-103">mobileAppRelationship resource type</span></span>

> <span data-ttu-id="eadb3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eadb3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eadb3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eadb3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eadb3-106">子モバイルアプリと親モバイルアプリとの関係を記述します。</span><span class="sxs-lookup"><span data-stu-id="eadb3-106">Describes the relationship for a child mobile app to its parent mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="eadb3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="eadb3-107">Methods</span></span>
|<span data-ttu-id="eadb3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="eadb3-108">Method</span></span>|<span data-ttu-id="eadb3-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="eadb3-109">Return Type</span></span>|<span data-ttu-id="eadb3-110">説明</span><span class="sxs-lookup"><span data-stu-id="eadb3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eadb3-111">リスト mobileAppRelationships</span><span class="sxs-lookup"><span data-stu-id="eadb3-111">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="eadb3-112">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="eadb3-112">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="eadb3-113">[MobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="eadb3-113">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="eadb3-114">MobileAppRelationship を取得する</span><span class="sxs-lookup"><span data-stu-id="eadb3-114">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="eadb3-115">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="eadb3-115">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="eadb3-116">[MobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="eadb3-116">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="eadb3-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eadb3-117">Properties</span></span>
|<span data-ttu-id="eadb3-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eadb3-118">Property</span></span>|<span data-ttu-id="eadb3-119">型</span><span class="sxs-lookup"><span data-stu-id="eadb3-119">Type</span></span>|<span data-ttu-id="eadb3-120">説明</span><span class="sxs-lookup"><span data-stu-id="eadb3-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eadb3-121">id</span><span class="sxs-lookup"><span data-stu-id="eadb3-121">id</span></span>|<span data-ttu-id="eadb3-122">String</span><span class="sxs-lookup"><span data-stu-id="eadb3-122">String</span></span>|<span data-ttu-id="eadb3-123">リレーションシップエンティティ id。</span><span class="sxs-lookup"><span data-stu-id="eadb3-123">The relationship entity id.</span></span>|
|<span data-ttu-id="eadb3-124">targetId</span><span class="sxs-lookup"><span data-stu-id="eadb3-124">targetId</span></span>|<span data-ttu-id="eadb3-125">String</span><span class="sxs-lookup"><span data-stu-id="eadb3-125">String</span></span>|<span data-ttu-id="eadb3-126">ターゲットの子モバイルアプリのアプリ id。</span><span class="sxs-lookup"><span data-stu-id="eadb3-126">The target child mobile app's app id.</span></span>|
|<span data-ttu-id="eadb3-127">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="eadb3-127">targetDisplayName</span></span>|<span data-ttu-id="eadb3-128">String</span><span class="sxs-lookup"><span data-stu-id="eadb3-128">String</span></span>|<span data-ttu-id="eadb3-129">ターゲットの子モバイルアプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="eadb3-129">The target child mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eadb3-130">関係</span><span class="sxs-lookup"><span data-stu-id="eadb3-130">Relationships</span></span>
<span data-ttu-id="eadb3-131">なし</span><span class="sxs-lookup"><span data-stu-id="eadb3-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eadb3-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eadb3-132">JSON Representation</span></span>
<span data-ttu-id="eadb3-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eadb3-133">Here is a JSON representation of the resource.</span></span>
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




