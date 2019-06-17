---
title: deviceManagementDomainJoinConnector リソースの種類
description: ドメイン参加コネクタは、コンピューターアカウント blob の割り当て (および削除) を行うコネクタです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0537d38d87a2cb574ca8984f895ed3796c33703a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35001924"
---
# <a name="devicemanagementdomainjoinconnector-resource-type"></a><span data-ttu-id="2ebc9-103">deviceManagementDomainJoinConnector リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2ebc9-103">deviceManagementDomainJoinConnector resource type</span></span>

> <span data-ttu-id="2ebc9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ebc9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ebc9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2ebc9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ebc9-106">ドメイン参加コネクタは、コンピューターアカウント blob の割り当て (および削除) を行うコネクタです。</span><span class="sxs-lookup"><span data-stu-id="2ebc9-106">A Domain Join Connector is a connector that is responsible to allocate (and delete) machine account blobs</span></span>

## <a name="methods"></a><span data-ttu-id="2ebc9-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="2ebc9-107">Methods</span></span>
|<span data-ttu-id="2ebc9-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="2ebc9-108">Method</span></span>|<span data-ttu-id="2ebc9-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2ebc9-109">Return Type</span></span>|<span data-ttu-id="2ebc9-110">説明</span><span class="sxs-lookup"><span data-stu-id="2ebc9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2ebc9-111">DeviceManagementDomainJoinConnectors を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2ebc9-111">List deviceManagementDomainJoinConnectors</span></span>](../api/intune-odj-devicemanagementdomainjoinconnector-list.md)|<span data-ttu-id="2ebc9-112">[Devicemanagementdomainjoinconnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2ebc9-112">[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) collection</span></span>|<span data-ttu-id="2ebc9-113">[Devicemanagementdomainjoinconnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2ebc9-113">List properties and relationships of the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) objects.</span></span>|
|[<span data-ttu-id="2ebc9-114">DeviceManagementDomainJoinConnector の取得</span><span class="sxs-lookup"><span data-stu-id="2ebc9-114">Get deviceManagementDomainJoinConnector</span></span>](../api/intune-odj-devicemanagementdomainjoinconnector-get.md)|[<span data-ttu-id="2ebc9-115">deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="2ebc9-115">deviceManagementDomainJoinConnector</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|<span data-ttu-id="2ebc9-116">[Devicemanagementdomainjoinconnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2ebc9-116">Read properties and relationships of the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>|
|[<span data-ttu-id="2ebc9-117">DeviceManagementDomainJoinConnector の作成</span><span class="sxs-lookup"><span data-stu-id="2ebc9-117">Create deviceManagementDomainJoinConnector</span></span>](../api/intune-odj-devicemanagementdomainjoinconnector-create.md)|[<span data-ttu-id="2ebc9-118">deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="2ebc9-118">deviceManagementDomainJoinConnector</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|<span data-ttu-id="2ebc9-119">新しい[Devicemanagementdomainjoinconnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2ebc9-119">Create a new [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>|
|[<span data-ttu-id="2ebc9-120">DeviceManagementDomainJoinConnector の削除</span><span class="sxs-lookup"><span data-stu-id="2ebc9-120">Delete deviceManagementDomainJoinConnector</span></span>](../api/intune-odj-devicemanagementdomainjoinconnector-delete.md)|<span data-ttu-id="2ebc9-121">None</span><span class="sxs-lookup"><span data-stu-id="2ebc9-121">None</span></span>|<span data-ttu-id="2ebc9-122">[Devicemanagementdomainjoinconnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="2ebc9-122">Deletes a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md).</span></span>|
|[<span data-ttu-id="2ebc9-123">DeviceManagementDomainJoinConnector の更新</span><span class="sxs-lookup"><span data-stu-id="2ebc9-123">Update deviceManagementDomainJoinConnector</span></span>](../api/intune-odj-devicemanagementdomainjoinconnector-update.md)|[<span data-ttu-id="2ebc9-124">deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="2ebc9-124">deviceManagementDomainJoinConnector</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|<span data-ttu-id="2ebc9-125">[Devicemanagementdomainjoinconnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2ebc9-125">Update the properties of a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2ebc9-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ebc9-126">Properties</span></span>
|<span data-ttu-id="2ebc9-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ebc9-127">Property</span></span>|<span data-ttu-id="2ebc9-128">型</span><span class="sxs-lookup"><span data-stu-id="2ebc9-128">Type</span></span>|<span data-ttu-id="2ebc9-129">説明</span><span class="sxs-lookup"><span data-stu-id="2ebc9-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ebc9-130">id</span><span class="sxs-lookup"><span data-stu-id="2ebc9-130">id</span></span>|<span data-ttu-id="2ebc9-131">文字列</span><span class="sxs-lookup"><span data-stu-id="2ebc9-131">String</span></span>|<span data-ttu-id="2ebc9-132">コネクタを表す一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="2ebc9-132">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="2ebc9-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2ebc9-133">displayName</span></span>|<span data-ttu-id="2ebc9-134">String</span><span class="sxs-lookup"><span data-stu-id="2ebc9-134">String</span></span>|<span data-ttu-id="2ebc9-135">コネクタの表示名。</span><span class="sxs-lookup"><span data-stu-id="2ebc9-135">The connector display name.</span></span>|
|<span data-ttu-id="2ebc9-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="2ebc9-136">lastConnectionDateTime</span></span>|<span data-ttu-id="2ebc9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ebc9-137">DateTimeOffset</span></span>|<span data-ttu-id="2ebc9-138">前回のコネクタが Intune に接続した時刻。</span><span class="sxs-lookup"><span data-stu-id="2ebc9-138">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="2ebc9-139">state</span><span class="sxs-lookup"><span data-stu-id="2ebc9-139">state</span></span>|[<span data-ttu-id="2ebc9-140">Devicemanagementdomainjoinコネクタ状態</span><span class="sxs-lookup"><span data-stu-id="2ebc9-140">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="2ebc9-141">コネクタの状態です。</span><span class="sxs-lookup"><span data-stu-id="2ebc9-141">The connector state.</span></span> <span data-ttu-id="2ebc9-142">可能な値は、`active`、`error`、`inactive` です。</span><span class="sxs-lookup"><span data-stu-id="2ebc9-142">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="2ebc9-143">version</span><span class="sxs-lookup"><span data-stu-id="2ebc9-143">version</span></span>|<span data-ttu-id="2ebc9-144">String</span><span class="sxs-lookup"><span data-stu-id="2ebc9-144">String</span></span>|<span data-ttu-id="2ebc9-145">コネクタのバージョン。</span><span class="sxs-lookup"><span data-stu-id="2ebc9-145">The version of the connector.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ebc9-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2ebc9-146">Relationships</span></span>
<span data-ttu-id="2ebc9-147">なし</span><span class="sxs-lookup"><span data-stu-id="2ebc9-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ebc9-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2ebc9-148">JSON Representation</span></span>
<span data-ttu-id="2ebc9-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2ebc9-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementDomainJoinConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "lastConnectionDateTime": "String (timestamp)",
  "state": "String",
  "version": "String"
}
```





