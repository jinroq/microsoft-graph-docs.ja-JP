---
title: managedMobileApp リソースの種類
description: アプリ展開の識別子。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: acd69164becf0b0199c9ddc845b8e45afb4420a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838417"
---
# <a name="managedmobileapp-resource-type"></a><span data-ttu-id="b4fa1-103">managedMobileApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b4fa1-103">managedMobileApp resource type</span></span>

> <span data-ttu-id="b4fa1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b4fa1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4fa1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4fa1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4fa1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b4fa1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4fa1-107">アプリ展開の識別子。</span><span class="sxs-lookup"><span data-stu-id="b4fa1-107">The identifier for the deployment an app.</span></span>
## <a name="methods"></a><span data-ttu-id="b4fa1-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b4fa1-108">Methods</span></span>
|<span data-ttu-id="b4fa1-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="b4fa1-109">Method</span></span>|<span data-ttu-id="b4fa1-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b4fa1-110">Return Type</span></span>|<span data-ttu-id="b4fa1-111">説明</span><span class="sxs-lookup"><span data-stu-id="b4fa1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b4fa1-112">List managedMobileApps</span><span class="sxs-lookup"><span data-stu-id="b4fa1-112">List managedMobileApps</span></span>](../api/intune-mam-managedmobileapp-list.md)|<span data-ttu-id="b4fa1-113">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b4fa1-113">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="b4fa1-114">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b4fa1-114">List properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects.</span></span>|
|[<span data-ttu-id="b4fa1-115">Get managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="b4fa1-115">Get managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-get.md)|[<span data-ttu-id="b4fa1-116">managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="b4fa1-116">managedMobileApp</span></span>](../resources/intune-mam-managedmobileapp.md)|<span data-ttu-id="b4fa1-117">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b4fa1-117">Read properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>|
|[<span data-ttu-id="b4fa1-118">Create managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="b4fa1-118">Create managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-create.md)|[<span data-ttu-id="b4fa1-119">managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="b4fa1-119">managedMobileApp</span></span>](../resources/intune-mam-managedmobileapp.md)|<span data-ttu-id="b4fa1-120">新しい [managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b4fa1-120">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>|
|[<span data-ttu-id="b4fa1-121">Delete managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="b4fa1-121">Delete managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-delete.md)|<span data-ttu-id="b4fa1-122">なし</span><span class="sxs-lookup"><span data-stu-id="b4fa1-122">None</span></span>|<span data-ttu-id="b4fa1-123">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="b4fa1-123">Deletes a [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>|
|[<span data-ttu-id="b4fa1-124">Update managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="b4fa1-124">Update managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-update.md)|[<span data-ttu-id="b4fa1-125">managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="b4fa1-125">managedMobileApp</span></span>](../resources/intune-mam-managedmobileapp.md)|<span data-ttu-id="b4fa1-126">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b4fa1-126">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b4fa1-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4fa1-127">Properties</span></span>
|<span data-ttu-id="b4fa1-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4fa1-128">Property</span></span>|<span data-ttu-id="b4fa1-129">種類</span><span class="sxs-lookup"><span data-stu-id="b4fa1-129">Type</span></span>|<span data-ttu-id="b4fa1-130">説明</span><span class="sxs-lookup"><span data-stu-id="b4fa1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4fa1-131">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b4fa1-131">mobileAppIdentifier</span></span>|[<span data-ttu-id="b4fa1-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b4fa1-132">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="b4fa1-133">対象のオペレーティング システムの種類のアプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="b4fa1-133">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="b4fa1-134">id</span><span class="sxs-lookup"><span data-stu-id="b4fa1-134">id</span></span>|<span data-ttu-id="b4fa1-135">String</span><span class="sxs-lookup"><span data-stu-id="b4fa1-135">String</span></span>|<span data-ttu-id="b4fa1-136">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b4fa1-136">Key of the entity.</span></span>|
|<span data-ttu-id="b4fa1-137">version</span><span class="sxs-lookup"><span data-stu-id="b4fa1-137">version</span></span>|<span data-ttu-id="b4fa1-138">String</span><span class="sxs-lookup"><span data-stu-id="b4fa1-138">String</span></span>|<span data-ttu-id="b4fa1-139">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="b4fa1-139">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4fa1-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b4fa1-140">Relationships</span></span>
<span data-ttu-id="b4fa1-141">なし</span><span class="sxs-lookup"><span data-stu-id="b4fa1-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b4fa1-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b4fa1-142">JSON Representation</span></span>
<span data-ttu-id="b4fa1-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b4fa1-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedMobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```





