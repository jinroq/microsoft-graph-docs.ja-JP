---
title: deviceManagementExchangeConnector リソースの種類
description: Exchange 環境との接続を表すエンティティです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d37fa88cf84b5e709175c91386b64a867eba41a3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422363"
---
# <a name="devicemanagementexchangeconnector-resource-type"></a><span data-ttu-id="22549-103">deviceManagementExchangeConnector リソースの種類</span><span class="sxs-lookup"><span data-stu-id="22549-103">deviceManagementExchangeConnector resource type</span></span>

> <span data-ttu-id="22549-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="22549-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="22549-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22549-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22549-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="22549-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22549-107">Exchange 環境との接続を表すエンティティです。</span><span class="sxs-lookup"><span data-stu-id="22549-107">Entity which represents a connection to an Exchange environment.</span></span>

## <a name="methods"></a><span data-ttu-id="22549-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="22549-108">Methods</span></span>
|<span data-ttu-id="22549-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="22549-109">Method</span></span>|<span data-ttu-id="22549-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="22549-110">Return Type</span></span>|<span data-ttu-id="22549-111">説明</span><span class="sxs-lookup"><span data-stu-id="22549-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="22549-112">List deviceManagementExchangeConnectors</span><span class="sxs-lookup"><span data-stu-id="22549-112">List deviceManagementExchangeConnectors</span></span>](../api/intune-onboarding-devicemanagementexchangeconnector-list.md)|<span data-ttu-id="22549-113">[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="22549-113">[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) collection</span></span>|<span data-ttu-id="22549-114">[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="22549-114">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects.</span></span>|
|[<span data-ttu-id="22549-115">Get deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="22549-115">Get deviceManagementExchangeConnector</span></span>](../api/intune-onboarding-devicemanagementexchangeconnector-get.md)|[<span data-ttu-id="22549-116">deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="22549-116">deviceManagementExchangeConnector</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|<span data-ttu-id="22549-117">[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="22549-117">Read properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>|
|[<span data-ttu-id="22549-118">Create deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="22549-118">Create deviceManagementExchangeConnector</span></span>](../api/intune-onboarding-devicemanagementexchangeconnector-create.md)|[<span data-ttu-id="22549-119">deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="22549-119">deviceManagementExchangeConnector</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|<span data-ttu-id="22549-120">新しい [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="22549-120">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>|
|[<span data-ttu-id="22549-121">Delete deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="22549-121">Delete deviceManagementExchangeConnector</span></span>](../api/intune-onboarding-devicemanagementexchangeconnector-delete.md)|<span data-ttu-id="22549-122">なし</span><span class="sxs-lookup"><span data-stu-id="22549-122">None</span></span>|<span data-ttu-id="22549-123">[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="22549-123">Deletes a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>|
|[<span data-ttu-id="22549-124">Update deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="22549-124">Update deviceManagementExchangeConnector</span></span>](../api/intune-onboarding-devicemanagementexchangeconnector-update.md)|[<span data-ttu-id="22549-125">deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="22549-125">deviceManagementExchangeConnector</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|<span data-ttu-id="22549-126">[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="22549-126">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>|
|[<span data-ttu-id="22549-127">同期アクション</span><span class="sxs-lookup"><span data-stu-id="22549-127">sync action</span></span>](../api/intune-onboarding-devicemanagementexchangeconnector-sync.md)|<span data-ttu-id="22549-128">なし</span><span class="sxs-lookup"><span data-stu-id="22549-128">None</span></span>|<span data-ttu-id="22549-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="22549-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="22549-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22549-130">Properties</span></span>
|<span data-ttu-id="22549-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22549-131">Property</span></span>|<span data-ttu-id="22549-132">型</span><span class="sxs-lookup"><span data-stu-id="22549-132">Type</span></span>|<span data-ttu-id="22549-133">説明</span><span class="sxs-lookup"><span data-stu-id="22549-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22549-134">id</span><span class="sxs-lookup"><span data-stu-id="22549-134">id</span></span>|<span data-ttu-id="22549-135">String</span><span class="sxs-lookup"><span data-stu-id="22549-135">String</span></span>|<span data-ttu-id="22549-136">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="22549-136">Not yet documented</span></span>|
|<span data-ttu-id="22549-137">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="22549-137">lastSyncDateTime</span></span>|<span data-ttu-id="22549-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22549-138">DateTimeOffset</span></span>|<span data-ttu-id="22549-139">Exchange Connector の最終同期日時</span><span class="sxs-lookup"><span data-stu-id="22549-139">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="22549-140">status</span><span class="sxs-lookup"><span data-stu-id="22549-140">status</span></span>|[<span data-ttu-id="22549-141">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="22549-141">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="22549-142">Exchange コネクタの状態です。</span><span class="sxs-lookup"><span data-stu-id="22549-142">Exchange Connector Status.</span></span> <span data-ttu-id="22549-143">可能な値は、`none`、`connectionPending`、`connected`、`disconnected` です。</span><span class="sxs-lookup"><span data-stu-id="22549-143">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="22549-144">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="22549-144">primarySmtpAddress</span></span>|<span data-ttu-id="22549-145">String</span><span class="sxs-lookup"><span data-stu-id="22549-145">String</span></span>|<span data-ttu-id="22549-146">サービス間の Exchange Connector を構成するときに使用するメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="22549-146">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="22549-147">serverName</span><span class="sxs-lookup"><span data-stu-id="22549-147">serverName</span></span>|<span data-ttu-id="22549-148">String</span><span class="sxs-lookup"><span data-stu-id="22549-148">String</span></span>|<span data-ttu-id="22549-149">Exchange サーバーの名前です。</span><span class="sxs-lookup"><span data-stu-id="22549-149">The name of the Exchange server.</span></span>|
|<span data-ttu-id="22549-150">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="22549-150">connectorServerName</span></span>|<span data-ttu-id="22549-151">String</span><span class="sxs-lookup"><span data-stu-id="22549-151">String</span></span>|<span data-ttu-id="22549-152">Exchange Connector をホストするサーバーの名前。</span><span class="sxs-lookup"><span data-stu-id="22549-152">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="22549-153">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="22549-153">exchangeConnectorType</span></span>|[<span data-ttu-id="22549-154">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="22549-154">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="22549-155">構成されている Exchange Connector の種類。</span><span class="sxs-lookup"><span data-stu-id="22549-155">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="22549-156">可能な値は、`onPremises`、`hosted`、`serviceToService`、`dedicated` です。</span><span class="sxs-lookup"><span data-stu-id="22549-156">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="22549-157">version</span><span class="sxs-lookup"><span data-stu-id="22549-157">version</span></span>|<span data-ttu-id="22549-158">String</span><span class="sxs-lookup"><span data-stu-id="22549-158">String</span></span>|<span data-ttu-id="22549-159">ExchangeConnectorAgent のバージョン</span><span class="sxs-lookup"><span data-stu-id="22549-159">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="22549-160">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="22549-160">exchangeAlias</span></span>|<span data-ttu-id="22549-161">String</span><span class="sxs-lookup"><span data-stu-id="22549-161">String</span></span>|<span data-ttu-id="22549-162">Exchange Server に割り当てられているエイリアス。</span><span class="sxs-lookup"><span data-stu-id="22549-162">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="22549-163">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="22549-163">exchangeOrganization</span></span>|<span data-ttu-id="22549-164">String</span><span class="sxs-lookup"><span data-stu-id="22549-164">String</span></span>|<span data-ttu-id="22549-165">Exchange Server に対する Exchange 組織</span><span class="sxs-lookup"><span data-stu-id="22549-165">Exchange Organization to the Exchange server</span></span>|

## <a name="relationships"></a><span data-ttu-id="22549-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="22549-166">Relationships</span></span>
<span data-ttu-id="22549-167">なし</span><span class="sxs-lookup"><span data-stu-id="22549-167">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22549-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="22549-168">JSON Representation</span></span>
<span data-ttu-id="22549-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="22549-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExchangeConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "status": "String",
  "primarySmtpAddress": "String",
  "serverName": "String",
  "connectorServerName": "String",
  "exchangeConnectorType": "String",
  "version": "String",
  "exchangeAlias": "String",
  "exchangeOrganization": "String"
}
```




