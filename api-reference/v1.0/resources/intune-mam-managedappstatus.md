---
title: managedAppStatus リソースの種類
description: 組織のアプリ保護と構成の状態を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bc6982161e204a4f2e5cac38b62d351ab417482
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258864"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="807bc-103">managedAppStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="807bc-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="807bc-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="807bc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="807bc-105">組織のアプリ保護と構成の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="807bc-105">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="807bc-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="807bc-106">Methods</span></span>
|<span data-ttu-id="807bc-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="807bc-107">Method</span></span>|<span data-ttu-id="807bc-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="807bc-108">Return Type</span></span>|<span data-ttu-id="807bc-109">説明</span><span class="sxs-lookup"><span data-stu-id="807bc-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="807bc-110">List managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="807bc-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="807bc-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="807bc-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="807bc-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="807bc-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="807bc-113">Get managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="807bc-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="807bc-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="807bc-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="807bc-115">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="807bc-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="807bc-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="807bc-116">Properties</span></span>
|<span data-ttu-id="807bc-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="807bc-117">Property</span></span>|<span data-ttu-id="807bc-118">型</span><span class="sxs-lookup"><span data-stu-id="807bc-118">Type</span></span>|<span data-ttu-id="807bc-119">説明</span><span class="sxs-lookup"><span data-stu-id="807bc-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="807bc-120">displayName</span><span class="sxs-lookup"><span data-stu-id="807bc-120">displayName</span></span>|<span data-ttu-id="807bc-121">String</span><span class="sxs-lookup"><span data-stu-id="807bc-121">String</span></span>|<span data-ttu-id="807bc-122">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="807bc-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="807bc-123">id</span><span class="sxs-lookup"><span data-stu-id="807bc-123">id</span></span>|<span data-ttu-id="807bc-124">文字列</span><span class="sxs-lookup"><span data-stu-id="807bc-124">String</span></span>|<span data-ttu-id="807bc-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="807bc-125">Key of the entity.</span></span>|
|<span data-ttu-id="807bc-126">version</span><span class="sxs-lookup"><span data-stu-id="807bc-126">version</span></span>|<span data-ttu-id="807bc-127">String</span><span class="sxs-lookup"><span data-stu-id="807bc-127">String</span></span>|<span data-ttu-id="807bc-128">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="807bc-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="807bc-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="807bc-129">Relationships</span></span>
<span data-ttu-id="807bc-130">なし</span><span class="sxs-lookup"><span data-stu-id="807bc-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="807bc-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="807bc-131">JSON Representation</span></span>
<span data-ttu-id="807bc-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="807bc-132">Here is a JSON representation of the resource.</span></span>
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



