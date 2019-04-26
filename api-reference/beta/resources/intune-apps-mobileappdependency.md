---
title: mobileAppDependency リソースの種類
description: 2つのモバイルアプリ間の依存関係の種類を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fbad9cc613ff97d0f627109316d58f9f0c8f1364
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551758"
---
# <a name="mobileappdependency-resource-type"></a><span data-ttu-id="42a98-103">mobileAppDependency リソースの種類</span><span class="sxs-lookup"><span data-stu-id="42a98-103">mobileAppDependency resource type</span></span>

> <span data-ttu-id="42a98-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42a98-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42a98-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="42a98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42a98-106">2つのモバイルアプリ間の依存関係の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="42a98-106">Describes a dependency type between two mobile apps.</span></span>


<span data-ttu-id="42a98-107">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="42a98-107">Inherits from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>

## <a name="methods"></a><span data-ttu-id="42a98-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="42a98-108">Methods</span></span>
|<span data-ttu-id="42a98-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="42a98-109">Method</span></span>|<span data-ttu-id="42a98-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="42a98-110">Return Type</span></span>|<span data-ttu-id="42a98-111">説明</span><span class="sxs-lookup"><span data-stu-id="42a98-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="42a98-112">リスト mobileAppDependencies</span><span class="sxs-lookup"><span data-stu-id="42a98-112">List mobileAppDependencies</span></span>](../api/intune-apps-mobileappdependency-list.md)|<span data-ttu-id="42a98-113">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="42a98-113">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md) collection</span></span>|<span data-ttu-id="42a98-114">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="42a98-114">List properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) objects.</span></span>|
|[<span data-ttu-id="42a98-115">mobileAppDependency を取得する</span><span class="sxs-lookup"><span data-stu-id="42a98-115">Get mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-get.md)|[<span data-ttu-id="42a98-116">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="42a98-116">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="42a98-117">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="42a98-117">Read properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|
|[<span data-ttu-id="42a98-118">mobileAppDependency を作成する</span><span class="sxs-lookup"><span data-stu-id="42a98-118">Create mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-create.md)|[<span data-ttu-id="42a98-119">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="42a98-119">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="42a98-120">新しい[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="42a98-120">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|
|[<span data-ttu-id="42a98-121">mobileAppDependency の削除</span><span class="sxs-lookup"><span data-stu-id="42a98-121">Delete mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-delete.md)|<span data-ttu-id="42a98-122">なし</span><span class="sxs-lookup"><span data-stu-id="42a98-122">None</span></span>|<span data-ttu-id="42a98-123">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="42a98-123">Deletes a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>|
|[<span data-ttu-id="42a98-124">mobileAppDependency の更新</span><span class="sxs-lookup"><span data-stu-id="42a98-124">Update mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-update.md)|[<span data-ttu-id="42a98-125">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="42a98-125">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="42a98-126">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="42a98-126">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="42a98-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42a98-127">Properties</span></span>
|<span data-ttu-id="42a98-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42a98-128">Property</span></span>|<span data-ttu-id="42a98-129">型</span><span class="sxs-lookup"><span data-stu-id="42a98-129">Type</span></span>|<span data-ttu-id="42a98-130">説明</span><span class="sxs-lookup"><span data-stu-id="42a98-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42a98-131">id</span><span class="sxs-lookup"><span data-stu-id="42a98-131">id</span></span>|<span data-ttu-id="42a98-132">String</span><span class="sxs-lookup"><span data-stu-id="42a98-132">String</span></span>|<span data-ttu-id="42a98-133">リレーションシップエンティティ id。[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="42a98-133">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="42a98-134">targetId</span><span class="sxs-lookup"><span data-stu-id="42a98-134">targetId</span></span>|<span data-ttu-id="42a98-135">String</span><span class="sxs-lookup"><span data-stu-id="42a98-135">String</span></span>|<span data-ttu-id="42a98-136">ターゲットの子モバイルアプリのアプリ id。[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="42a98-136">The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="42a98-137">targetdisplayname</span><span class="sxs-lookup"><span data-stu-id="42a98-137">targetDisplayName</span></span>|<span data-ttu-id="42a98-138">String</span><span class="sxs-lookup"><span data-stu-id="42a98-138">String</span></span>|<span data-ttu-id="42a98-139">ターゲットの子モバイルアプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="42a98-139">The target child mobile app's display name.</span></span> <span data-ttu-id="42a98-140">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="42a98-140">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="42a98-141">dependencytype</span><span class="sxs-lookup"><span data-stu-id="42a98-141">dependencyType</span></span>|[<span data-ttu-id="42a98-142">mobileAppDependecyType</span><span class="sxs-lookup"><span data-stu-id="42a98-142">mobileAppDependecyType</span></span>](../resources/intune-apps-mobileappdependecytype.md)|<span data-ttu-id="42a98-143">親アプリと子アプリ間の依存関係の種類。</span><span class="sxs-lookup"><span data-stu-id="42a98-143">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="42a98-144">可能な値は、`detect`、`autoInstall` です。</span><span class="sxs-lookup"><span data-stu-id="42a98-144">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="42a98-145">dependentappcount</span><span class="sxs-lookup"><span data-stu-id="42a98-145">dependentAppCount</span></span>|<span data-ttu-id="42a98-146">Int32</span><span class="sxs-lookup"><span data-stu-id="42a98-146">Int32</span></span>|<span data-ttu-id="42a98-147">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="42a98-147">The total number of dependencies the child app has.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42a98-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="42a98-148">Relationships</span></span>
<span data-ttu-id="42a98-149">なし</span><span class="sxs-lookup"><span data-stu-id="42a98-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42a98-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="42a98-150">JSON Representation</span></span>
<span data-ttu-id="42a98-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="42a98-151">Here is a JSON representation of the resource.</span></span>
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





