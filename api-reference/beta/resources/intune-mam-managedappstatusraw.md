---
title: managedAppStatusRaw リソースの種類
description: 組織アプリの保護と構成についての型指定されていない進捗レポートを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f7c609c8ac1a228be588c5bdfe93cca7d42069da
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551709"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="9f12a-103">managedAppStatusRaw リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9f12a-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="9f12a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f12a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f12a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9f12a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f12a-106">組織アプリの保護と構成についての型指定されていない進捗レポートを表します。</span><span class="sxs-lookup"><span data-stu-id="9f12a-106">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="9f12a-107">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f12a-107">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="9f12a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="9f12a-108">Methods</span></span>
|<span data-ttu-id="9f12a-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="9f12a-109">Method</span></span>|<span data-ttu-id="9f12a-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9f12a-110">Return Type</span></span>|<span data-ttu-id="9f12a-111">説明</span><span class="sxs-lookup"><span data-stu-id="9f12a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9f12a-112">managedAppStatusRaws のリスト</span><span class="sxs-lookup"><span data-stu-id="9f12a-112">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="9f12a-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9f12a-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="9f12a-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="9f12a-114">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="9f12a-115">managedAppStatusRaw の取得</span><span class="sxs-lookup"><span data-stu-id="9f12a-115">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="9f12a-116">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="9f12a-116">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="9f12a-117">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9f12a-117">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9f12a-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f12a-118">Properties</span></span>
|<span data-ttu-id="9f12a-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f12a-119">Property</span></span>|<span data-ttu-id="9f12a-120">型</span><span class="sxs-lookup"><span data-stu-id="9f12a-120">Type</span></span>|<span data-ttu-id="9f12a-121">説明</span><span class="sxs-lookup"><span data-stu-id="9f12a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f12a-122">displayName</span><span class="sxs-lookup"><span data-stu-id="9f12a-122">displayName</span></span>|<span data-ttu-id="9f12a-123">String</span><span class="sxs-lookup"><span data-stu-id="9f12a-123">String</span></span>|<span data-ttu-id="9f12a-124">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="9f12a-124">Friendly name of the status report.</span></span> <span data-ttu-id="9f12a-125">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f12a-125">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="9f12a-126">id</span><span class="sxs-lookup"><span data-stu-id="9f12a-126">id</span></span>|<span data-ttu-id="9f12a-127">String</span><span class="sxs-lookup"><span data-stu-id="9f12a-127">String</span></span>|<span data-ttu-id="9f12a-128">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9f12a-128">Key of the entity.</span></span> <span data-ttu-id="9f12a-129">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f12a-129">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="9f12a-130">version</span><span class="sxs-lookup"><span data-stu-id="9f12a-130">version</span></span>|<span data-ttu-id="9f12a-131">String</span><span class="sxs-lookup"><span data-stu-id="9f12a-131">String</span></span>|<span data-ttu-id="9f12a-132">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="9f12a-132">Version of the entity.</span></span> <span data-ttu-id="9f12a-133">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9f12a-133">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="9f12a-134">content</span><span class="sxs-lookup"><span data-stu-id="9f12a-134">content</span></span>|[<span data-ttu-id="9f12a-135">Json</span><span class="sxs-lookup"><span data-stu-id="9f12a-135">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="9f12a-136">進捗レポートの内容。</span><span class="sxs-lookup"><span data-stu-id="9f12a-136">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f12a-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9f12a-137">Relationships</span></span>
<span data-ttu-id="9f12a-138">なし</span><span class="sxs-lookup"><span data-stu-id="9f12a-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f12a-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f12a-139">JSON Representation</span></span>
<span data-ttu-id="9f12a-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9f12a-140">Here is a JSON representation of the resource.</span></span>
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





