---
title: ndesConnector リソースの種類
description: Ndes の OnPrem コネクタを表すエンティティです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b504173c0a56e15fd2a4ba09ce50beeabbb20edc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411149"
---
# <a name="ndesconnector-resource-type"></a><span data-ttu-id="d4cf5-103">ndesConnector リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d4cf5-103">ndesConnector resource type</span></span>

> <span data-ttu-id="d4cf5-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d4cf5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d4cf5-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4cf5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4cf5-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d4cf5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4cf5-107">Ndes の OnPrem コネクタを表すエンティティです。</span><span class="sxs-lookup"><span data-stu-id="d4cf5-107">Entity which represents an OnPrem Ndes connector.</span></span>

## <a name="methods"></a><span data-ttu-id="d4cf5-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d4cf5-108">Methods</span></span>
|<span data-ttu-id="d4cf5-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d4cf5-109">Method</span></span>|<span data-ttu-id="d4cf5-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d4cf5-110">Return Type</span></span>|<span data-ttu-id="d4cf5-111">説明</span><span class="sxs-lookup"><span data-stu-id="d4cf5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d4cf5-112">リスト ndesConnectors</span><span class="sxs-lookup"><span data-stu-id="d4cf5-112">List ndesConnectors</span></span>](../api/intune-deviceconfig-ndesconnector-list.md)|<span data-ttu-id="d4cf5-113">[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d4cf5-113">[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) collection</span></span>|<span data-ttu-id="d4cf5-114">[NdesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d4cf5-114">List properties and relationships of the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) objects.</span></span>|
|[<span data-ttu-id="d4cf5-115">NdesConnector を取得します。</span><span class="sxs-lookup"><span data-stu-id="d4cf5-115">Get ndesConnector</span></span>](../api/intune-deviceconfig-ndesconnector-get.md)|[<span data-ttu-id="d4cf5-116">ndesConnector</span><span class="sxs-lookup"><span data-stu-id="d4cf5-116">ndesConnector</span></span>](../resources/intune-deviceconfig-ndesconnector.md)|<span data-ttu-id="d4cf5-117">[NdesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4cf5-117">Read properties and relationships of the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>|
|[<span data-ttu-id="d4cf5-118">NdesConnector を作成します。</span><span class="sxs-lookup"><span data-stu-id="d4cf5-118">Create ndesConnector</span></span>](../api/intune-deviceconfig-ndesconnector-create.md)|[<span data-ttu-id="d4cf5-119">ndesConnector</span><span class="sxs-lookup"><span data-stu-id="d4cf5-119">ndesConnector</span></span>](../resources/intune-deviceconfig-ndesconnector.md)|<span data-ttu-id="d4cf5-120">新しい[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d4cf5-120">Create a new [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>|
|[<span data-ttu-id="d4cf5-121">NdesConnector を削除します。</span><span class="sxs-lookup"><span data-stu-id="d4cf5-121">Delete ndesConnector</span></span>](../api/intune-deviceconfig-ndesconnector-delete.md)|<span data-ttu-id="d4cf5-122">なし</span><span class="sxs-lookup"><span data-stu-id="d4cf5-122">None</span></span>|<span data-ttu-id="d4cf5-123">の[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="d4cf5-123">Deletes a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>|
|[<span data-ttu-id="d4cf5-124">NdesConnector を更新します。</span><span class="sxs-lookup"><span data-stu-id="d4cf5-124">Update ndesConnector</span></span>](../api/intune-deviceconfig-ndesconnector-update.md)|[<span data-ttu-id="d4cf5-125">ndesConnector</span><span class="sxs-lookup"><span data-stu-id="d4cf5-125">ndesConnector</span></span>](../resources/intune-deviceconfig-ndesconnector.md)|<span data-ttu-id="d4cf5-126">[NdesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d4cf5-126">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d4cf5-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4cf5-127">Properties</span></span>
|<span data-ttu-id="d4cf5-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4cf5-128">Property</span></span>|<span data-ttu-id="d4cf5-129">型</span><span class="sxs-lookup"><span data-stu-id="d4cf5-129">Type</span></span>|<span data-ttu-id="d4cf5-130">説明</span><span class="sxs-lookup"><span data-stu-id="d4cf5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4cf5-131">id</span><span class="sxs-lookup"><span data-stu-id="d4cf5-131">id</span></span>|<span data-ttu-id="d4cf5-132">String</span><span class="sxs-lookup"><span data-stu-id="d4cf5-132">String</span></span>|<span data-ttu-id="d4cf5-133">NDES のコネクタのキー。</span><span class="sxs-lookup"><span data-stu-id="d4cf5-133">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="d4cf5-134">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="d4cf5-134">lastConnectionDateTime</span></span>|<span data-ttu-id="d4cf5-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4cf5-135">DateTimeOffset</span></span>|<span data-ttu-id="d4cf5-136">Ndes コネクタの前回の接続</span><span class="sxs-lookup"><span data-stu-id="d4cf5-136">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="d4cf5-137">state</span><span class="sxs-lookup"><span data-stu-id="d4cf5-137">state</span></span>|[<span data-ttu-id="d4cf5-138">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="d4cf5-138">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="d4cf5-139">Ndes のコネクタの状態です。</span><span class="sxs-lookup"><span data-stu-id="d4cf5-139">Ndes Connector Status.</span></span> <span data-ttu-id="d4cf5-140">可能な値は、`none`、`active`、`inactive` です。</span><span class="sxs-lookup"><span data-stu-id="d4cf5-140">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="d4cf5-141">displayName</span><span class="sxs-lookup"><span data-stu-id="d4cf5-141">displayName</span></span>|<span data-ttu-id="d4cf5-142">String</span><span class="sxs-lookup"><span data-stu-id="d4cf5-142">String</span></span>|<span data-ttu-id="d4cf5-143">Ndes のコネクタの表示名。</span><span class="sxs-lookup"><span data-stu-id="d4cf5-143">The friendly name of the Ndes Connector.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4cf5-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d4cf5-144">Relationships</span></span>
<span data-ttu-id="d4cf5-145">なし</span><span class="sxs-lookup"><span data-stu-id="d4cf5-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4cf5-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d4cf5-146">JSON Representation</span></span>
<span data-ttu-id="d4cf5-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d4cf5-147">Here is a JSON representation of the resource.</span></span>
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




