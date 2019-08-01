---
title: managedAppStatusRaw リソースの種類
description: 組織アプリの保護と構成についての型指定されていない進捗レポートを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b21c15784409d9d7c373c954faecbc23426041b1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037878"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="869cf-103">managedAppStatusRaw リソースの種類</span><span class="sxs-lookup"><span data-stu-id="869cf-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="869cf-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="869cf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="869cf-105">組織アプリの保護と構成についての型指定されていない進捗レポートを表します。</span><span class="sxs-lookup"><span data-stu-id="869cf-105">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="869cf-106">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="869cf-106">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="869cf-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="869cf-107">Methods</span></span>
|<span data-ttu-id="869cf-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="869cf-108">Method</span></span>|<span data-ttu-id="869cf-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="869cf-109">Return Type</span></span>|<span data-ttu-id="869cf-110">説明</span><span class="sxs-lookup"><span data-stu-id="869cf-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="869cf-111">managedAppStatusRaws のリスト</span><span class="sxs-lookup"><span data-stu-id="869cf-111">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="869cf-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="869cf-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="869cf-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="869cf-113">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="869cf-114">managedAppStatusRaw の取得</span><span class="sxs-lookup"><span data-stu-id="869cf-114">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="869cf-115">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="869cf-115">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="869cf-116">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="869cf-116">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="869cf-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="869cf-117">Properties</span></span>
|<span data-ttu-id="869cf-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="869cf-118">Property</span></span>|<span data-ttu-id="869cf-119">型</span><span class="sxs-lookup"><span data-stu-id="869cf-119">Type</span></span>|<span data-ttu-id="869cf-120">説明</span><span class="sxs-lookup"><span data-stu-id="869cf-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="869cf-121">displayName</span><span class="sxs-lookup"><span data-stu-id="869cf-121">displayName</span></span>|<span data-ttu-id="869cf-122">String</span><span class="sxs-lookup"><span data-stu-id="869cf-122">String</span></span>|<span data-ttu-id="869cf-123">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="869cf-123">Friendly name of the status report.</span></span> <span data-ttu-id="869cf-124">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="869cf-124">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="869cf-125">id</span><span class="sxs-lookup"><span data-stu-id="869cf-125">id</span></span>|<span data-ttu-id="869cf-126">文字列</span><span class="sxs-lookup"><span data-stu-id="869cf-126">String</span></span>|<span data-ttu-id="869cf-127">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="869cf-127">Key of the entity.</span></span> <span data-ttu-id="869cf-128">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="869cf-128">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="869cf-129">version</span><span class="sxs-lookup"><span data-stu-id="869cf-129">version</span></span>|<span data-ttu-id="869cf-130">String</span><span class="sxs-lookup"><span data-stu-id="869cf-130">String</span></span>|<span data-ttu-id="869cf-131">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="869cf-131">Version of the entity.</span></span> <span data-ttu-id="869cf-132">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="869cf-132">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="869cf-133">content</span><span class="sxs-lookup"><span data-stu-id="869cf-133">content</span></span>|[<span data-ttu-id="869cf-134">Json</span><span class="sxs-lookup"><span data-stu-id="869cf-134">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="869cf-135">進捗レポートの内容。</span><span class="sxs-lookup"><span data-stu-id="869cf-135">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="869cf-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="869cf-136">Relationships</span></span>
<span data-ttu-id="869cf-137">なし</span><span class="sxs-lookup"><span data-stu-id="869cf-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="869cf-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="869cf-138">JSON Representation</span></span>
<span data-ttu-id="869cf-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="869cf-139">Here is a JSON representation of the resource.</span></span>
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



