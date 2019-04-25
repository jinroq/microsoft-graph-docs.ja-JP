---
title: certificateConnectorSetting リソースの種類
description: 証明書コネクタの設定。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6fe154ed3150ae434f8068bc04a56dd6e5b48744
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573061"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="125e8-103">certificateConnectorSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="125e8-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="125e8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="125e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="125e8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="125e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="125e8-106">証明書コネクタの設定。</span><span class="sxs-lookup"><span data-stu-id="125e8-106">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="125e8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="125e8-107">Properties</span></span>
|<span data-ttu-id="125e8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="125e8-108">Property</span></span>|<span data-ttu-id="125e8-109">型</span><span class="sxs-lookup"><span data-stu-id="125e8-109">Type</span></span>|<span data-ttu-id="125e8-110">説明</span><span class="sxs-lookup"><span data-stu-id="125e8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="125e8-111">status</span><span class="sxs-lookup"><span data-stu-id="125e8-111">status</span></span>|<span data-ttu-id="125e8-112">Int32</span><span class="sxs-lookup"><span data-stu-id="125e8-112">Int32</span></span>|<span data-ttu-id="125e8-113">証明書コネクタの状態</span><span class="sxs-lookup"><span data-stu-id="125e8-113">Certificate connector status</span></span>|
|<span data-ttu-id="125e8-114">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="125e8-114">certExpiryTime</span></span>|<span data-ttu-id="125e8-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="125e8-115">DateTimeOffset</span></span>|<span data-ttu-id="125e8-116">証明書の有効期限</span><span class="sxs-lookup"><span data-stu-id="125e8-116">Certificate expire time</span></span>|
|<span data-ttu-id="125e8-117">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="125e8-117">enrollmentError</span></span>|<span data-ttu-id="125e8-118">String</span><span class="sxs-lookup"><span data-stu-id="125e8-118">String</span></span>|<span data-ttu-id="125e8-119">証明書コネクタの登録エラー</span><span class="sxs-lookup"><span data-stu-id="125e8-119">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="125e8-120">lastコネクタ接続時間</span><span class="sxs-lookup"><span data-stu-id="125e8-120">lastConnectorConnectionTime</span></span>|<span data-ttu-id="125e8-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="125e8-121">DateTimeOffset</span></span>|<span data-ttu-id="125e8-122">証明書コネクタが前回接続された日時</span><span class="sxs-lookup"><span data-stu-id="125e8-122">Last time certificate connector connected</span></span>|
|<span data-ttu-id="125e8-123">コネクタのバージョン</span><span class="sxs-lookup"><span data-stu-id="125e8-123">connectorVersion</span></span>|<span data-ttu-id="125e8-124">String</span><span class="sxs-lookup"><span data-stu-id="125e8-124">String</span></span>|<span data-ttu-id="125e8-125">証明書コネクタのバージョン</span><span class="sxs-lookup"><span data-stu-id="125e8-125">Version of certificate connector</span></span>|
|<span data-ttu-id="125e8-126">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="125e8-126">lastUploadVersion</span></span>|<span data-ttu-id="125e8-127">Int64</span><span class="sxs-lookup"><span data-stu-id="125e8-127">Int64</span></span>|<span data-ttu-id="125e8-128">最後にアップロードされた証明書コネクタのバージョン</span><span class="sxs-lookup"><span data-stu-id="125e8-128">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="125e8-129">関係</span><span class="sxs-lookup"><span data-stu-id="125e8-129">Relationships</span></span>
<span data-ttu-id="125e8-130">なし</span><span class="sxs-lookup"><span data-stu-id="125e8-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="125e8-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="125e8-131">JSON Representation</span></span>
<span data-ttu-id="125e8-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="125e8-132">Here is a JSON representation of the resource.</span></span>
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





