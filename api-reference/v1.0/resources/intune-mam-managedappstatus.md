---
title: managedAppStatus リソースの種類
description: 組織のアプリ保護と構成の状態を表します。
ms.openlocfilehash: d25770468341e1f62e96273c6c925d322b385c89
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022575"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="7244e-103">managedAppStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7244e-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="7244e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7244e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7244e-105">組織のアプリ保護と構成の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="7244e-105">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="7244e-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="7244e-106">Methods</span></span>
|<span data-ttu-id="7244e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="7244e-107">Method</span></span>|<span data-ttu-id="7244e-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7244e-108">Return Type</span></span>|<span data-ttu-id="7244e-109">説明</span><span class="sxs-lookup"><span data-stu-id="7244e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7244e-110">List managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="7244e-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="7244e-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7244e-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="7244e-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7244e-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="7244e-113">Get managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="7244e-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="7244e-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="7244e-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="7244e-115">[managedAppStatus](../resources/intune-mam-managedappstatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7244e-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7244e-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7244e-116">Properties</span></span>
|<span data-ttu-id="7244e-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7244e-117">Property</span></span>|<span data-ttu-id="7244e-118">型</span><span class="sxs-lookup"><span data-stu-id="7244e-118">Type</span></span>|<span data-ttu-id="7244e-119">説明</span><span class="sxs-lookup"><span data-stu-id="7244e-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7244e-120">displayName</span><span class="sxs-lookup"><span data-stu-id="7244e-120">displayName</span></span>|<span data-ttu-id="7244e-121">String</span><span class="sxs-lookup"><span data-stu-id="7244e-121">String</span></span>|<span data-ttu-id="7244e-122">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="7244e-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="7244e-123">id</span><span class="sxs-lookup"><span data-stu-id="7244e-123">id</span></span>|<span data-ttu-id="7244e-124">String</span><span class="sxs-lookup"><span data-stu-id="7244e-124">String</span></span>|<span data-ttu-id="7244e-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7244e-125">Key of the entity.</span></span>|
|<span data-ttu-id="7244e-126">version</span><span class="sxs-lookup"><span data-stu-id="7244e-126">version</span></span>|<span data-ttu-id="7244e-127">String</span><span class="sxs-lookup"><span data-stu-id="7244e-127">String</span></span>|<span data-ttu-id="7244e-128">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="7244e-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7244e-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7244e-129">Relationships</span></span>
<span data-ttu-id="7244e-130">なし</span><span class="sxs-lookup"><span data-stu-id="7244e-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7244e-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7244e-131">JSON Representation</span></span>
<span data-ttu-id="7244e-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7244e-132">Here is a JSON representation of the resource.</span></span>
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



