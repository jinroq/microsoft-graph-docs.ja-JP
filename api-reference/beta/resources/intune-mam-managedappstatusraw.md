---
title: managedAppStatusRaw リソースの種類
description: 組織アプリの保護と構成についての型指定されていない進捗レポートを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 980521b7f58338501d69ec83a6fc68b591c8688c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967910"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="c18c1-103">managedAppStatusRaw リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c18c1-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="c18c1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c18c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c18c1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c18c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c18c1-106">組織アプリの保護と構成についての型指定されていない進捗レポートを表します。</span><span class="sxs-lookup"><span data-stu-id="c18c1-106">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="c18c1-107">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c18c1-107">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c18c1-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c18c1-108">Methods</span></span>
|<span data-ttu-id="c18c1-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c18c1-109">Method</span></span>|<span data-ttu-id="c18c1-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c18c1-110">Return Type</span></span>|<span data-ttu-id="c18c1-111">説明</span><span class="sxs-lookup"><span data-stu-id="c18c1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c18c1-112">managedAppStatusRaws のリスト</span><span class="sxs-lookup"><span data-stu-id="c18c1-112">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="c18c1-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c18c1-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="c18c1-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c18c1-114">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="c18c1-115">managedAppStatusRaw の取得</span><span class="sxs-lookup"><span data-stu-id="c18c1-115">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="c18c1-116">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="c18c1-116">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="c18c1-117">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c18c1-117">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c18c1-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c18c1-118">Properties</span></span>
|<span data-ttu-id="c18c1-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c18c1-119">Property</span></span>|<span data-ttu-id="c18c1-120">型</span><span class="sxs-lookup"><span data-stu-id="c18c1-120">Type</span></span>|<span data-ttu-id="c18c1-121">説明</span><span class="sxs-lookup"><span data-stu-id="c18c1-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c18c1-122">displayName</span><span class="sxs-lookup"><span data-stu-id="c18c1-122">displayName</span></span>|<span data-ttu-id="c18c1-123">String</span><span class="sxs-lookup"><span data-stu-id="c18c1-123">String</span></span>|<span data-ttu-id="c18c1-124">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="c18c1-124">Friendly name of the status report.</span></span> <span data-ttu-id="c18c1-125">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c18c1-125">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="c18c1-126">id</span><span class="sxs-lookup"><span data-stu-id="c18c1-126">id</span></span>|<span data-ttu-id="c18c1-127">文字列</span><span class="sxs-lookup"><span data-stu-id="c18c1-127">String</span></span>|<span data-ttu-id="c18c1-128">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c18c1-128">Key of the entity.</span></span> <span data-ttu-id="c18c1-129">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c18c1-129">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="c18c1-130">version</span><span class="sxs-lookup"><span data-stu-id="c18c1-130">version</span></span>|<span data-ttu-id="c18c1-131">String</span><span class="sxs-lookup"><span data-stu-id="c18c1-131">String</span></span>|<span data-ttu-id="c18c1-132">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="c18c1-132">Version of the entity.</span></span> <span data-ttu-id="c18c1-133">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c18c1-133">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="c18c1-134">content</span><span class="sxs-lookup"><span data-stu-id="c18c1-134">content</span></span>|[<span data-ttu-id="c18c1-135">Json</span><span class="sxs-lookup"><span data-stu-id="c18c1-135">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="c18c1-136">進捗レポートの内容。</span><span class="sxs-lookup"><span data-stu-id="c18c1-136">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c18c1-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c18c1-137">Relationships</span></span>
<span data-ttu-id="c18c1-138">なし</span><span class="sxs-lookup"><span data-stu-id="c18c1-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c18c1-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c18c1-139">JSON Representation</span></span>
<span data-ttu-id="c18c1-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c18c1-140">Here is a JSON representation of the resource.</span></span>
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





