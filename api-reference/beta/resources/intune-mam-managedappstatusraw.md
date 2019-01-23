---
title: managedAppStatusRaw リソースの種類
description: 組織アプリの保護と構成についての型指定されていない進捗レポートを表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bfc7815e7f893294a72b88f67054702e1fb7347e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399263"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="b30d5-103">managedAppStatusRaw リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b30d5-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="b30d5-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b30d5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b30d5-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b30d5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b30d5-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b30d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b30d5-107">組織アプリの保護と構成についての型指定されていない進捗レポートを表します。</span><span class="sxs-lookup"><span data-stu-id="b30d5-107">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="b30d5-108">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b30d5-108">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b30d5-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="b30d5-109">Methods</span></span>
|<span data-ttu-id="b30d5-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="b30d5-110">Method</span></span>|<span data-ttu-id="b30d5-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b30d5-111">Return Type</span></span>|<span data-ttu-id="b30d5-112">説明</span><span class="sxs-lookup"><span data-stu-id="b30d5-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b30d5-113">managedAppStatusRaws のリスト</span><span class="sxs-lookup"><span data-stu-id="b30d5-113">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="b30d5-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b30d5-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="b30d5-115">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b30d5-115">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="b30d5-116">managedAppStatusRaw の取得</span><span class="sxs-lookup"><span data-stu-id="b30d5-116">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="b30d5-117">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="b30d5-117">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="b30d5-118">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b30d5-118">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b30d5-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b30d5-119">Properties</span></span>
|<span data-ttu-id="b30d5-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b30d5-120">Property</span></span>|<span data-ttu-id="b30d5-121">型</span><span class="sxs-lookup"><span data-stu-id="b30d5-121">Type</span></span>|<span data-ttu-id="b30d5-122">説明</span><span class="sxs-lookup"><span data-stu-id="b30d5-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b30d5-123">displayName</span><span class="sxs-lookup"><span data-stu-id="b30d5-123">displayName</span></span>|<span data-ttu-id="b30d5-124">String</span><span class="sxs-lookup"><span data-stu-id="b30d5-124">String</span></span>|<span data-ttu-id="b30d5-125">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="b30d5-125">Friendly name of the status report.</span></span> <span data-ttu-id="b30d5-126">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b30d5-126">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="b30d5-127">id</span><span class="sxs-lookup"><span data-stu-id="b30d5-127">id</span></span>|<span data-ttu-id="b30d5-128">String</span><span class="sxs-lookup"><span data-stu-id="b30d5-128">String</span></span>|<span data-ttu-id="b30d5-129">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b30d5-129">Key of the entity.</span></span> <span data-ttu-id="b30d5-130">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b30d5-130">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="b30d5-131">version</span><span class="sxs-lookup"><span data-stu-id="b30d5-131">version</span></span>|<span data-ttu-id="b30d5-132">String</span><span class="sxs-lookup"><span data-stu-id="b30d5-132">String</span></span>|<span data-ttu-id="b30d5-133">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="b30d5-133">Version of the entity.</span></span> <span data-ttu-id="b30d5-134">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b30d5-134">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="b30d5-135">content</span><span class="sxs-lookup"><span data-stu-id="b30d5-135">content</span></span>|[<span data-ttu-id="b30d5-136">Json</span><span class="sxs-lookup"><span data-stu-id="b30d5-136">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="b30d5-137">進捗レポートの内容。</span><span class="sxs-lookup"><span data-stu-id="b30d5-137">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b30d5-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b30d5-138">Relationships</span></span>
<span data-ttu-id="b30d5-139">なし</span><span class="sxs-lookup"><span data-stu-id="b30d5-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b30d5-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b30d5-140">JSON Representation</span></span>
<span data-ttu-id="b30d5-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b30d5-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```




