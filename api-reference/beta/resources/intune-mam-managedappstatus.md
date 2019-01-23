---
title: managedAppStatus リソースの種類
description: 組織のアプリ保護と構成の状態を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7625543106b1ccf019df9622c1b0f37d40232f0c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415566"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="cd976-103">managedAppStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cd976-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="cd976-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cd976-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cd976-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd976-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cd976-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cd976-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd976-107">組織のアプリ保護と構成の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="cd976-107">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="cd976-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="cd976-108">Methods</span></span>
|<span data-ttu-id="cd976-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="cd976-109">Method</span></span>|<span data-ttu-id="cd976-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cd976-110">Return Type</span></span>|<span data-ttu-id="cd976-111">説明</span><span class="sxs-lookup"><span data-stu-id="cd976-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cd976-112">List managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="cd976-112">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="cd976-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cd976-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="cd976-114">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="cd976-114">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="cd976-115">Get managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="cd976-115">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="cd976-116">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="cd976-116">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="cd976-117">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="cd976-117">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cd976-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd976-118">Properties</span></span>
|<span data-ttu-id="cd976-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd976-119">Property</span></span>|<span data-ttu-id="cd976-120">型</span><span class="sxs-lookup"><span data-stu-id="cd976-120">Type</span></span>|<span data-ttu-id="cd976-121">説明</span><span class="sxs-lookup"><span data-stu-id="cd976-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd976-122">displayName</span><span class="sxs-lookup"><span data-stu-id="cd976-122">displayName</span></span>|<span data-ttu-id="cd976-123">String</span><span class="sxs-lookup"><span data-stu-id="cd976-123">String</span></span>|<span data-ttu-id="cd976-124">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="cd976-124">Friendly name of the status report.</span></span>|
|<span data-ttu-id="cd976-125">id</span><span class="sxs-lookup"><span data-stu-id="cd976-125">id</span></span>|<span data-ttu-id="cd976-126">String</span><span class="sxs-lookup"><span data-stu-id="cd976-126">String</span></span>|<span data-ttu-id="cd976-127">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cd976-127">Key of the entity.</span></span>|
|<span data-ttu-id="cd976-128">version</span><span class="sxs-lookup"><span data-stu-id="cd976-128">version</span></span>|<span data-ttu-id="cd976-129">String</span><span class="sxs-lookup"><span data-stu-id="cd976-129">String</span></span>|<span data-ttu-id="cd976-130">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="cd976-130">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd976-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cd976-131">Relationships</span></span>
<span data-ttu-id="cd976-132">なし</span><span class="sxs-lookup"><span data-stu-id="cd976-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd976-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cd976-133">JSON Representation</span></span>
<span data-ttu-id="cd976-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cd976-134">Here is a JSON representation of the resource.</span></span>
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




