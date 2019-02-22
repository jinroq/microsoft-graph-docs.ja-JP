---
title: certificateConnectorSetting リソースの種類
description: 証明書コネクタの設定。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 09f4baf9ddd8be630c432fcec5d7df71c442bbe2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168307"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="58b1a-103">certificateConnectorSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="58b1a-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="58b1a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58b1a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58b1a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="58b1a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58b1a-106">証明書コネクタの設定。</span><span class="sxs-lookup"><span data-stu-id="58b1a-106">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="58b1a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58b1a-107">Properties</span></span>
|<span data-ttu-id="58b1a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58b1a-108">Property</span></span>|<span data-ttu-id="58b1a-109">型</span><span class="sxs-lookup"><span data-stu-id="58b1a-109">Type</span></span>|<span data-ttu-id="58b1a-110">説明</span><span class="sxs-lookup"><span data-stu-id="58b1a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58b1a-111">status</span><span class="sxs-lookup"><span data-stu-id="58b1a-111">status</span></span>|<span data-ttu-id="58b1a-112">Int32</span><span class="sxs-lookup"><span data-stu-id="58b1a-112">Int32</span></span>|<span data-ttu-id="58b1a-113">証明書コネクタの状態</span><span class="sxs-lookup"><span data-stu-id="58b1a-113">Certificate connector status</span></span>|
|<span data-ttu-id="58b1a-114">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="58b1a-114">certExpiryTime</span></span>|<span data-ttu-id="58b1a-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58b1a-115">DateTimeOffset</span></span>|<span data-ttu-id="58b1a-116">証明書の有効期限</span><span class="sxs-lookup"><span data-stu-id="58b1a-116">Certificate expire time</span></span>|
|<span data-ttu-id="58b1a-117">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="58b1a-117">enrollmentError</span></span>|<span data-ttu-id="58b1a-118">String</span><span class="sxs-lookup"><span data-stu-id="58b1a-118">String</span></span>|<span data-ttu-id="58b1a-119">証明書コネクタの登録エラー</span><span class="sxs-lookup"><span data-stu-id="58b1a-119">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="58b1a-120">lastコネクタ接続時間</span><span class="sxs-lookup"><span data-stu-id="58b1a-120">lastConnectorConnectionTime</span></span>|<span data-ttu-id="58b1a-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58b1a-121">DateTimeOffset</span></span>|<span data-ttu-id="58b1a-122">証明書コネクタが前回接続された日時</span><span class="sxs-lookup"><span data-stu-id="58b1a-122">Last time certificate connector connected</span></span>|
|<span data-ttu-id="58b1a-123">コネクタのバージョン</span><span class="sxs-lookup"><span data-stu-id="58b1a-123">connectorVersion</span></span>|<span data-ttu-id="58b1a-124">String</span><span class="sxs-lookup"><span data-stu-id="58b1a-124">String</span></span>|<span data-ttu-id="58b1a-125">証明書コネクタのバージョン</span><span class="sxs-lookup"><span data-stu-id="58b1a-125">Version of certificate connector</span></span>|
|<span data-ttu-id="58b1a-126">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="58b1a-126">lastUploadVersion</span></span>|<span data-ttu-id="58b1a-127">Int64</span><span class="sxs-lookup"><span data-stu-id="58b1a-127">Int64</span></span>|<span data-ttu-id="58b1a-128">最後にアップロードされた証明書コネクタのバージョン</span><span class="sxs-lookup"><span data-stu-id="58b1a-128">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="58b1a-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="58b1a-129">Relationships</span></span>
<span data-ttu-id="58b1a-130">なし</span><span class="sxs-lookup"><span data-stu-id="58b1a-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58b1a-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="58b1a-131">JSON Representation</span></span>
<span data-ttu-id="58b1a-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="58b1a-132">Here is a JSON representation of the resource.</span></span>
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




