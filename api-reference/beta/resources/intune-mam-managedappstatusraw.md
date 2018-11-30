---
title: managedAppStatusRaw リソースの種類
description: 組織アプリの保護と構成についての型指定されていない進捗レポートを表します。
ms.openlocfilehash: ba2f398e54e27cb079dd575530d46a7bf287722d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066783"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="c16cd-103">managedAppStatusRaw リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c16cd-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="c16cd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c16cd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c16cd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c16cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c16cd-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c16cd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c16cd-107">組織アプリの保護と構成についての型指定されていない進捗レポートを表します。</span><span class="sxs-lookup"><span data-stu-id="c16cd-107">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="c16cd-108">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c16cd-108">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c16cd-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c16cd-109">Methods</span></span>
|<span data-ttu-id="c16cd-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="c16cd-110">Method</span></span>|<span data-ttu-id="c16cd-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c16cd-111">Return Type</span></span>|<span data-ttu-id="c16cd-112">説明</span><span class="sxs-lookup"><span data-stu-id="c16cd-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c16cd-113">managedAppStatusRaws のリスト</span><span class="sxs-lookup"><span data-stu-id="c16cd-113">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="c16cd-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c16cd-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="c16cd-115">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c16cd-115">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="c16cd-116">managedAppStatusRaw の取得</span><span class="sxs-lookup"><span data-stu-id="c16cd-116">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="c16cd-117">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="c16cd-117">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="c16cd-118">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c16cd-118">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c16cd-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c16cd-119">Properties</span></span>
|<span data-ttu-id="c16cd-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c16cd-120">Property</span></span>|<span data-ttu-id="c16cd-121">型</span><span class="sxs-lookup"><span data-stu-id="c16cd-121">Type</span></span>|<span data-ttu-id="c16cd-122">説明</span><span class="sxs-lookup"><span data-stu-id="c16cd-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c16cd-123">displayName</span><span class="sxs-lookup"><span data-stu-id="c16cd-123">displayName</span></span>|<span data-ttu-id="c16cd-124">String</span><span class="sxs-lookup"><span data-stu-id="c16cd-124">String</span></span>|<span data-ttu-id="c16cd-125">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="c16cd-125">Friendly name of the status report.</span></span> <span data-ttu-id="c16cd-126">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c16cd-126">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="c16cd-127">id</span><span class="sxs-lookup"><span data-stu-id="c16cd-127">id</span></span>|<span data-ttu-id="c16cd-128">String</span><span class="sxs-lookup"><span data-stu-id="c16cd-128">String</span></span>|<span data-ttu-id="c16cd-129">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c16cd-129">Key of the entity.</span></span> <span data-ttu-id="c16cd-130">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c16cd-130">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="c16cd-131">version</span><span class="sxs-lookup"><span data-stu-id="c16cd-131">version</span></span>|<span data-ttu-id="c16cd-132">String</span><span class="sxs-lookup"><span data-stu-id="c16cd-132">String</span></span>|<span data-ttu-id="c16cd-133">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="c16cd-133">Version of the entity.</span></span> <span data-ttu-id="c16cd-134">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c16cd-134">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="c16cd-135">content</span><span class="sxs-lookup"><span data-stu-id="c16cd-135">content</span></span>|[<span data-ttu-id="c16cd-136">Json</span><span class="sxs-lookup"><span data-stu-id="c16cd-136">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="c16cd-137">進捗レポートの内容。</span><span class="sxs-lookup"><span data-stu-id="c16cd-137">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c16cd-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c16cd-138">Relationships</span></span>
<span data-ttu-id="c16cd-139">なし</span><span class="sxs-lookup"><span data-stu-id="c16cd-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c16cd-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c16cd-140">JSON Representation</span></span>
<span data-ttu-id="c16cd-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c16cd-141">Here is a JSON representation of the resource.</span></span>
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





