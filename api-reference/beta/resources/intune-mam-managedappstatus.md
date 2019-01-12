---
title: managedAppStatus リソースの種類
description: 組織のアプリ保護と構成の状態を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac7e2c727bce9da64e9262e3e3165a0bcc024623
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923713"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="37ad5-103">managedAppStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="37ad5-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="37ad5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="37ad5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37ad5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37ad5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37ad5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="37ad5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37ad5-107">組織のアプリ保護と構成の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="37ad5-107">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="37ad5-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="37ad5-108">Methods</span></span>
|<span data-ttu-id="37ad5-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="37ad5-109">Method</span></span>|<span data-ttu-id="37ad5-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="37ad5-110">Return Type</span></span>|<span data-ttu-id="37ad5-111">説明</span><span class="sxs-lookup"><span data-stu-id="37ad5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="37ad5-112">List managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="37ad5-112">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="37ad5-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="37ad5-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="37ad5-114">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="37ad5-114">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="37ad5-115">Get managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="37ad5-115">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="37ad5-116">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="37ad5-116">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="37ad5-117">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="37ad5-117">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="37ad5-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37ad5-118">Properties</span></span>
|<span data-ttu-id="37ad5-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37ad5-119">Property</span></span>|<span data-ttu-id="37ad5-120">種類</span><span class="sxs-lookup"><span data-stu-id="37ad5-120">Type</span></span>|<span data-ttu-id="37ad5-121">説明</span><span class="sxs-lookup"><span data-stu-id="37ad5-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37ad5-122">displayName</span><span class="sxs-lookup"><span data-stu-id="37ad5-122">displayName</span></span>|<span data-ttu-id="37ad5-123">String</span><span class="sxs-lookup"><span data-stu-id="37ad5-123">String</span></span>|<span data-ttu-id="37ad5-124">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="37ad5-124">Friendly name of the status report.</span></span>|
|<span data-ttu-id="37ad5-125">id</span><span class="sxs-lookup"><span data-stu-id="37ad5-125">id</span></span>|<span data-ttu-id="37ad5-126">String</span><span class="sxs-lookup"><span data-stu-id="37ad5-126">String</span></span>|<span data-ttu-id="37ad5-127">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="37ad5-127">Key of the entity.</span></span>|
|<span data-ttu-id="37ad5-128">version</span><span class="sxs-lookup"><span data-stu-id="37ad5-128">version</span></span>|<span data-ttu-id="37ad5-129">String</span><span class="sxs-lookup"><span data-stu-id="37ad5-129">String</span></span>|<span data-ttu-id="37ad5-130">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="37ad5-130">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37ad5-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="37ad5-131">Relationships</span></span>
<span data-ttu-id="37ad5-132">なし</span><span class="sxs-lookup"><span data-stu-id="37ad5-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="37ad5-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="37ad5-133">JSON Representation</span></span>
<span data-ttu-id="37ad5-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="37ad5-134">Here is a JSON representation of the resource.</span></span>
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





