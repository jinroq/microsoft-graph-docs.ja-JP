---
title: certificateConnectorSetting リソースの種類
description: 証明書コネクタの設定。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60c7ac990a4eccd1f4faf0fd8f32c42a1e1addba
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36341985"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="d00b4-103">certificateConnectorSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d00b4-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="d00b4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d00b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d00b4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d00b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d00b4-106">証明書コネクタの設定。</span><span class="sxs-lookup"><span data-stu-id="d00b4-106">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="d00b4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d00b4-107">Properties</span></span>
|<span data-ttu-id="d00b4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d00b4-108">Property</span></span>|<span data-ttu-id="d00b4-109">型</span><span class="sxs-lookup"><span data-stu-id="d00b4-109">Type</span></span>|<span data-ttu-id="d00b4-110">説明</span><span class="sxs-lookup"><span data-stu-id="d00b4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d00b4-111">status</span><span class="sxs-lookup"><span data-stu-id="d00b4-111">status</span></span>|<span data-ttu-id="d00b4-112">Int32</span><span class="sxs-lookup"><span data-stu-id="d00b4-112">Int32</span></span>|<span data-ttu-id="d00b4-113">証明書コネクタの状態</span><span class="sxs-lookup"><span data-stu-id="d00b4-113">Certificate connector status</span></span>|
|<span data-ttu-id="d00b4-114">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="d00b4-114">certExpiryTime</span></span>|<span data-ttu-id="d00b4-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d00b4-115">DateTimeOffset</span></span>|<span data-ttu-id="d00b4-116">証明書の有効期限</span><span class="sxs-lookup"><span data-stu-id="d00b4-116">Certificate expire time</span></span>|
|<span data-ttu-id="d00b4-117">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="d00b4-117">enrollmentError</span></span>|<span data-ttu-id="d00b4-118">String</span><span class="sxs-lookup"><span data-stu-id="d00b4-118">String</span></span>|<span data-ttu-id="d00b4-119">証明書コネクタの登録エラー</span><span class="sxs-lookup"><span data-stu-id="d00b4-119">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="d00b4-120">Lastコネクタ接続時間</span><span class="sxs-lookup"><span data-stu-id="d00b4-120">lastConnectorConnectionTime</span></span>|<span data-ttu-id="d00b4-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d00b4-121">DateTimeOffset</span></span>|<span data-ttu-id="d00b4-122">証明書コネクタが前回接続された日時</span><span class="sxs-lookup"><span data-stu-id="d00b4-122">Last time certificate connector connected</span></span>|
|<span data-ttu-id="d00b4-123">コネクタのバージョン</span><span class="sxs-lookup"><span data-stu-id="d00b4-123">connectorVersion</span></span>|<span data-ttu-id="d00b4-124">String</span><span class="sxs-lookup"><span data-stu-id="d00b4-124">String</span></span>|<span data-ttu-id="d00b4-125">証明書コネクタのバージョン</span><span class="sxs-lookup"><span data-stu-id="d00b4-125">Version of certificate connector</span></span>|
|<span data-ttu-id="d00b4-126">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="d00b4-126">lastUploadVersion</span></span>|<span data-ttu-id="d00b4-127">Int64</span><span class="sxs-lookup"><span data-stu-id="d00b4-127">Int64</span></span>|<span data-ttu-id="d00b4-128">最後にアップロードされた証明書コネクタのバージョン</span><span class="sxs-lookup"><span data-stu-id="d00b4-128">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="d00b4-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d00b4-129">Relationships</span></span>
<span data-ttu-id="d00b4-130">なし</span><span class="sxs-lookup"><span data-stu-id="d00b4-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d00b4-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d00b4-131">JSON Representation</span></span>
<span data-ttu-id="d00b4-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d00b4-132">Here is a JSON representation of the resource.</span></span>
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



