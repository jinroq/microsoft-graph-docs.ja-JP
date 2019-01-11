---
title: managedAppStatus リソースの種類
description: 組織のアプリ保護と構成の状態を表します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 13bf28c0244a3288b949ebf718e3d5ce97ceb60c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890385"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="64d14-103">managedAppStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="64d14-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="64d14-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="64d14-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64d14-105">組織のアプリ保護と構成の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="64d14-105">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="64d14-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="64d14-106">Methods</span></span>
|<span data-ttu-id="64d14-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="64d14-107">Method</span></span>|<span data-ttu-id="64d14-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="64d14-108">Return Type</span></span>|<span data-ttu-id="64d14-109">説明</span><span class="sxs-lookup"><span data-stu-id="64d14-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="64d14-110">List managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="64d14-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="64d14-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="64d14-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="64d14-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="64d14-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="64d14-113">Get managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="64d14-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="64d14-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="64d14-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="64d14-115">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="64d14-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="64d14-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64d14-116">Properties</span></span>
|<span data-ttu-id="64d14-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64d14-117">Property</span></span>|<span data-ttu-id="64d14-118">種類</span><span class="sxs-lookup"><span data-stu-id="64d14-118">Type</span></span>|<span data-ttu-id="64d14-119">説明</span><span class="sxs-lookup"><span data-stu-id="64d14-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64d14-120">displayName</span><span class="sxs-lookup"><span data-stu-id="64d14-120">displayName</span></span>|<span data-ttu-id="64d14-121">String</span><span class="sxs-lookup"><span data-stu-id="64d14-121">String</span></span>|<span data-ttu-id="64d14-122">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="64d14-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="64d14-123">id</span><span class="sxs-lookup"><span data-stu-id="64d14-123">id</span></span>|<span data-ttu-id="64d14-124">String</span><span class="sxs-lookup"><span data-stu-id="64d14-124">String</span></span>|<span data-ttu-id="64d14-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="64d14-125">Key of the entity.</span></span>|
|<span data-ttu-id="64d14-126">version</span><span class="sxs-lookup"><span data-stu-id="64d14-126">version</span></span>|<span data-ttu-id="64d14-127">String</span><span class="sxs-lookup"><span data-stu-id="64d14-127">String</span></span>|<span data-ttu-id="64d14-128">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="64d14-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64d14-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="64d14-129">Relationships</span></span>
<span data-ttu-id="64d14-130">なし</span><span class="sxs-lookup"><span data-stu-id="64d14-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="64d14-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="64d14-131">JSON Representation</span></span>
<span data-ttu-id="64d14-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="64d14-132">Here is a JSON representation of the resource.</span></span>
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



