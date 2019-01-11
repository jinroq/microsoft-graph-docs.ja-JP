---
title: managedAppStatus リソースの種類
description: 組織のアプリ保護と構成の状態を表します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 05b2117f441fd60f92970cc506245d177a618fce
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840748"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="8b03c-103">managedAppStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8b03c-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="8b03c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8b03c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b03c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b03c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b03c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8b03c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b03c-107">組織のアプリ保護と構成の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="8b03c-107">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="8b03c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8b03c-108">Methods</span></span>
|<span data-ttu-id="8b03c-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="8b03c-109">Method</span></span>|<span data-ttu-id="8b03c-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8b03c-110">Return Type</span></span>|<span data-ttu-id="8b03c-111">説明</span><span class="sxs-lookup"><span data-stu-id="8b03c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8b03c-112">List managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="8b03c-112">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="8b03c-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8b03c-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="8b03c-114">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8b03c-114">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="8b03c-115">Get managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="8b03c-115">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="8b03c-116">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="8b03c-116">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="8b03c-117">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8b03c-117">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8b03c-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b03c-118">Properties</span></span>
|<span data-ttu-id="8b03c-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b03c-119">Property</span></span>|<span data-ttu-id="8b03c-120">種類</span><span class="sxs-lookup"><span data-stu-id="8b03c-120">Type</span></span>|<span data-ttu-id="8b03c-121">説明</span><span class="sxs-lookup"><span data-stu-id="8b03c-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b03c-122">displayName</span><span class="sxs-lookup"><span data-stu-id="8b03c-122">displayName</span></span>|<span data-ttu-id="8b03c-123">String</span><span class="sxs-lookup"><span data-stu-id="8b03c-123">String</span></span>|<span data-ttu-id="8b03c-124">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="8b03c-124">Friendly name of the status report.</span></span>|
|<span data-ttu-id="8b03c-125">id</span><span class="sxs-lookup"><span data-stu-id="8b03c-125">id</span></span>|<span data-ttu-id="8b03c-126">String</span><span class="sxs-lookup"><span data-stu-id="8b03c-126">String</span></span>|<span data-ttu-id="8b03c-127">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8b03c-127">Key of the entity.</span></span>|
|<span data-ttu-id="8b03c-128">version</span><span class="sxs-lookup"><span data-stu-id="8b03c-128">version</span></span>|<span data-ttu-id="8b03c-129">String</span><span class="sxs-lookup"><span data-stu-id="8b03c-129">String</span></span>|<span data-ttu-id="8b03c-130">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="8b03c-130">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b03c-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8b03c-131">Relationships</span></span>
<span data-ttu-id="8b03c-132">なし</span><span class="sxs-lookup"><span data-stu-id="8b03c-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8b03c-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8b03c-133">JSON Representation</span></span>
<span data-ttu-id="8b03c-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8b03c-134">Here is a JSON representation of the resource.</span></span>
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





