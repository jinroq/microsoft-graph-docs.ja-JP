---
title: mobileAppRelationship リソースの種類
description: 子モバイルアプリと親モバイルアプリとの関係を記述します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1ed999914958578bfa4c39b99b27ff159827e207
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809270"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="e10a5-103">mobileAppRelationship リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e10a5-103">mobileAppRelationship resource type</span></span>

> <span data-ttu-id="e10a5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e10a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e10a5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e10a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e10a5-106">子モバイルアプリと親モバイルアプリとの関係を記述します。</span><span class="sxs-lookup"><span data-stu-id="e10a5-106">Describes the relationship for a child mobile app to its parent mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="e10a5-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e10a5-107">Methods</span></span>
|<span data-ttu-id="e10a5-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e10a5-108">Method</span></span>|<span data-ttu-id="e10a5-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e10a5-109">Return Type</span></span>|<span data-ttu-id="e10a5-110">説明</span><span class="sxs-lookup"><span data-stu-id="e10a5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e10a5-111">リスト mobileAppRelationships</span><span class="sxs-lookup"><span data-stu-id="e10a5-111">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="e10a5-112">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e10a5-112">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="e10a5-113">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e10a5-113">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="e10a5-114">mobileAppRelationship を取得する</span><span class="sxs-lookup"><span data-stu-id="e10a5-114">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="e10a5-115">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="e10a5-115">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="e10a5-116">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e10a5-116">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e10a5-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e10a5-117">Properties</span></span>
|<span data-ttu-id="e10a5-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e10a5-118">Property</span></span>|<span data-ttu-id="e10a5-119">型</span><span class="sxs-lookup"><span data-stu-id="e10a5-119">Type</span></span>|<span data-ttu-id="e10a5-120">説明</span><span class="sxs-lookup"><span data-stu-id="e10a5-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e10a5-121">id</span><span class="sxs-lookup"><span data-stu-id="e10a5-121">id</span></span>|<span data-ttu-id="e10a5-122">String</span><span class="sxs-lookup"><span data-stu-id="e10a5-122">String</span></span>|<span data-ttu-id="e10a5-123">リレーションシップエンティティ id。</span><span class="sxs-lookup"><span data-stu-id="e10a5-123">The relationship entity id.</span></span>|
|<span data-ttu-id="e10a5-124">targetId</span><span class="sxs-lookup"><span data-stu-id="e10a5-124">targetId</span></span>|<span data-ttu-id="e10a5-125">文字列</span><span class="sxs-lookup"><span data-stu-id="e10a5-125">String</span></span>|<span data-ttu-id="e10a5-126">ターゲットの子モバイルアプリのアプリ id。</span><span class="sxs-lookup"><span data-stu-id="e10a5-126">The target child mobile app's app id.</span></span>|
|<span data-ttu-id="e10a5-127">targetdisplayname</span><span class="sxs-lookup"><span data-stu-id="e10a5-127">targetDisplayName</span></span>|<span data-ttu-id="e10a5-128">文字列</span><span class="sxs-lookup"><span data-stu-id="e10a5-128">String</span></span>|<span data-ttu-id="e10a5-129">ターゲットの子モバイルアプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="e10a5-129">The target child mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e10a5-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e10a5-130">Relationships</span></span>
<span data-ttu-id="e10a5-131">なし</span><span class="sxs-lookup"><span data-stu-id="e10a5-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e10a5-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e10a5-132">JSON Representation</span></span>
<span data-ttu-id="e10a5-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e10a5-133">Here is a JSON representation of the resource.</span></span>
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





