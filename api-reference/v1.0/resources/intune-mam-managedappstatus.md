---
title: managedAppStatus リソースの種類
description: 組織のアプリ保護と構成の状態を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eef17c260d868b05280a41f14e797c928c432002
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037892"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="b31e2-103">managedAppStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b31e2-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="b31e2-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b31e2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b31e2-105">組織のアプリ保護と構成の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="b31e2-105">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="b31e2-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b31e2-106">Methods</span></span>
|<span data-ttu-id="b31e2-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b31e2-107">Method</span></span>|<span data-ttu-id="b31e2-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b31e2-108">Return Type</span></span>|<span data-ttu-id="b31e2-109">説明</span><span class="sxs-lookup"><span data-stu-id="b31e2-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b31e2-110">List managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="b31e2-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="b31e2-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b31e2-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="b31e2-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b31e2-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="b31e2-113">Get managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="b31e2-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="b31e2-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="b31e2-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="b31e2-115">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b31e2-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b31e2-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b31e2-116">Properties</span></span>
|<span data-ttu-id="b31e2-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b31e2-117">Property</span></span>|<span data-ttu-id="b31e2-118">型</span><span class="sxs-lookup"><span data-stu-id="b31e2-118">Type</span></span>|<span data-ttu-id="b31e2-119">説明</span><span class="sxs-lookup"><span data-stu-id="b31e2-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b31e2-120">displayName</span><span class="sxs-lookup"><span data-stu-id="b31e2-120">displayName</span></span>|<span data-ttu-id="b31e2-121">String</span><span class="sxs-lookup"><span data-stu-id="b31e2-121">String</span></span>|<span data-ttu-id="b31e2-122">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="b31e2-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="b31e2-123">id</span><span class="sxs-lookup"><span data-stu-id="b31e2-123">id</span></span>|<span data-ttu-id="b31e2-124">文字列</span><span class="sxs-lookup"><span data-stu-id="b31e2-124">String</span></span>|<span data-ttu-id="b31e2-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b31e2-125">Key of the entity.</span></span>|
|<span data-ttu-id="b31e2-126">version</span><span class="sxs-lookup"><span data-stu-id="b31e2-126">version</span></span>|<span data-ttu-id="b31e2-127">String</span><span class="sxs-lookup"><span data-stu-id="b31e2-127">String</span></span>|<span data-ttu-id="b31e2-128">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="b31e2-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b31e2-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b31e2-129">Relationships</span></span>
<span data-ttu-id="b31e2-130">なし</span><span class="sxs-lookup"><span data-stu-id="b31e2-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b31e2-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b31e2-131">JSON Representation</span></span>
<span data-ttu-id="b31e2-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b31e2-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



