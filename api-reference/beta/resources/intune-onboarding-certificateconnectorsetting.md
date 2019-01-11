---
title: certificateConnectorSetting リソースの種類
description: コネクタの設定を証明書です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 56f12600b6aa78982dc51732d685dcd7c962d0b0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888600"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="bec90-103">certificateConnectorSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bec90-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="bec90-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bec90-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bec90-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bec90-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bec90-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bec90-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bec90-107">コネクタの設定を証明書です。</span><span class="sxs-lookup"><span data-stu-id="bec90-107">Certificate connector settings.</span></span>
## <a name="properties"></a><span data-ttu-id="bec90-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bec90-108">Properties</span></span>
|<span data-ttu-id="bec90-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bec90-109">Property</span></span>|<span data-ttu-id="bec90-110">種類</span><span class="sxs-lookup"><span data-stu-id="bec90-110">Type</span></span>|<span data-ttu-id="bec90-111">説明</span><span class="sxs-lookup"><span data-stu-id="bec90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bec90-112">status</span><span class="sxs-lookup"><span data-stu-id="bec90-112">status</span></span>|<span data-ttu-id="bec90-113">Int32</span><span class="sxs-lookup"><span data-stu-id="bec90-113">Int32</span></span>|<span data-ttu-id="bec90-114">証明書のコネクタの状態</span><span class="sxs-lookup"><span data-stu-id="bec90-114">Certificate connector status</span></span>|
|<span data-ttu-id="bec90-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="bec90-115">certExpiryTime</span></span>|<span data-ttu-id="bec90-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bec90-116">DateTimeOffset</span></span>|<span data-ttu-id="bec90-117">証明書の有効期限が切れる時間</span><span class="sxs-lookup"><span data-stu-id="bec90-117">Certificate expire time</span></span>|
|<span data-ttu-id="bec90-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="bec90-118">enrollmentError</span></span>|<span data-ttu-id="bec90-119">String</span><span class="sxs-lookup"><span data-stu-id="bec90-119">String</span></span>|<span data-ttu-id="bec90-120">コネクタの登録の証明書のエラー</span><span class="sxs-lookup"><span data-stu-id="bec90-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="bec90-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="bec90-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="bec90-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bec90-122">DateTimeOffset</span></span>|<span data-ttu-id="bec90-123">コネクタが接続されている証明書の最後に</span><span class="sxs-lookup"><span data-stu-id="bec90-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="bec90-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="bec90-124">connectorVersion</span></span>|<span data-ttu-id="bec90-125">String</span><span class="sxs-lookup"><span data-stu-id="bec90-125">String</span></span>|<span data-ttu-id="bec90-126">コネクタの証明書のバージョン</span><span class="sxs-lookup"><span data-stu-id="bec90-126">Version of certificate connector</span></span>|
|<span data-ttu-id="bec90-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="bec90-127">lastUploadVersion</span></span>|<span data-ttu-id="bec90-128">Int64</span><span class="sxs-lookup"><span data-stu-id="bec90-128">Int64</span></span>|<span data-ttu-id="bec90-129">最後の証明書をアップロードしたコネクタのバージョン</span><span class="sxs-lookup"><span data-stu-id="bec90-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="bec90-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bec90-130">Relationships</span></span>
<span data-ttu-id="bec90-131">なし</span><span class="sxs-lookup"><span data-stu-id="bec90-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bec90-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bec90-132">JSON Representation</span></span>
<span data-ttu-id="bec90-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bec90-133">Here is a JSON representation of the resource.</span></span>
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





