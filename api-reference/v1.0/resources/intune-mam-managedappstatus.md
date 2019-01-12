---
title: managedAppStatus リソースの種類
description: 組織のアプリ保護と構成の状態を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b06e52d34cbbfb1e358ee2353c3420f8d129a61e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956935"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="18f4b-103">managedAppStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="18f4b-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="18f4b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="18f4b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18f4b-105">組織のアプリ保護と構成の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="18f4b-105">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="18f4b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="18f4b-106">Methods</span></span>
|<span data-ttu-id="18f4b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="18f4b-107">Method</span></span>|<span data-ttu-id="18f4b-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="18f4b-108">Return Type</span></span>|<span data-ttu-id="18f4b-109">説明</span><span class="sxs-lookup"><span data-stu-id="18f4b-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="18f4b-110">List managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="18f4b-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="18f4b-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="18f4b-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="18f4b-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="18f4b-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="18f4b-113">Get managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="18f4b-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="18f4b-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="18f4b-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="18f4b-115">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="18f4b-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="18f4b-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18f4b-116">Properties</span></span>
|<span data-ttu-id="18f4b-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18f4b-117">Property</span></span>|<span data-ttu-id="18f4b-118">種類</span><span class="sxs-lookup"><span data-stu-id="18f4b-118">Type</span></span>|<span data-ttu-id="18f4b-119">説明</span><span class="sxs-lookup"><span data-stu-id="18f4b-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18f4b-120">displayName</span><span class="sxs-lookup"><span data-stu-id="18f4b-120">displayName</span></span>|<span data-ttu-id="18f4b-121">String</span><span class="sxs-lookup"><span data-stu-id="18f4b-121">String</span></span>|<span data-ttu-id="18f4b-122">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="18f4b-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="18f4b-123">id</span><span class="sxs-lookup"><span data-stu-id="18f4b-123">id</span></span>|<span data-ttu-id="18f4b-124">String</span><span class="sxs-lookup"><span data-stu-id="18f4b-124">String</span></span>|<span data-ttu-id="18f4b-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="18f4b-125">Key of the entity.</span></span>|
|<span data-ttu-id="18f4b-126">version</span><span class="sxs-lookup"><span data-stu-id="18f4b-126">version</span></span>|<span data-ttu-id="18f4b-127">String</span><span class="sxs-lookup"><span data-stu-id="18f4b-127">String</span></span>|<span data-ttu-id="18f4b-128">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="18f4b-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18f4b-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="18f4b-129">Relationships</span></span>
<span data-ttu-id="18f4b-130">なし</span><span class="sxs-lookup"><span data-stu-id="18f4b-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="18f4b-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="18f4b-131">JSON Representation</span></span>
<span data-ttu-id="18f4b-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="18f4b-132">Here is a JSON representation of the resource.</span></span>
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



