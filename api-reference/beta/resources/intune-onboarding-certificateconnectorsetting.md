---
title: certificateConnectorSetting リソースの種類
description: コネクタの設定を証明書です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 74a63d308d53d09b71b19b2ff10a9d94c3fa818d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980994"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="237c5-103">certificateConnectorSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="237c5-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="237c5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="237c5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="237c5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="237c5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="237c5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="237c5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="237c5-107">コネクタの設定を証明書です。</span><span class="sxs-lookup"><span data-stu-id="237c5-107">Certificate connector settings.</span></span>
## <a name="properties"></a><span data-ttu-id="237c5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="237c5-108">Properties</span></span>
|<span data-ttu-id="237c5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="237c5-109">Property</span></span>|<span data-ttu-id="237c5-110">種類</span><span class="sxs-lookup"><span data-stu-id="237c5-110">Type</span></span>|<span data-ttu-id="237c5-111">説明</span><span class="sxs-lookup"><span data-stu-id="237c5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="237c5-112">status</span><span class="sxs-lookup"><span data-stu-id="237c5-112">status</span></span>|<span data-ttu-id="237c5-113">Int32</span><span class="sxs-lookup"><span data-stu-id="237c5-113">Int32</span></span>|<span data-ttu-id="237c5-114">証明書のコネクタの状態</span><span class="sxs-lookup"><span data-stu-id="237c5-114">Certificate connector status</span></span>|
|<span data-ttu-id="237c5-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="237c5-115">certExpiryTime</span></span>|<span data-ttu-id="237c5-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="237c5-116">DateTimeOffset</span></span>|<span data-ttu-id="237c5-117">証明書の有効期限が切れる時間</span><span class="sxs-lookup"><span data-stu-id="237c5-117">Certificate expire time</span></span>|
|<span data-ttu-id="237c5-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="237c5-118">enrollmentError</span></span>|<span data-ttu-id="237c5-119">String</span><span class="sxs-lookup"><span data-stu-id="237c5-119">String</span></span>|<span data-ttu-id="237c5-120">コネクタの登録の証明書のエラー</span><span class="sxs-lookup"><span data-stu-id="237c5-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="237c5-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="237c5-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="237c5-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="237c5-122">DateTimeOffset</span></span>|<span data-ttu-id="237c5-123">コネクタが接続されている証明書の最後に</span><span class="sxs-lookup"><span data-stu-id="237c5-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="237c5-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="237c5-124">connectorVersion</span></span>|<span data-ttu-id="237c5-125">String</span><span class="sxs-lookup"><span data-stu-id="237c5-125">String</span></span>|<span data-ttu-id="237c5-126">コネクタの証明書のバージョン</span><span class="sxs-lookup"><span data-stu-id="237c5-126">Version of certificate connector</span></span>|
|<span data-ttu-id="237c5-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="237c5-127">lastUploadVersion</span></span>|<span data-ttu-id="237c5-128">Int64</span><span class="sxs-lookup"><span data-stu-id="237c5-128">Int64</span></span>|<span data-ttu-id="237c5-129">最後の証明書をアップロードしたコネクタのバージョン</span><span class="sxs-lookup"><span data-stu-id="237c5-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="237c5-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="237c5-130">Relationships</span></span>
<span data-ttu-id="237c5-131">なし</span><span class="sxs-lookup"><span data-stu-id="237c5-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="237c5-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="237c5-132">JSON Representation</span></span>
<span data-ttu-id="237c5-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="237c5-133">Here is a JSON representation of the resource.</span></span>
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





