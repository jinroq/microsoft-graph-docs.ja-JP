---
title: managedAppPolicy リソースの種類
description: ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bc3047eed950cc547f47fa45fbf609e86ba025bb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998381"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="a5e43-103">managedAppPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a5e43-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="a5e43-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5e43-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5e43-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a5e43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5e43-106">ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。</span><span class="sxs-lookup"><span data-stu-id="a5e43-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="a5e43-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a5e43-107">Methods</span></span>
|<span data-ttu-id="a5e43-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a5e43-108">Method</span></span>|<span data-ttu-id="a5e43-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a5e43-109">Return Type</span></span>|<span data-ttu-id="a5e43-110">説明</span><span class="sxs-lookup"><span data-stu-id="a5e43-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a5e43-111">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="a5e43-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="a5e43-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a5e43-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="a5e43-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a5e43-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="a5e43-114">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="a5e43-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="a5e43-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="a5e43-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="a5e43-116">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a5e43-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="a5e43-117">targetApps アクション</span><span class="sxs-lookup"><span data-stu-id="a5e43-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="a5e43-118">なし</span><span class="sxs-lookup"><span data-stu-id="a5e43-118">None</span></span>|<span data-ttu-id="a5e43-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a5e43-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a5e43-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5e43-120">Properties</span></span>
|<span data-ttu-id="a5e43-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5e43-121">Property</span></span>|<span data-ttu-id="a5e43-122">型</span><span class="sxs-lookup"><span data-stu-id="a5e43-122">Type</span></span>|<span data-ttu-id="a5e43-123">説明</span><span class="sxs-lookup"><span data-stu-id="a5e43-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5e43-124">displayName</span><span class="sxs-lookup"><span data-stu-id="a5e43-124">displayName</span></span>|<span data-ttu-id="a5e43-125">String</span><span class="sxs-lookup"><span data-stu-id="a5e43-125">String</span></span>|<span data-ttu-id="a5e43-126">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="a5e43-126">Policy display name.</span></span>|
|<span data-ttu-id="a5e43-127">description</span><span class="sxs-lookup"><span data-stu-id="a5e43-127">description</span></span>|<span data-ttu-id="a5e43-128">String</span><span class="sxs-lookup"><span data-stu-id="a5e43-128">String</span></span>|<span data-ttu-id="a5e43-129">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="a5e43-129">The policy's description.</span></span>|
|<span data-ttu-id="a5e43-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a5e43-130">createdDateTime</span></span>|<span data-ttu-id="a5e43-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5e43-131">DateTimeOffset</span></span>|<span data-ttu-id="a5e43-132">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="a5e43-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="a5e43-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5e43-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a5e43-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5e43-134">DateTimeOffset</span></span>|<span data-ttu-id="a5e43-135">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="a5e43-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="a5e43-136">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a5e43-136">roleScopeTagIds</span></span>|<span data-ttu-id="a5e43-137">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="a5e43-137">String collection</span></span>|<span data-ttu-id="a5e43-138">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="a5e43-138">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="a5e43-139">id</span><span class="sxs-lookup"><span data-stu-id="a5e43-139">id</span></span>|<span data-ttu-id="a5e43-140">文字列</span><span class="sxs-lookup"><span data-stu-id="a5e43-140">String</span></span>|<span data-ttu-id="a5e43-141">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a5e43-141">Key of the entity.</span></span>|
|<span data-ttu-id="a5e43-142">version</span><span class="sxs-lookup"><span data-stu-id="a5e43-142">version</span></span>|<span data-ttu-id="a5e43-143">String</span><span class="sxs-lookup"><span data-stu-id="a5e43-143">String</span></span>|<span data-ttu-id="a5e43-144">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="a5e43-144">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5e43-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a5e43-145">Relationships</span></span>
<span data-ttu-id="a5e43-146">なし</span><span class="sxs-lookup"><span data-stu-id="a5e43-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5e43-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a5e43-147">JSON Representation</span></span>
<span data-ttu-id="a5e43-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a5e43-148">Here is a JSON representation of the resource.</span></span>
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





