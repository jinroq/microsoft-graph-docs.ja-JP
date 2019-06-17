---
title: mobileAppDependency リソースの種類
description: 2つのモバイルアプリ間の依存関係の種類を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a29f658a67c3930b1b693589dc9115c0c1ff185
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990261"
---
# <a name="mobileappdependency-resource-type"></a><span data-ttu-id="ab96f-103">mobileAppDependency リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ab96f-103">mobileAppDependency resource type</span></span>

> <span data-ttu-id="ab96f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab96f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab96f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ab96f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab96f-106">2つのモバイルアプリ間の依存関係の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="ab96f-106">Describes a dependency type between two mobile apps.</span></span>


<span data-ttu-id="ab96f-107">[MobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ab96f-107">Inherits from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ab96f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ab96f-108">Methods</span></span>
|<span data-ttu-id="ab96f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="ab96f-109">Method</span></span>|<span data-ttu-id="ab96f-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ab96f-110">Return Type</span></span>|<span data-ttu-id="ab96f-111">説明</span><span class="sxs-lookup"><span data-stu-id="ab96f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ab96f-112">リスト mobileAppDependencies</span><span class="sxs-lookup"><span data-stu-id="ab96f-112">List mobileAppDependencies</span></span>](../api/intune-apps-mobileappdependency-list.md)|<span data-ttu-id="ab96f-113">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ab96f-113">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md) collection</span></span>|<span data-ttu-id="ab96f-114">[MobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ab96f-114">List properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) objects.</span></span>|
|[<span data-ttu-id="ab96f-115">MobileAppDependency を取得する</span><span class="sxs-lookup"><span data-stu-id="ab96f-115">Get mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-get.md)|[<span data-ttu-id="ab96f-116">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="ab96f-116">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="ab96f-117">[MobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ab96f-117">Read properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|
|[<span data-ttu-id="ab96f-118">MobileAppDependency を作成する</span><span class="sxs-lookup"><span data-stu-id="ab96f-118">Create mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-create.md)|[<span data-ttu-id="ab96f-119">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="ab96f-119">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="ab96f-120">新しい[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ab96f-120">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|
|[<span data-ttu-id="ab96f-121">MobileAppDependency の削除</span><span class="sxs-lookup"><span data-stu-id="ab96f-121">Delete mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-delete.md)|<span data-ttu-id="ab96f-122">None</span><span class="sxs-lookup"><span data-stu-id="ab96f-122">None</span></span>|<span data-ttu-id="ab96f-123">[MobileAppDependency](../resources/intune-apps-mobileappdependency.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="ab96f-123">Deletes a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>|
|[<span data-ttu-id="ab96f-124">MobileAppDependency の更新</span><span class="sxs-lookup"><span data-stu-id="ab96f-124">Update mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-update.md)|[<span data-ttu-id="ab96f-125">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="ab96f-125">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="ab96f-126">[MobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ab96f-126">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ab96f-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab96f-127">Properties</span></span>
|<span data-ttu-id="ab96f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab96f-128">Property</span></span>|<span data-ttu-id="ab96f-129">型</span><span class="sxs-lookup"><span data-stu-id="ab96f-129">Type</span></span>|<span data-ttu-id="ab96f-130">説明</span><span class="sxs-lookup"><span data-stu-id="ab96f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab96f-131">id</span><span class="sxs-lookup"><span data-stu-id="ab96f-131">id</span></span>|<span data-ttu-id="ab96f-132">String</span><span class="sxs-lookup"><span data-stu-id="ab96f-132">String</span></span>|<span data-ttu-id="ab96f-133">リレーションシップエンティティ id。[MobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ab96f-133">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="ab96f-134">targetId</span><span class="sxs-lookup"><span data-stu-id="ab96f-134">targetId</span></span>|<span data-ttu-id="ab96f-135">String</span><span class="sxs-lookup"><span data-stu-id="ab96f-135">String</span></span>|<span data-ttu-id="ab96f-136">ターゲットの子モバイルアプリのアプリ id。[MobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ab96f-136">The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="ab96f-137">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="ab96f-137">targetDisplayName</span></span>|<span data-ttu-id="ab96f-138">String</span><span class="sxs-lookup"><span data-stu-id="ab96f-138">String</span></span>|<span data-ttu-id="ab96f-139">ターゲットの子モバイルアプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="ab96f-139">The target child mobile app's display name.</span></span> <span data-ttu-id="ab96f-140">[MobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ab96f-140">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="ab96f-141">dependencyType</span><span class="sxs-lookup"><span data-stu-id="ab96f-141">dependencyType</span></span>|[<span data-ttu-id="ab96f-142">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="ab96f-142">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="ab96f-143">親アプリと子アプリ間の依存関係の種類。</span><span class="sxs-lookup"><span data-stu-id="ab96f-143">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="ab96f-144">可能な値は、`detect`、`autoInstall` です。</span><span class="sxs-lookup"><span data-stu-id="ab96f-144">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="ab96f-145">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="ab96f-145">dependentAppCount</span></span>|<span data-ttu-id="ab96f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ab96f-146">Int32</span></span>|<span data-ttu-id="ab96f-147">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="ab96f-147">The total number of dependencies the child app has.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab96f-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ab96f-148">Relationships</span></span>
<span data-ttu-id="ab96f-149">なし</span><span class="sxs-lookup"><span data-stu-id="ab96f-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab96f-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ab96f-150">JSON Representation</span></span>
<span data-ttu-id="ab96f-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ab96f-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppDependency"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String",
  "dependencyType": "String",
  "dependentAppCount": 1024
}
```





