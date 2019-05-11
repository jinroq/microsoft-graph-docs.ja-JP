---
title: managedAppStatus リソースの種類
description: 組織のアプリ保護と構成の状態を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ccfb4aad51d8c0436f6cb8446775c93551d5c99a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940695"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="ceabe-103">managedAppStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ceabe-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="ceabe-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ceabe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ceabe-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ceabe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ceabe-106">組織のアプリ保護と構成の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="ceabe-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="ceabe-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ceabe-107">Methods</span></span>
|<span data-ttu-id="ceabe-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ceabe-108">Method</span></span>|<span data-ttu-id="ceabe-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ceabe-109">Return Type</span></span>|<span data-ttu-id="ceabe-110">説明</span><span class="sxs-lookup"><span data-stu-id="ceabe-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ceabe-111">List managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="ceabe-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="ceabe-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ceabe-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="ceabe-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ceabe-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="ceabe-114">Get managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="ceabe-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="ceabe-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="ceabe-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="ceabe-116">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ceabe-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ceabe-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ceabe-117">Properties</span></span>
|<span data-ttu-id="ceabe-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ceabe-118">Property</span></span>|<span data-ttu-id="ceabe-119">型</span><span class="sxs-lookup"><span data-stu-id="ceabe-119">Type</span></span>|<span data-ttu-id="ceabe-120">説明</span><span class="sxs-lookup"><span data-stu-id="ceabe-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ceabe-121">displayName</span><span class="sxs-lookup"><span data-stu-id="ceabe-121">displayName</span></span>|<span data-ttu-id="ceabe-122">String</span><span class="sxs-lookup"><span data-stu-id="ceabe-122">String</span></span>|<span data-ttu-id="ceabe-123">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="ceabe-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="ceabe-124">id</span><span class="sxs-lookup"><span data-stu-id="ceabe-124">id</span></span>|<span data-ttu-id="ceabe-125">文字列</span><span class="sxs-lookup"><span data-stu-id="ceabe-125">String</span></span>|<span data-ttu-id="ceabe-126">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ceabe-126">Key of the entity.</span></span>|
|<span data-ttu-id="ceabe-127">version</span><span class="sxs-lookup"><span data-stu-id="ceabe-127">version</span></span>|<span data-ttu-id="ceabe-128">String</span><span class="sxs-lookup"><span data-stu-id="ceabe-128">String</span></span>|<span data-ttu-id="ceabe-129">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="ceabe-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ceabe-130">関係</span><span class="sxs-lookup"><span data-stu-id="ceabe-130">Relationships</span></span>
<span data-ttu-id="ceabe-131">なし</span><span class="sxs-lookup"><span data-stu-id="ceabe-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ceabe-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ceabe-132">JSON Representation</span></span>
<span data-ttu-id="ceabe-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ceabe-133">Here is a JSON representation of the resource.</span></span>
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




