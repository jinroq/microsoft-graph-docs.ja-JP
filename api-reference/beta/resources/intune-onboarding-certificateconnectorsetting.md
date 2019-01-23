---
title: certificateConnectorSetting リソースの種類
description: コネクタの設定を証明書です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5886418aaddede43f2397ad626028598a63a0066
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398654"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="82606-103">certificateConnectorSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="82606-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="82606-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="82606-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="82606-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82606-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82606-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="82606-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82606-107">コネクタの設定を証明書です。</span><span class="sxs-lookup"><span data-stu-id="82606-107">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="82606-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82606-108">Properties</span></span>
|<span data-ttu-id="82606-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82606-109">Property</span></span>|<span data-ttu-id="82606-110">型</span><span class="sxs-lookup"><span data-stu-id="82606-110">Type</span></span>|<span data-ttu-id="82606-111">説明</span><span class="sxs-lookup"><span data-stu-id="82606-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82606-112">status</span><span class="sxs-lookup"><span data-stu-id="82606-112">status</span></span>|<span data-ttu-id="82606-113">Int32</span><span class="sxs-lookup"><span data-stu-id="82606-113">Int32</span></span>|<span data-ttu-id="82606-114">証明書のコネクタの状態</span><span class="sxs-lookup"><span data-stu-id="82606-114">Certificate connector status</span></span>|
|<span data-ttu-id="82606-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="82606-115">certExpiryTime</span></span>|<span data-ttu-id="82606-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82606-116">DateTimeOffset</span></span>|<span data-ttu-id="82606-117">証明書の有効期限が切れる時間</span><span class="sxs-lookup"><span data-stu-id="82606-117">Certificate expire time</span></span>|
|<span data-ttu-id="82606-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="82606-118">enrollmentError</span></span>|<span data-ttu-id="82606-119">String</span><span class="sxs-lookup"><span data-stu-id="82606-119">String</span></span>|<span data-ttu-id="82606-120">コネクタの登録の証明書のエラー</span><span class="sxs-lookup"><span data-stu-id="82606-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="82606-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="82606-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="82606-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82606-122">DateTimeOffset</span></span>|<span data-ttu-id="82606-123">コネクタが接続されている証明書の最後に</span><span class="sxs-lookup"><span data-stu-id="82606-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="82606-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="82606-124">connectorVersion</span></span>|<span data-ttu-id="82606-125">String</span><span class="sxs-lookup"><span data-stu-id="82606-125">String</span></span>|<span data-ttu-id="82606-126">コネクタの証明書のバージョン</span><span class="sxs-lookup"><span data-stu-id="82606-126">Version of certificate connector</span></span>|
|<span data-ttu-id="82606-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="82606-127">lastUploadVersion</span></span>|<span data-ttu-id="82606-128">Int64</span><span class="sxs-lookup"><span data-stu-id="82606-128">Int64</span></span>|<span data-ttu-id="82606-129">最後の証明書をアップロードしたコネクタのバージョン</span><span class="sxs-lookup"><span data-stu-id="82606-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="82606-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="82606-130">Relationships</span></span>
<span data-ttu-id="82606-131">なし</span><span class="sxs-lookup"><span data-stu-id="82606-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82606-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="82606-132">JSON Representation</span></span>
<span data-ttu-id="82606-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="82606-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certificateConnectorSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorSetting",
  "status": 1024,
  "certExpiryTime": "String (timestamp)",
  "enrollmentError": "String",
  "lastConnectorConnectionTime": "String (timestamp)",
  "connectorVersion": "String",
  "lastUploadVersion": 1024
}
```




