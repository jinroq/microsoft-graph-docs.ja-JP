---
title: managedAppStatusRaw リソースの種類
description: 組織アプリの保護と構成についての型指定されていない進捗レポートを表します。
author: tfitzmac
ms.openlocfilehash: 9b7c957451e3fc92ad79ef10433e26bf39fd1c48
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331928"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="7df56-103">managedAppStatusRaw リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7df56-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="7df56-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7df56-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7df56-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7df56-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7df56-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7df56-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7df56-107">組織アプリの保護と構成についての型指定されていない進捗レポートを表します。</span><span class="sxs-lookup"><span data-stu-id="7df56-107">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="7df56-108">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7df56-108">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="7df56-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="7df56-109">Methods</span></span>
|<span data-ttu-id="7df56-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="7df56-110">Method</span></span>|<span data-ttu-id="7df56-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7df56-111">Return Type</span></span>|<span data-ttu-id="7df56-112">説明</span><span class="sxs-lookup"><span data-stu-id="7df56-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7df56-113">managedAppStatusRaws のリスト</span><span class="sxs-lookup"><span data-stu-id="7df56-113">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="7df56-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7df56-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="7df56-115">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7df56-115">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="7df56-116">managedAppStatusRaw の取得</span><span class="sxs-lookup"><span data-stu-id="7df56-116">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="7df56-117">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="7df56-117">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="7df56-118">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7df56-118">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7df56-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7df56-119">Properties</span></span>
|<span data-ttu-id="7df56-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7df56-120">Property</span></span>|<span data-ttu-id="7df56-121">種類</span><span class="sxs-lookup"><span data-stu-id="7df56-121">Type</span></span>|<span data-ttu-id="7df56-122">説明</span><span class="sxs-lookup"><span data-stu-id="7df56-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7df56-123">displayName</span><span class="sxs-lookup"><span data-stu-id="7df56-123">displayName</span></span>|<span data-ttu-id="7df56-124">String</span><span class="sxs-lookup"><span data-stu-id="7df56-124">String</span></span>|<span data-ttu-id="7df56-125">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="7df56-125">Friendly name of the status report.</span></span> <span data-ttu-id="7df56-126">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7df56-126">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="7df56-127">id</span><span class="sxs-lookup"><span data-stu-id="7df56-127">id</span></span>|<span data-ttu-id="7df56-128">String</span><span class="sxs-lookup"><span data-stu-id="7df56-128">String</span></span>|<span data-ttu-id="7df56-129">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7df56-129">Key of the entity.</span></span> <span data-ttu-id="7df56-130">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7df56-130">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="7df56-131">version</span><span class="sxs-lookup"><span data-stu-id="7df56-131">version</span></span>|<span data-ttu-id="7df56-132">String</span><span class="sxs-lookup"><span data-stu-id="7df56-132">String</span></span>|<span data-ttu-id="7df56-133">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="7df56-133">Version of the entity.</span></span> <span data-ttu-id="7df56-134">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7df56-134">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="7df56-135">content</span><span class="sxs-lookup"><span data-stu-id="7df56-135">content</span></span>|[<span data-ttu-id="7df56-136">Json</span><span class="sxs-lookup"><span data-stu-id="7df56-136">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="7df56-137">進捗レポートの内容。</span><span class="sxs-lookup"><span data-stu-id="7df56-137">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7df56-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7df56-138">Relationships</span></span>
<span data-ttu-id="7df56-139">なし</span><span class="sxs-lookup"><span data-stu-id="7df56-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7df56-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7df56-140">JSON Representation</span></span>
<span data-ttu-id="7df56-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7df56-141">Here is a JSON representation of the resource.</span></span>
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





