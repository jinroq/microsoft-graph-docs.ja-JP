---
title: managedAppStatus リソースの種類
description: 組織のアプリ保護と構成の状態を表します。
author: tfitzmac
ms.openlocfilehash: e23b20b53d7ad89a4bbd0df8510a66e0f7da581d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331592"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="75eff-103">managedAppStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="75eff-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="75eff-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="75eff-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75eff-105">組織のアプリ保護と構成の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="75eff-105">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="75eff-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="75eff-106">Methods</span></span>
|<span data-ttu-id="75eff-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="75eff-107">Method</span></span>|<span data-ttu-id="75eff-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="75eff-108">Return Type</span></span>|<span data-ttu-id="75eff-109">説明</span><span class="sxs-lookup"><span data-stu-id="75eff-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="75eff-110">List managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="75eff-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="75eff-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="75eff-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="75eff-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="75eff-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="75eff-113">Get managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="75eff-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="75eff-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="75eff-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="75eff-115">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="75eff-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="75eff-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75eff-116">Properties</span></span>
|<span data-ttu-id="75eff-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75eff-117">Property</span></span>|<span data-ttu-id="75eff-118">種類</span><span class="sxs-lookup"><span data-stu-id="75eff-118">Type</span></span>|<span data-ttu-id="75eff-119">説明</span><span class="sxs-lookup"><span data-stu-id="75eff-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75eff-120">displayName</span><span class="sxs-lookup"><span data-stu-id="75eff-120">displayName</span></span>|<span data-ttu-id="75eff-121">String</span><span class="sxs-lookup"><span data-stu-id="75eff-121">String</span></span>|<span data-ttu-id="75eff-122">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="75eff-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="75eff-123">id</span><span class="sxs-lookup"><span data-stu-id="75eff-123">id</span></span>|<span data-ttu-id="75eff-124">String</span><span class="sxs-lookup"><span data-stu-id="75eff-124">String</span></span>|<span data-ttu-id="75eff-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="75eff-125">Key of the entity.</span></span>|
|<span data-ttu-id="75eff-126">version</span><span class="sxs-lookup"><span data-stu-id="75eff-126">version</span></span>|<span data-ttu-id="75eff-127">String</span><span class="sxs-lookup"><span data-stu-id="75eff-127">String</span></span>|<span data-ttu-id="75eff-128">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="75eff-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75eff-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="75eff-129">Relationships</span></span>
<span data-ttu-id="75eff-130">なし</span><span class="sxs-lookup"><span data-stu-id="75eff-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="75eff-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="75eff-131">JSON Representation</span></span>
<span data-ttu-id="75eff-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="75eff-132">Here is a JSON representation of the resource.</span></span>
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



