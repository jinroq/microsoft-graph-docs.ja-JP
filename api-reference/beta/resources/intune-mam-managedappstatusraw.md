---
title: managedAppStatusRaw リソースの種類
description: 組織アプリの保護と構成についての型指定されていない進捗レポートを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f7c609c8ac1a228be588c5bdfe93cca7d42069da
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781541"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="65f12-103">managedAppStatusRaw リソースの種類</span><span class="sxs-lookup"><span data-stu-id="65f12-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="65f12-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65f12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65f12-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="65f12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65f12-106">組織アプリの保護と構成についての型指定されていない進捗レポートを表します。</span><span class="sxs-lookup"><span data-stu-id="65f12-106">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="65f12-107">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="65f12-107">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="65f12-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="65f12-108">Methods</span></span>
|<span data-ttu-id="65f12-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="65f12-109">Method</span></span>|<span data-ttu-id="65f12-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="65f12-110">Return Type</span></span>|<span data-ttu-id="65f12-111">説明</span><span class="sxs-lookup"><span data-stu-id="65f12-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="65f12-112">managedAppStatusRaws のリスト</span><span class="sxs-lookup"><span data-stu-id="65f12-112">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="65f12-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="65f12-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="65f12-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="65f12-114">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="65f12-115">Get managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="65f12-115">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="65f12-116">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="65f12-116">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="65f12-117">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="65f12-117">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="65f12-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65f12-118">Properties</span></span>
|<span data-ttu-id="65f12-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65f12-119">Property</span></span>|<span data-ttu-id="65f12-120">型</span><span class="sxs-lookup"><span data-stu-id="65f12-120">Type</span></span>|<span data-ttu-id="65f12-121">説明</span><span class="sxs-lookup"><span data-stu-id="65f12-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65f12-122">displayName</span><span class="sxs-lookup"><span data-stu-id="65f12-122">displayName</span></span>|<span data-ttu-id="65f12-123">String</span><span class="sxs-lookup"><span data-stu-id="65f12-123">String</span></span>|<span data-ttu-id="65f12-124">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="65f12-124">Friendly name of the status report.</span></span> <span data-ttu-id="65f12-125">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="65f12-125">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="65f12-126">id</span><span class="sxs-lookup"><span data-stu-id="65f12-126">id</span></span>|<span data-ttu-id="65f12-127">String</span><span class="sxs-lookup"><span data-stu-id="65f12-127">String</span></span>|<span data-ttu-id="65f12-128">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="65f12-128">Key of the entity.</span></span> <span data-ttu-id="65f12-129">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="65f12-129">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="65f12-130">version</span><span class="sxs-lookup"><span data-stu-id="65f12-130">version</span></span>|<span data-ttu-id="65f12-131">String</span><span class="sxs-lookup"><span data-stu-id="65f12-131">String</span></span>|<span data-ttu-id="65f12-132">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="65f12-132">Version of the entity.</span></span> <span data-ttu-id="65f12-133">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="65f12-133">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="65f12-134">content</span><span class="sxs-lookup"><span data-stu-id="65f12-134">content</span></span>|[<span data-ttu-id="65f12-135">Json</span><span class="sxs-lookup"><span data-stu-id="65f12-135">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="65f12-136">進捗レポートの内容。</span><span class="sxs-lookup"><span data-stu-id="65f12-136">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65f12-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="65f12-137">Relationships</span></span>
<span data-ttu-id="65f12-138">なし</span><span class="sxs-lookup"><span data-stu-id="65f12-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65f12-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="65f12-139">JSON Representation</span></span>
<span data-ttu-id="65f12-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="65f12-140">Here is a JSON representation of the resource.</span></span>
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





