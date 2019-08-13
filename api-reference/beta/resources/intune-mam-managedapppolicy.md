---
title: managedAppPolicy リソースの種類
description: ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ddc93ff13e55af15e86fbc72514b7b7daac81556
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332072"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="644a4-103">managedAppPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="644a4-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="644a4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="644a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="644a4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="644a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="644a4-106">ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。</span><span class="sxs-lookup"><span data-stu-id="644a4-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="644a4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="644a4-107">Methods</span></span>
|<span data-ttu-id="644a4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="644a4-108">Method</span></span>|<span data-ttu-id="644a4-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="644a4-109">Return Type</span></span>|<span data-ttu-id="644a4-110">説明</span><span class="sxs-lookup"><span data-stu-id="644a4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="644a4-111">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="644a4-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="644a4-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="644a4-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="644a4-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="644a4-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="644a4-114">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="644a4-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="644a4-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="644a4-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="644a4-116">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="644a4-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="644a4-117">targetApps アクション</span><span class="sxs-lookup"><span data-stu-id="644a4-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="644a4-118">なし</span><span class="sxs-lookup"><span data-stu-id="644a4-118">None</span></span>|<span data-ttu-id="644a4-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="644a4-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="644a4-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="644a4-120">Properties</span></span>
|<span data-ttu-id="644a4-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="644a4-121">Property</span></span>|<span data-ttu-id="644a4-122">型</span><span class="sxs-lookup"><span data-stu-id="644a4-122">Type</span></span>|<span data-ttu-id="644a4-123">説明</span><span class="sxs-lookup"><span data-stu-id="644a4-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="644a4-124">displayName</span><span class="sxs-lookup"><span data-stu-id="644a4-124">displayName</span></span>|<span data-ttu-id="644a4-125">String</span><span class="sxs-lookup"><span data-stu-id="644a4-125">String</span></span>|<span data-ttu-id="644a4-126">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="644a4-126">Policy display name.</span></span>|
|<span data-ttu-id="644a4-127">description</span><span class="sxs-lookup"><span data-stu-id="644a4-127">description</span></span>|<span data-ttu-id="644a4-128">String</span><span class="sxs-lookup"><span data-stu-id="644a4-128">String</span></span>|<span data-ttu-id="644a4-129">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="644a4-129">The policy's description.</span></span>|
|<span data-ttu-id="644a4-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="644a4-130">createdDateTime</span></span>|<span data-ttu-id="644a4-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="644a4-131">DateTimeOffset</span></span>|<span data-ttu-id="644a4-132">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="644a4-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="644a4-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="644a4-133">lastModifiedDateTime</span></span>|<span data-ttu-id="644a4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="644a4-134">DateTimeOffset</span></span>|<span data-ttu-id="644a4-135">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="644a4-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="644a4-136">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="644a4-136">roleScopeTagIds</span></span>|<span data-ttu-id="644a4-137">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="644a4-137">String collection</span></span>|<span data-ttu-id="644a4-138">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="644a4-138">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="644a4-139">id</span><span class="sxs-lookup"><span data-stu-id="644a4-139">id</span></span>|<span data-ttu-id="644a4-140">文字列</span><span class="sxs-lookup"><span data-stu-id="644a4-140">String</span></span>|<span data-ttu-id="644a4-141">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="644a4-141">Key of the entity.</span></span>|
|<span data-ttu-id="644a4-142">version</span><span class="sxs-lookup"><span data-stu-id="644a4-142">version</span></span>|<span data-ttu-id="644a4-143">String</span><span class="sxs-lookup"><span data-stu-id="644a4-143">String</span></span>|<span data-ttu-id="644a4-144">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="644a4-144">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="644a4-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="644a4-145">Relationships</span></span>
<span data-ttu-id="644a4-146">なし</span><span class="sxs-lookup"><span data-stu-id="644a4-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="644a4-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="644a4-147">JSON Representation</span></span>
<span data-ttu-id="644a4-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="644a4-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String"
}
```



