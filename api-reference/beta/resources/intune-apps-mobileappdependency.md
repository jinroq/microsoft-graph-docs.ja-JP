---
title: mobileAppDependency リソースの種類
description: 2つのモバイルアプリ間の依存関係の種類を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fbad9cc613ff97d0f627109316d58f9f0c8f1364
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31808844"
---
# <a name="mobileappdependency-resource-type"></a><span data-ttu-id="1a6a8-103">mobileAppDependency リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1a6a8-103">mobileAppDependency resource type</span></span>

> <span data-ttu-id="1a6a8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a6a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a6a8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1a6a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a6a8-106">2つのモバイルアプリ間の依存関係の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="1a6a8-106">Describes a dependency type between two mobile apps.</span></span>


<span data-ttu-id="1a6a8-107">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1a6a8-107">Inherits from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1a6a8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1a6a8-108">Methods</span></span>
|<span data-ttu-id="1a6a8-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="1a6a8-109">Method</span></span>|<span data-ttu-id="1a6a8-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1a6a8-110">Return Type</span></span>|<span data-ttu-id="1a6a8-111">説明</span><span class="sxs-lookup"><span data-stu-id="1a6a8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1a6a8-112">リスト mobileAppDependencies</span><span class="sxs-lookup"><span data-stu-id="1a6a8-112">List mobileAppDependencies</span></span>](../api/intune-apps-mobileappdependency-list.md)|<span data-ttu-id="1a6a8-113">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1a6a8-113">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md) collection</span></span>|<span data-ttu-id="1a6a8-114">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1a6a8-114">List properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) objects.</span></span>|
|[<span data-ttu-id="1a6a8-115">mobileAppDependency を取得する</span><span class="sxs-lookup"><span data-stu-id="1a6a8-115">Get mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-get.md)|[<span data-ttu-id="1a6a8-116">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="1a6a8-116">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="1a6a8-117">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1a6a8-117">Read properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|
|[<span data-ttu-id="1a6a8-118">mobileAppDependency を作成する</span><span class="sxs-lookup"><span data-stu-id="1a6a8-118">Create mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-create.md)|[<span data-ttu-id="1a6a8-119">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="1a6a8-119">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="1a6a8-120">新しい[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1a6a8-120">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|
|[<span data-ttu-id="1a6a8-121">mobileAppDependency の削除</span><span class="sxs-lookup"><span data-stu-id="1a6a8-121">Delete mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-delete.md)|<span data-ttu-id="1a6a8-122">なし</span><span class="sxs-lookup"><span data-stu-id="1a6a8-122">None</span></span>|<span data-ttu-id="1a6a8-123">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="1a6a8-123">Deletes a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>|
|[<span data-ttu-id="1a6a8-124">mobileAppDependency の更新</span><span class="sxs-lookup"><span data-stu-id="1a6a8-124">Update mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-update.md)|[<span data-ttu-id="1a6a8-125">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="1a6a8-125">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="1a6a8-126">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1a6a8-126">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1a6a8-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a6a8-127">Properties</span></span>
|<span data-ttu-id="1a6a8-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a6a8-128">Property</span></span>|<span data-ttu-id="1a6a8-129">型</span><span class="sxs-lookup"><span data-stu-id="1a6a8-129">Type</span></span>|<span data-ttu-id="1a6a8-130">説明</span><span class="sxs-lookup"><span data-stu-id="1a6a8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a6a8-131">id</span><span class="sxs-lookup"><span data-stu-id="1a6a8-131">id</span></span>|<span data-ttu-id="1a6a8-132">String</span><span class="sxs-lookup"><span data-stu-id="1a6a8-132">String</span></span>|<span data-ttu-id="1a6a8-133">リレーションシップエンティティ id。[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1a6a8-133">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="1a6a8-134">targetId</span><span class="sxs-lookup"><span data-stu-id="1a6a8-134">targetId</span></span>|<span data-ttu-id="1a6a8-135">文字列</span><span class="sxs-lookup"><span data-stu-id="1a6a8-135">String</span></span>|<span data-ttu-id="1a6a8-136">ターゲットの子モバイルアプリのアプリ id。[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1a6a8-136">The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="1a6a8-137">targetdisplayname</span><span class="sxs-lookup"><span data-stu-id="1a6a8-137">targetDisplayName</span></span>|<span data-ttu-id="1a6a8-138">文字列</span><span class="sxs-lookup"><span data-stu-id="1a6a8-138">String</span></span>|<span data-ttu-id="1a6a8-139">ターゲットの子モバイルアプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="1a6a8-139">The target child mobile app's display name.</span></span> <span data-ttu-id="1a6a8-140">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1a6a8-140">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="1a6a8-141">dependencytype</span><span class="sxs-lookup"><span data-stu-id="1a6a8-141">dependencyType</span></span>|[<span data-ttu-id="1a6a8-142">mobileAppDependecyType</span><span class="sxs-lookup"><span data-stu-id="1a6a8-142">mobileAppDependecyType</span></span>](../resources/intune-apps-mobileappdependecytype.md)|<span data-ttu-id="1a6a8-143">親アプリと子アプリ間の依存関係の種類。</span><span class="sxs-lookup"><span data-stu-id="1a6a8-143">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="1a6a8-144">可能な値は、`detect`、`autoInstall` です。</span><span class="sxs-lookup"><span data-stu-id="1a6a8-144">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="1a6a8-145">dependentappcount</span><span class="sxs-lookup"><span data-stu-id="1a6a8-145">dependentAppCount</span></span>|<span data-ttu-id="1a6a8-146">Int32</span><span class="sxs-lookup"><span data-stu-id="1a6a8-146">Int32</span></span>|<span data-ttu-id="1a6a8-147">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="1a6a8-147">The total number of dependencies the child app has.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a6a8-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1a6a8-148">Relationships</span></span>
<span data-ttu-id="1a6a8-149">なし</span><span class="sxs-lookup"><span data-stu-id="1a6a8-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a6a8-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1a6a8-150">JSON Representation</span></span>
<span data-ttu-id="1a6a8-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1a6a8-151">Here is a JSON representation of the resource.</span></span>
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





