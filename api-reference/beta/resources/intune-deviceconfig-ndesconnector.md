---
title: ndesConnector リソースの種類
description: Ndes の OnPrem コネクタを表すエンティティです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 582d49ccd9a5d61c144e3ef915994302515dbe40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884918"
---
# <a name="ndesconnector-resource-type"></a><span data-ttu-id="41bc8-103">ndesConnector リソースの種類</span><span class="sxs-lookup"><span data-stu-id="41bc8-103">ndesConnector resource type</span></span>

> <span data-ttu-id="41bc8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="41bc8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41bc8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41bc8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="41bc8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="41bc8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41bc8-107">Ndes の OnPrem コネクタを表すエンティティです。</span><span class="sxs-lookup"><span data-stu-id="41bc8-107">Entity which represents an OnPrem Ndes connector.</span></span>
## <a name="methods"></a><span data-ttu-id="41bc8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="41bc8-108">Methods</span></span>
|<span data-ttu-id="41bc8-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="41bc8-109">Method</span></span>|<span data-ttu-id="41bc8-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="41bc8-110">Return Type</span></span>|<span data-ttu-id="41bc8-111">説明</span><span class="sxs-lookup"><span data-stu-id="41bc8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="41bc8-112">リスト ndesConnectors</span><span class="sxs-lookup"><span data-stu-id="41bc8-112">List ndesConnectors</span></span>](../api/intune-deviceconfig-ndesconnector-list.md)|<span data-ttu-id="41bc8-113">[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="41bc8-113">[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) collection</span></span>|<span data-ttu-id="41bc8-114">[NdesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="41bc8-114">List properties and relationships of the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) objects.</span></span>|
|[<span data-ttu-id="41bc8-115">NdesConnector を取得します。</span><span class="sxs-lookup"><span data-stu-id="41bc8-115">Get ndesConnector</span></span>](../api/intune-deviceconfig-ndesconnector-get.md)|[<span data-ttu-id="41bc8-116">ndesConnector</span><span class="sxs-lookup"><span data-stu-id="41bc8-116">ndesConnector</span></span>](../resources/intune-deviceconfig-ndesconnector.md)|<span data-ttu-id="41bc8-117">[NdesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41bc8-117">Read properties and relationships of the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>|
|[<span data-ttu-id="41bc8-118">NdesConnector を作成します。</span><span class="sxs-lookup"><span data-stu-id="41bc8-118">Create ndesConnector</span></span>](../api/intune-deviceconfig-ndesconnector-create.md)|[<span data-ttu-id="41bc8-119">ndesConnector</span><span class="sxs-lookup"><span data-stu-id="41bc8-119">ndesConnector</span></span>](../resources/intune-deviceconfig-ndesconnector.md)|<span data-ttu-id="41bc8-120">新しい[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="41bc8-120">Create a new [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>|
|[<span data-ttu-id="41bc8-121">NdesConnector を削除します。</span><span class="sxs-lookup"><span data-stu-id="41bc8-121">Delete ndesConnector</span></span>](../api/intune-deviceconfig-ndesconnector-delete.md)|<span data-ttu-id="41bc8-122">なし</span><span class="sxs-lookup"><span data-stu-id="41bc8-122">None</span></span>|<span data-ttu-id="41bc8-123">の[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="41bc8-123">Deletes a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>|
|[<span data-ttu-id="41bc8-124">NdesConnector を更新します。</span><span class="sxs-lookup"><span data-stu-id="41bc8-124">Update ndesConnector</span></span>](../api/intune-deviceconfig-ndesconnector-update.md)|[<span data-ttu-id="41bc8-125">ndesConnector</span><span class="sxs-lookup"><span data-stu-id="41bc8-125">ndesConnector</span></span>](../resources/intune-deviceconfig-ndesconnector.md)|<span data-ttu-id="41bc8-126">[NdesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="41bc8-126">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="41bc8-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41bc8-127">Properties</span></span>
|<span data-ttu-id="41bc8-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41bc8-128">Property</span></span>|<span data-ttu-id="41bc8-129">種類</span><span class="sxs-lookup"><span data-stu-id="41bc8-129">Type</span></span>|<span data-ttu-id="41bc8-130">説明</span><span class="sxs-lookup"><span data-stu-id="41bc8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41bc8-131">ID</span><span class="sxs-lookup"><span data-stu-id="41bc8-131">id</span></span>|<span data-ttu-id="41bc8-132">String</span><span class="sxs-lookup"><span data-stu-id="41bc8-132">String</span></span>|<span data-ttu-id="41bc8-133">NDES のコネクタのキー。</span><span class="sxs-lookup"><span data-stu-id="41bc8-133">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="41bc8-134">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="41bc8-134">lastConnectionDateTime</span></span>|<span data-ttu-id="41bc8-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41bc8-135">DateTimeOffset</span></span>|<span data-ttu-id="41bc8-136">Ndes コネクタの前回の接続</span><span class="sxs-lookup"><span data-stu-id="41bc8-136">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="41bc8-137">state</span><span class="sxs-lookup"><span data-stu-id="41bc8-137">state</span></span>|[<span data-ttu-id="41bc8-138">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="41bc8-138">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="41bc8-139">Ndes のコネクタの状態です。</span><span class="sxs-lookup"><span data-stu-id="41bc8-139">Ndes Connector Status.</span></span> <span data-ttu-id="41bc8-140">可能な値は、`none`、`active`、`inactive` です。</span><span class="sxs-lookup"><span data-stu-id="41bc8-140">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="41bc8-141">displayName</span><span class="sxs-lookup"><span data-stu-id="41bc8-141">displayName</span></span>|<span data-ttu-id="41bc8-142">String</span><span class="sxs-lookup"><span data-stu-id="41bc8-142">String</span></span>|<span data-ttu-id="41bc8-143">Ndes のコネクタの表示名。</span><span class="sxs-lookup"><span data-stu-id="41bc8-143">The friendly name of the Ndes Connector.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41bc8-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="41bc8-144">Relationships</span></span>
<span data-ttu-id="41bc8-145">なし</span><span class="sxs-lookup"><span data-stu-id="41bc8-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="41bc8-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="41bc8-146">JSON Representation</span></span>
<span data-ttu-id="41bc8-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="41bc8-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ndesConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "String (identifier)",
  "lastConnectionDateTime": "String (timestamp)",
  "state": "String",
  "displayName": "String"
}
```





