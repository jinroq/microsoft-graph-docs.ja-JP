---
title: mobileAppRelationship リソースの種類
description: 子モバイルアプリと親モバイルアプリとの関係を記述します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e193878122a3a43cd97d05ad1bdc5bea302fcc8a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991822"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="f5983-103">mobileAppRelationship リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f5983-103">mobileAppRelationship resource type</span></span>

> <span data-ttu-id="f5983-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5983-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5983-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f5983-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5983-106">子モバイルアプリと親モバイルアプリとの関係を記述します。</span><span class="sxs-lookup"><span data-stu-id="f5983-106">Describes the relationship for a child mobile app to its parent mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="f5983-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f5983-107">Methods</span></span>
|<span data-ttu-id="f5983-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f5983-108">Method</span></span>|<span data-ttu-id="f5983-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f5983-109">Return Type</span></span>|<span data-ttu-id="f5983-110">説明</span><span class="sxs-lookup"><span data-stu-id="f5983-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f5983-111">リスト mobileAppRelationships</span><span class="sxs-lookup"><span data-stu-id="f5983-111">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="f5983-112">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f5983-112">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="f5983-113">[MobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f5983-113">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="f5983-114">MobileAppRelationship を取得する</span><span class="sxs-lookup"><span data-stu-id="f5983-114">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="f5983-115">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="f5983-115">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="f5983-116">[MobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f5983-116">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f5983-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5983-117">Properties</span></span>
|<span data-ttu-id="f5983-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5983-118">Property</span></span>|<span data-ttu-id="f5983-119">型</span><span class="sxs-lookup"><span data-stu-id="f5983-119">Type</span></span>|<span data-ttu-id="f5983-120">説明</span><span class="sxs-lookup"><span data-stu-id="f5983-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5983-121">id</span><span class="sxs-lookup"><span data-stu-id="f5983-121">id</span></span>|<span data-ttu-id="f5983-122">String</span><span class="sxs-lookup"><span data-stu-id="f5983-122">String</span></span>|<span data-ttu-id="f5983-123">リレーションシップエンティティ id。</span><span class="sxs-lookup"><span data-stu-id="f5983-123">The relationship entity id.</span></span>|
|<span data-ttu-id="f5983-124">targetId</span><span class="sxs-lookup"><span data-stu-id="f5983-124">targetId</span></span>|<span data-ttu-id="f5983-125">String</span><span class="sxs-lookup"><span data-stu-id="f5983-125">String</span></span>|<span data-ttu-id="f5983-126">ターゲットの子モバイルアプリのアプリ id。</span><span class="sxs-lookup"><span data-stu-id="f5983-126">The target child mobile app's app id.</span></span>|
|<span data-ttu-id="f5983-127">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="f5983-127">targetDisplayName</span></span>|<span data-ttu-id="f5983-128">String</span><span class="sxs-lookup"><span data-stu-id="f5983-128">String</span></span>|<span data-ttu-id="f5983-129">ターゲットの子モバイルアプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="f5983-129">The target child mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5983-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f5983-130">Relationships</span></span>
<span data-ttu-id="f5983-131">なし</span><span class="sxs-lookup"><span data-stu-id="f5983-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5983-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f5983-132">JSON Representation</span></span>
<span data-ttu-id="f5983-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f5983-133">Here is a JSON representation of the resource.</span></span>
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





