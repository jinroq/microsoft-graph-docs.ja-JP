---
title: managedAppStatusRaw リソースの種類
description: 組織アプリの保護と構成についての型指定されていない進捗レポートを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 34c70a268c3940843759844c27de7f31bfab002e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154195"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="3f955-103">managedAppStatusRaw リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3f955-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="3f955-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f955-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f955-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3f955-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f955-106">組織アプリの保護と構成についての型指定されていない進捗レポートを表します。</span><span class="sxs-lookup"><span data-stu-id="3f955-106">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="3f955-107">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f955-107">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="3f955-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="3f955-108">Methods</span></span>
|<span data-ttu-id="3f955-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="3f955-109">Method</span></span>|<span data-ttu-id="3f955-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3f955-110">Return Type</span></span>|<span data-ttu-id="3f955-111">説明</span><span class="sxs-lookup"><span data-stu-id="3f955-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3f955-112">managedAppStatusRaws のリスト</span><span class="sxs-lookup"><span data-stu-id="3f955-112">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="3f955-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3f955-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="3f955-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="3f955-114">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="3f955-115">managedAppStatusRaw の取得</span><span class="sxs-lookup"><span data-stu-id="3f955-115">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="3f955-116">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="3f955-116">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="3f955-117">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3f955-117">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3f955-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f955-118">Properties</span></span>
|<span data-ttu-id="3f955-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f955-119">Property</span></span>|<span data-ttu-id="3f955-120">型</span><span class="sxs-lookup"><span data-stu-id="3f955-120">Type</span></span>|<span data-ttu-id="3f955-121">説明</span><span class="sxs-lookup"><span data-stu-id="3f955-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f955-122">displayName</span><span class="sxs-lookup"><span data-stu-id="3f955-122">displayName</span></span>|<span data-ttu-id="3f955-123">String</span><span class="sxs-lookup"><span data-stu-id="3f955-123">String</span></span>|<span data-ttu-id="3f955-124">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="3f955-124">Friendly name of the status report.</span></span> <span data-ttu-id="3f955-125">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f955-125">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="3f955-126">id</span><span class="sxs-lookup"><span data-stu-id="3f955-126">id</span></span>|<span data-ttu-id="3f955-127">文字列</span><span class="sxs-lookup"><span data-stu-id="3f955-127">String</span></span>|<span data-ttu-id="3f955-128">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3f955-128">Key of the entity.</span></span> <span data-ttu-id="3f955-129">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f955-129">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="3f955-130">version</span><span class="sxs-lookup"><span data-stu-id="3f955-130">version</span></span>|<span data-ttu-id="3f955-131">String</span><span class="sxs-lookup"><span data-stu-id="3f955-131">String</span></span>|<span data-ttu-id="3f955-132">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="3f955-132">Version of the entity.</span></span> <span data-ttu-id="3f955-133">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3f955-133">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="3f955-134">content</span><span class="sxs-lookup"><span data-stu-id="3f955-134">content</span></span>|[<span data-ttu-id="3f955-135">Json</span><span class="sxs-lookup"><span data-stu-id="3f955-135">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="3f955-136">進捗レポートの内容。</span><span class="sxs-lookup"><span data-stu-id="3f955-136">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f955-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3f955-137">Relationships</span></span>
<span data-ttu-id="3f955-138">なし</span><span class="sxs-lookup"><span data-stu-id="3f955-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f955-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3f955-139">JSON Representation</span></span>
<span data-ttu-id="3f955-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3f955-140">Here is a JSON representation of the resource.</span></span>
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




